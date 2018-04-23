##git 使用教程

### 创建版本库

> 创建一个文件目录用来放git库

~~~
$ mkdir learngit  #表示在当前目录下创建一个名为learngit的文件夹
$ cd learngit     #进入该目录
$ pwd 			  #显示当前目录
/Users/michael/learngit   
~~~

> 通过`git init`命令初始化该目录为git仓库

~~~
$ git init
~~~

> `git add <file>` 将文件放到git仓库

~~~
$ git add readme.txt
~~~

> `git commit`将文件提交到仓库并给出提交说明

~~~
$ git commit readme.txt -m "项目说明文档"
~~~

**-m 后面的为提交说明**

> 使用`git status`查看结果

~~~
git status 
~~~

> 使用`git diff <file>`列出文件具体修改的内容

~~~
git diff
~~~

### 版本回退

> 使用`git reset --hard HEAD^`回退到上一个提交版本










