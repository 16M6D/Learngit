# Git 

#### 安装

Linux

```
#Is git installed?
git
#Debian & Ubuntu Linux
sudo apt-get install git
```

Windows

​	Git官网下载->Git Bash->初始化

```
$ git config --global user.name "Your Name"
$ git config --global user.email "email@example.com"
```

### 创建版本库

### 时光机穿梭

#### 版本回退

```
#显示从最近到最远的提交日志
git log
#tips:press'q' to quit in VSCode
#简洁显示log
git log --pretty=oneline
```

#### 工作区和暂存区

Working Directory:在电脑里能看到的目录

Repository:

 ![git-repo](https://www.liaoxuefeng.com/files/attachments/919020037470528/0) 



#### 管理修改

 每次修改，如果不用`git add`到暂存区，那就不会加入到`commit`中。也就是最终的版本需要先add再commit.

#### 撤销修改

场景1：当你改乱了工作区某个文件的内容，想直接丢弃工作区的修改时，用命令`git checkout -- file`。

场景2：当你不但改乱了工作区某个文件的内容，还添加到了暂存区时，想丢弃修改，分两步，第一步用命令`git reset HEAD `，就回到了场景1，第二步按场景1操作。

场景3：已经提交了不合适的修改到版本库时，想要撤销本次提交，参考[版本回退](https://www.liaoxuefeng.com/wiki/896043488029600/897013573512192)一节，不过前提是没有推送到远程库。

#### 删除文件

`rm <file>`删除文件后此时工作区和版本库中不一致,若确实要从版本库中删除则使用 `git rm ``git commit ` ,若删错了,`git checkout -- test.txt`,即用版本库中的版本替换工作区中的版本.

### 远程仓库

### 分支管理

### 标签管理

