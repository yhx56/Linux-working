# GitLab 部署使用

## Centos 7.9 部署 GitLab （RPM 安装）

**RPM 链接：[Index of /gitlab-ce/yum/el7/ | 清华大学开源软件镜像站 | Tsinghua Open Source Mirror](https://mirrors.tuna.tsinghua.edu.cn/gitlab-ce/yum/el7/)**

​                   

​                    **[gitlab/gitlab-ce - Packages · packages.gitlab.com](https://packages.gitlab.com/gitlab/gitlab-ce)**

```
# 创建目录并进入
[root@master1 ~]# mkdir /opt/Software
[root@master1 ~]# cd /opt/Software/

# 下载 RPM 包
[root@master1 Software]# wget https://mirrors.tuna.tsinghua.edu.cn/gitlab-ce/yum/el7/gitlab-ce-15.11.7-ce.0.el7.x86_64.rpm --no-check-certificate

# 安装依赖软件
[root@master1 Software]# yum -y install policycoreutils openssh-server openssh-clients postfix policycoreutils-python

# 开始 RPM 安装
[root@master1 Software]# rpm -ivh gitlab-ce-15.11.7-ce.0.el7.x86_64.rpm

# 修改配置文件
[root@master1 Software]# vim /etc/gitlab/gitlab.rb 

原配置文件：external_url 'http://gitlab.example.com'
修改后：external_url 'http://192.168.1.10:1234'   （本机IP+端口号）

# 重新加载配置文件
[root@master1 Software]# gitlab-ctl reconfigure

# 重新加载配置文件之后，以下表示存放密码的地方
Notes:
Default admin account has been configured with following details:
Username: root
Password: You didn't opt-in to print initial root password to STDOUT.
Password stored to /etc/gitlab/initial_root_password. This file will be cleaned up in first reconfigure run after 24 hours.


# 重启 GitLab
[root@master1 Software]# gitlab-ctl restart

# 关闭防火墙，或者开放防火墙规则
systemctl stop firewalld.service

# 查看密码，并在浏览器输入 IP 和 端口 使用 Root 用户登录
[root@master1 Software]# cat /etc/gitlab/initial_root_password   （查看密码）
```

