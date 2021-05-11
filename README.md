# Git 学习

## Git构成

1. remote repository：远程仓库
2. local repository：版本库或本地仓库，工作区有一个隐藏目录 .git，这个不算工作区，而是 Git 的版本库
3. staging area：暂存区/缓存区，一般存放在 .git 目录下的 index 文件（.git/index）中，所以我们把暂存区有时也叫作索引（index），只存储最近的一次内容，不保留所有历史版本
4. workspace：工作区，电脑里能看到的目录文件

## Git常用命令

### Git使用前提

1. 安装git软件
2. Git初始化：git init
3. 从remote repository远程仓库克隆至工作区和本地仓库：git clone repository(后缀为.git)----是否同步至暂存区？
4. 从远程库直接到工作区：git pull----git pull和git clone的区别？

### 对代码的操作

1. 如果工作区代码有调整，需要先将内容同步至暂存区/缓存区，只有先提交到暂存区/缓存区，才能提交到本地仓库：git add
2. 将代码调整提交到本地仓库：git commit
3. 从暂存区/缓存区获取最新版本：git reset----如果暂存区/缓存区没有提交到本地仓库，则从暂存区/缓存区获取的最新版本与本地仓库获取的版本不一致
4. add但是不commit，之后再reset会怎样？-依然可以获取到最新的版本
5. 查看历史提交记录：git log
6. 从远程获取代码库：git fetch-----fetch和clone的区别？
7. 从本地仓库提交至远程仓库：git push