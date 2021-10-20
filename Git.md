# Shell
MPAGS: https://cpp-pg-mpags.github.io/shell-novice/

^ means ctrl, control
```bash
mkdir -p 
```

# Git
MPAGS git: https://warwick.ac.uk/fac/sci/physics/research/epp/resources/teaching/software_development_2021/day_1/versioncontrolwithgit.pdf

初始化一个Git仓库： git init
添加文件到Git仓库：
1.$ git add <file>, 可以反复多次使用，添加多个文件 把提交的所有修改放到暂存区(stage)
2.$ git commit -m <message>.  把修改提交到分支
查看工作区的状态 git status
查看修改内容 git diff
查看提交历史 git log 简化输出历史：git log --pretty=oneline
HEAD 指向的是当前版本 去往不同版本： git reset --hard commit_id
退回上一个版本 git reset --hard HEAD^
退回前，查看提交历史$ git log
重返未来版本 查看历史$ git reflog
丢弃工作区的修改1. git restore <file>  or2. git checkout --file
丢弃暂存区的徐改1/git reset HEAD <file> or2. git restore --staged
use "git restore <file>..." to discard changes in working directory
use "git restore --staged <file>..." to unstage)
git chechkout [branch] 进行分支的切换
git checkout -- [file] 将本地工作区的内容和当前最新版本库保持同步
git config --global user.name "Your Name"
git add . #track all files
git branch <new branch name>
git branch #check where you are
git checkout <branch name> #switch to another branch
git merge <branch name>

git remote add origin git@github.com:YutongLee2333/learngit.git
git branch -M main
git push -u origin main
$ ssh-keygen -t ed25519 -C "your_email@example.com"

git congit --global -l

git status
git add
git commit -m
git restore
git restore --staged
git reset --hard HEAD^
git reset --hard commit_id
git log --pretty=oneline
git checkout [branch]
git checkout -- [file]

### 合并策略
git merge 快进合并和非快进合并
fast-forward 快进合并

git merge --ff-only 快进合并
git merge --no-ff 非快进普通合并
git merge --rebase 变基合并　
git config pull.rebase false #合并
git config pull.rebase true #变基 git pull == git pull --rebase

git fetch

### git push --rebase
多人基于同一个远程分支开发的时候，如果想要顺利 push 又不自动生成 merge commit，建议在每次提交ß都按照如下顺序操作：
把本地发生改动的文件贮藏一下
$ git stash
把远程最新的 commit 以变基的方式同步到本地
$ git pull --rebase
把本地的 commit 推送到远程
$ git push
把本地贮藏的文件弹出，继续修改
$ git stash pop

### 2. git tag
```bash 
git tag
git tag -a v0.1.0 -m "mpags 0.1.0 ohter comment"
git show v0.1.0 
```
### 3. Sharing changes between Repositories
```bash
git remote -v
ssh-keygen -t ed25519
#Adding the Public SSH Key Part to Github
cat ~/.ssh/id_ed25519.pub (copy it to https://github.com/settings/keys)
#Changing the remote URL
#The URL you need can be found by just replacing the ‘https://github.com/’ part to ‘git@github.com:’, e.g. https://github.com/MPAGS-CPP-2021/mpags-day-1.git → git@github.com:MPAGS-CPP-2021/mpags-day-1.gi
git remote set-url origin <remote-url>
#pushing your repository to github
git push
```

# Let python organised
MPAGS python: https://mpags-python.github.io/
https://mpags-python.github.io/assets/slides/2021/Python-3.pdf
git clone https:---
git push