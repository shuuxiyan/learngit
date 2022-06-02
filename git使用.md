# git使用

---

参考网站：[Git教程-廖雪峰的官方网站](https://www.liaoxuefeng.com/wiki/896043488029600)

---
## 一、如何把一个文件放入git仓库
首先找到你使用git init命令创建仓库的目录。  
把文件放到此目录下。  
1、使用git add [文件名] 把文件添加到仓库。
2、使用git commit -m "info" 把文件提交到仓库。

		初始化一个Git仓库，使用git init命令。

		添加文件到Git仓库，分两步：

		使用命令git add <file>，注意，可反复多次使用，添加多个文件；
		使用命令git commit -m <message>，完成。

## 二、推送远程库
要关联一个远程库，使用命令git remote add origin git@server-name:path/repo-name.git；

关联一个远程库时必须给远程库指定一个名字，origin是默认习惯命名；

关联后，使用命令git push -u origin master第一次推送master分支的所有内容；

此后，每次本地提交后，只要有必要，就可以使用命令git push origin master推送最新修改；

分布式版本系统的最大好处之一是在本地工作完全不需要考虑远程库的存在，也就是有没有联网都可以正常工作，而SVN在没有联网的时候是拒绝干活的！当有网络的时候，再把本地提交推送一下就完成了同步，真是太方便了！