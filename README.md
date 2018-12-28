# Git学习笔记
### Git配置
#### 配置git用户邮箱
```bash
$ git config --global user.email "<Your_Email>"
```
#### 配置git用户名
```bash
$ git config --global user.name "<Your_Name>"
```

### Git基本命令
#### 初始化一个Git仓库
```bash
$ git init
```
#### 注册需要提交的文件
```bash
$ git add <Your_File>
```
#### 注册所有文件
```bash
$ git add --all
```
#### 创建提交
```bash
$ git commit --message "<Your_Message>"
```
#### 查看工作区状态
```bash
$ git status
```
#### 查看版本文件的差异
```bash
$ git diff <Your_FILE>
```
#### 查看当前版本与版本库中HEAD提交与暂存区的不同
```bash
$ git diff --staged
```
#### 删除不需要的文件
```bash
$ git rm <Your_FILE>
```
#### 查看项目提交历史
```bash
$ git log
```
#### 查看项目提交历史且显示成一行
```bash
$ git log --oneline
```
#### 查看项目提交历史且显示成图状
```bash
$ git log --graph
```
#### 查看项目提交历史且限制输出次数为3
```bash
$ git log --n 3
```
#### 查看项目提交历史且显示细节信息
```bash
$ git log --format
```
#### 查看命令历史
```bash
$ git reflog
```
#### 版本回退
```bash
$ git reset --hard HEAD^
```
#### 克隆项目
```bash
$ git clone <Your_Path>
```
#### 从原版本库中取回新的提交
```bash
$ git pull
```
#### 查看版本库的完整性
```bash
$ git fsck
```
#### 丢弃工作区的修改
```bash
$ git checkout -- <file>
```
### 查看命令历史
```bash
$ git reflog
```
### 版本回退
```bash
$ git reset --hard HEAD^
```
### 回退指定版本号
```bash
$ git reset --hard <Your_Commit_Id>
```
#### 将工作区和暂存区中的修改保存在存储栈中
```bash
$ git stash
```
#### 检查存储栈修改的内容
```bash
$ git stash list
```
#### 新建一个标签
```bash
$ git tag <Your_Tag_Name>
```
#### 查看所有标签
```bash
$ git tag
```

### 远程仓库
#### 创建SSH Key
```bash
$ ssh-keygen -t rsa -C "<Your_Email>"
```
#### 关联远程仓库
```bash
$ git remote add origin <Your_Repository_Path>
```
#### 推送到远程仓库
```bash
$ git push -u origin master
```


### 分支
#### 创建分支
```bash
$ git branch <Your_Branch_Name>
```
#### 查看当前的活跃分支
```bash
$ git branch
```
#### 切换分支
```bash
$ git checkout <Your_Branch_Name>
```
#### 合并某分支到当前分支
```bash
$ git merge <Your_Branch_Name>
```
#### 快进合并且产生一次提交
```bash
$ git merge --no-ff <Your_Branch_Name>
```
#### 分支变基
```bash
$ git rebase master
```
#### 从版本库获取提交
```bash
$ git fetch <Your_Clone_Name>
```
#### 查看远程库信息
```bash
$ git remote -v
```
#### 从本地推送分支
```bash
$ git push origin <Your_branch_Name>
```

### 子模块
#### 纳入子模块
```bash
$ git add submodule add <Your_Sub_Name> sub
```
#### 注册子模块
```bash
$ git submodule init
```
#### 选择子模块版本
```bash
$ git checkout v1.0
```
