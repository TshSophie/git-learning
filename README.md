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

***注意使用git commit提交前要先git add一下，把文件往Git版本库里添加的时候，是分两步执行的：
第一步是用git add把文件添加进去，实际上就是把文件修改添加到暂存区；
第二步是用git commit提交更改，实际上就是把暂存区的所有内容提交到当前分支。
***

> 使用`git status`查看结果

~~~
git status 
~~~

> 使用`git diff <file>`列出文件具体修改的内容

~~~
git diff
~~~

### 版本回退

> 使用`git log`查看提交日志

~~~
$ git log
~~~

上面会列出提交的ID、提交人、邮箱以及提交日期

***加--pretty=oneline参数简化查看提交的日志
这时只会把提交ID和提交的说明列出来
***

> 使用`git reset --hard HEAD^`回退到上一个提交版本

首先，Git必须知道当前版本是哪个版本，在Git中，用HEAD表示当前版本，也就是最新的提交3628164...882e1e0（注意我的提交ID和你的肯定不一样），上一个版本就是HEAD^，上上一个版本就是HEAD^^，当然往上100个版本写100个^比较容易数不过来，所以写成HEAD~100。

> 使用`git reset --hard 提交ID`回到这个提交ID所对应的版本

>使用`git reflog`查看每一次命令以及对应版本号

~~~
$ git reflog
~~~












