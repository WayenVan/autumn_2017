
# 第一次学习报告
***
## Git篇
### Git初步使用
* 申请github账号:[WayenVan](https://github.com/WayenVan)

* 基于windows安装git（使用gitbash）设置个人信息
```
      $ git config --global user.email "544972781@qq.com"
      $ git config --global user.name  "WayenVan"
```
  使用`mkdir`创建一个目录(与Linux bash相同)然后使用如下代码初始化git仓库：

      $ git init

### Git本地操作
* 添加操作到暂存区与提交操作：
使用`git add filename`将文件操作提交到暂存区，再使用`git commit -m "name"`操作将文件修改提交到现在分支，例如：
```
      $ git add file //提交
      $ git commit -m (add one file) //跟新库文件
```
  同时我们还可以使用`git status`命令追踪现阶段暂存区的内容和工作区的内容

* 文件的新建，恢复与删除：
文件恢复到上一次提交或者版本确认：
```
      $ git checkout --file //修复文件
```
  文件删除：可以直接在文件管理器中删除后，使用指令`git rm filename`删除后提交

* 版本管理，使用`git log`得到之前任意版本号，再使用`git reset ID`还原到过去版本:
```
      $ git reset ID //还原仓库到ID版本
```
* 分支管理：使用`git checkout -b BranchID` 命令创建并切换到新分支
```
      $ git checkout BranchID //切换到新分支
      $ git checkout -b BranchID //切换分支
      $ git branch //查看分支
      $ git merge // 分支合并
```
### Git远程操作
* 与github建立远程通信（应用ssh协议）：
```
      $ ssh-keygen -t rsa -C "544972781@qq.com" //获取远程ssh公共和私人key
```
  接着复制公共key到github网站。

* 远程仓库操作：
```
      $ git remote add name URL //建立远程链接
      $ git push name branch //推送本地仓库至云仓库
      $ git fetch name branch //获取远程仓库信息
      $ git remote -v //显示远程信息
```
  **远程仓库的更新**:
```
      $ git remote add originname URL //建立与原始仓库的链接
      $ git fetch originname //获得原始仓库所有分支，储存在originname/branch 当中
      $ git merge originname/branch //保持跟新
```      
>学习文档包括[廖雪峰的git](https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000),
[github的协作中文版](https://github.com/milLearningGroup/autumn_2017/issues/55)。


***
## Markdown篇
*markdown 真是一种好用的语言 （强行划水）
