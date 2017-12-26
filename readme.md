# git的一些基本指令

### git
##### 配置
* git config --global user.name "Your Name"
* git config --global user.email "email@example.com"

* git init
* Initialized empty Git repository in /Users/michael/learngit/.git/

##### 提交事务
上传
* git add readme.md
删除git仓库某文件,需要git commit确定
* git rm readme.md
提交
* git commit -m 'some explain'
查看状态
* git status
查看文件何处被修改
* git diff readmd.md


##### 撤销事务
撤销提交
* git checkout -- readme.md
或者
* git reset HEAD readme.md

##### 查看日志
查看所有日志
* git log
查看所有命令记录
* git reflog
退回到某个版本
* git reset --hard commitid


### 与github连接
先在github创建仓库
然后cd到项目文件
* git remote add origin git@github.com:michaelliao/learngit.git
* git push -u origin master

##### 从github克隆仓库
* git clone git@github.com:michaelliao/gitskills.git
