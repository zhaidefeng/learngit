## Git 指令

* git init：把目录编程Git可以管理的仓库
* git add readme.txt：把文件放到暂存区，也可以多次添加
* git commit -m "message"：把文件提交到仓库
* git log：查看历史记录
* git reflog：查看每一次的命令
* git status：查看状态
* git reset --hard 1094a：版本回退到1094a
* git reset --hard HEAD^：版本回退到上一个版本
* git checkout -- readme.txt：丢弃工作区的修改，让文件回到最近一次git commit或git add时的状态
* git rm：删除一个文件

#### 远程仓库

* ssh-keygen -t rsa -C "youremail&example.com"：创建SSH Key
* git push -u origin master：把本地库的所有内容推送到远程库上，并关联起来，此后每次本地提交后，只要有必要既可以使用命令git push origin master推送最近修改

* git clone git@github.com:zhaidefeng/gitskills.git：克隆一个本地库

#### 分支管理

* git checkout -b dev：创建dev分支，-b参数表示创建并切换
  * 相当于这两条命令：git branch dev、git checkout dev
* git branch：查看当前分支
* git merge dev：切换回master分支（git checkout master）后，把dev分支的工作成果合并到master分支上
* git branch -d dev：删除dev分支