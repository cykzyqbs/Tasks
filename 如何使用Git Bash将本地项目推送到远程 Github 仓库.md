## 初始化本地仓库：

找一个本地项目进入该项目的根目录：

在根目录空白处右键点击git bash，出现git的命令行工具：

在命令行中输入：git init

到此本地仓库就初始化成功了。

## 创建秘钥：

本地仓库连接远程的仓库需要秘钥：

在某个磁盘任何地方创建一个.ssh文件夹 。成功创建后，进入.ssh目录右键点击git bash输入：ssh-keygen -t rsa -C ["](mailto:"18860433348@163.com)youremail@example.com" 然后给保存私钥的文件起一个名字。之后就会有两个文件，一个私钥文件，一个公钥文件。

## 把公钥粘贴到GitHub:

登录github,点击settings，创建一个ssh key，把公钥文件中的秘钥粘贴进去吗，粘贴好后点击add.



## 创建仓库：

返回github首页，点击创建一个新仓库：

## 建立本地仓库与远程仓库链接：

在项目根目录右键命令行工具输入：

git remote add origin [https://github.com/XXXXXX/xxxxx.git](https://link.zhihu.com/?target=https%3A//github.com/tugenhua0707/testgit.git) 这里是你的仓库即项目地址：

## 把项目推送到远程仓库：

同样使用在根目录下的命令行工具输入：git add .(点为全部的意思) 把项目所有文件加到缓存区

输入：git commit -m '这里为注释，随便写' 把缓存区里的文件提交到本地仓库

输入：git pull --rebase origin master 把远程仓库和本地仓库同步 成功后可以看到项目文件夹多了一个远程仓库中的README.md

最后输入：git push -u origin master 把仓库中的文件推送到github仓库

到此项目已经成功推送到远程仓库，小伙伴们只要得到链接就能下载该项目了。

我们进入github 进入我们之前创建的仓库 刷新发现仓库中已经有了项目代码。

