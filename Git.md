# Shell
MPAGS: https://cpp-pg-mpags.github.io/shell-novice/

^ means ctrl, control
```bash
mkdir -p 
```

# Git
MPAGS git: https://warwick.ac.uk/fac/sci/physics/research/epp/resources/teaching/software_development_2021/day_1/versioncontrolwithgit.pdf


git congit --global -l

git status
git add
git commit

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
