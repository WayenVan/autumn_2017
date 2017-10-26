# 第一次学习报告
***
## Git篇
### Git初步使用
* 申请github账号:[WayenVan](https://github.com/WayenVan)

* 基于windows安装git（使用gitbash）设置个人信息
        $ git config --global user.email "544972781@qq.com"
        $ git config --global user.name  "WayenVan"
  使用`mkdir`创建一个目录(与Linux bash相同)然后使用如下代码初始化git仓库：
        $ git init

### Git本地操作
* 添加操作到暂存区与提交操作：
使用`git add filename`将文件操作提交到暂存区，再使用`git commit -m "name"`操作将文件修改提交到现在分支，例如：
        $ git add file
        $ git commit -m (add one file)
同时我们还可以使用`git status`命令追踪现阶段暂存区的内容和工作区的内容

* 文件的新建，恢复与删除：
文件恢复到上一次提交或者版本确认：
        $ git checkout --file
文件删除：可以直接在文件管理器中删除后，使用指令`git rm filename`删除后提交

* 版本管理，使用`git log`得到之前任意版本号，再使用`git reset ID`还原到过去版本
