# Git 系列学习

## Git 基本使用 && 安装

*   Git官网：[Git (git-scm.com)](https://git-scm.com/)
*   什么是Git：[Git到底是什么? - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/501326715)
*   Git的学习：[尚硅谷新版Git快速入门(3h迅速掌握git)\_哔哩哔哩\_bilibili](https://www.bilibili.com/video/BV1wm4y1z7Dg/?spm_id_from=333.880.my_history.page.click\&vd_source=f34fbb94411729427c7957728faf0df2)
                       [01_尚硅谷_Git_课程介绍_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1vy4y1s7k6?p=1&vd_source=f34fbb94411729427c7957728faf0df2)
*   Git的安装：[Git 详细安装教程（详解 Git 安装过程的每一个步骤）\_git安装\_mukes的博客-CSDN博客](https://blog.csdn.net/mukes/article/details/115693833)
*   Git中文设置：[Git的汉化 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/259270374)
*   Git的用户配置：[git的安装与配置（详细） - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/597447255)
*   分布式和集中式的区别：[集中式版本管理系统和分布式管理系统的区别-集中式vs分布式\_Karagrade的博客-CSDN博客](https://blog.csdn.net/coco1118/article/details/103091872)
*   GitHub Desktop 的安装和使用：[GitHub Desktop的安装和使用「2020.7.8」\_修改github desktop安装目录\_JCtry的博客-CSDN博客](https://blog.csdn.net/JCtry/article/details/107198217)
*   GitHub Desktop 汉化：[【GitHub】GitHub桌面版（GitHubDesktop）安装加汉化教程\_githubdesktop设置汉化\_江奈河的博客-CSDN博客](https://blog.csdn.net/qq_46365857/article/details/112581517)
*   SVN和Git的区别：[SVN和Git 介绍，区别，优缺点以及适用范围\_git和svn的区别和优缺点\_想养一只！的博客-CSDN博客](https://blog.csdn.net/weixin_45151960/article/details/104720654)
*   [Git 教程 | 菜鸟教程 (runoob.com)](https://www.runoob.com/git/git-tutorial.html)

## Git 的使用

1.  设置命令别名：[Git 命令的简写配置(别名)\_git 配置简写\_Lakers2015的博客-CSDN博客](https://blog.csdn.net/Lakers2015/article/details/111872161)
2.  Git添加标签：[使用Git添加Tag的方法\_git add tag\_MinecodeAir的博客-CSDN博客](https://blog.csdn.net/b735098742/article/details/78935748)
3.  Git添加标签：\[Git优雅使用：git tag操作 - 知乎 (zhihu.com)]\(<https://zhuanlan.zhihu.com/p/622331227#:~:text=git打tag操作步骤> 1 查看最新的提交ID，可以使用以下命令： git log -1 --pretty%3Dformat%3A"%H" 2,{标签名} 如果要一次性推送所有本地标签，可以使用以下命令： git push origin --tags 其中， {标签名}是标签的名称。)
4.  Git与Github建立链接：[Github——git本地仓库建立与远程连接（最详细清晰版本！附简化步骤与常见错误）\_github仓库\_你脸上有BUG的博客-CSDN博客](https://blog.csdn.net/qq_29493173/article/details/113094143)
5.  https和ssh：[【git】git中使用https和ssh协议的区别以及它们的用法 - WANNANANANA - 博客园 (cnblogs.com)](https://www.cnblogs.com/wannananana/p/12059806.html)
6.  用户配置：[添加、修改、删除以及查看本地git的用户名和邮箱_linux 删除git global用户-CSDN博客](https://blog.csdn.net/womeng2009/article/details/101124910#:~:text=添加、修改、删除以及查看本地git的用户名和邮箱 1 1.添加 %24 git config --global user.name,4.查看 （1）查看所有： %24 git config --list 1 )
7.  SSH 配置：[git配置SSH - 江风余火 - 博客园 (cnblogs.com)](https://www.cnblogs.com/jiangfengtomhuo/p/8243001.html)

## Git 英文翻译 && 命令解析

| 英文 && 命令                              | 翻译 && 解析                   |
| :---------------------------------------- | :----------------------------- |
| history                                   | 查看历史命令                   |
| git config --global user.name "用户名"    | 配置用户名（全局）             |
| git config --global user.email "用户邮箱" | 配置用户邮箱（全局）           |
| git config --list                         | 查看用户配置                   |
| git init                                  | 初始化命令                     |
| git status                                | 查看文件状态                   |
| Untracked files                           | 红色文件（未提交状态）         |
| git add  文件名                           | 添加文件到暂存区               |
| git add --all                             | 全部文件添加到暂存区           |
| git commit -m "描述信息" 文件名           | 提交到版本库，并描述信息       |
| git log                                   | 查看提交日志                   |
| git log --oneline --graph                 | 精简查看提交日志               |
| git log --oneline --author="yhx"          | 寻找一名叫做 “yhx”作者的commit |
| git rm 文件名 --cached                    | 解除git的控制                  |
| git checkout 文件名                       | 把不下心删除的文件恢复         |
| git reset 版本号                          | 回退到前一次                   |
| git branch 分支名                         | 创建一个分支                   |
| git branch -v                             | 查看分支                       |
| git checkout 分支名                       | 切换分支                       |
| git branch -m 原始分支名 新分支名         | 修改分支名                     |
| git branch -d 分支名  （D：强制删除）     | 删除分支名                     |
| git merge 分支名                          | 合并分支                       |
| git tag 标签名 版本号                     | 添加标签                       |
| git tag -d 标签名                         | 删除标签                       |
| clone                                     | 克隆                           |
| pull                                      | 拉                             |
| push                                      | 推                             |
| git reset --hard 版本号                   | 版本穿梭                       |
| git reflog                                | 查看历史记录                   |
| git rm --caches 文件名                    | 清除暂存区内容                 |
| git reflog                                | 查看提交记录                   |
| git remote -v                             | 查看别名                       |
| git remote remove 别名                    | 删除别名                       |
| git remote add 别名名称  需要别名的链接   | 创建别名                       |
| git push 别名或者https链接  分支名        | 本地代码推送                   |
| git pull   别名或者https链接  分支名      | 远程代码拉取                   |
| git clone 目标链接                        | 克隆远程代码                   |
| origin                                    | 远程仓库别名                   |
| ssh-keygen -t rsa -C ”邮箱“               | 配置ssh密钥                    |
| git push origin 标签名                    | 将创建的标签推送到远程仓库     |
| git update-git-for-windows                | 更新 Git 版本                  |



