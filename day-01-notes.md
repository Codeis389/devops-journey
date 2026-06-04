#Day 1 - Devops Learning 

## What is Devops

- Devops = Development + Operations + Automation
- Makes code go from developer laptop to user automatically
- Like a factory conveyor belt for software.

## What I Built Today
- HTML/CSS/JS site deployed with CI/CD pipeline
- Every git push = site updates automatically
- My live site: https://codeis389.github.io/my-devops-site/

## Commands I Learned

## Git Setup

git config --global user.name "Your Name"
git config --global user.email "email@gmail.com"
git config --list

### Git Daily Commands
git init           =  Start git in folder
git add .          =  add all files
git status         =  check what changed
git commit -m ""   = save changes
git push           =  send to github
git remote -v      = check remote URL
git remote remove  =  remove wrong remote  


### Linux Commands Used
cd ~                =  go to home floder
mkdir foldername    =  create folder
touch filename      =  create file
nano filename       =  edit file
cat filename        =  view file content
ls -la              =  list all files
pwd                 =  show current location


## Eror I Faced and Fixed
Problme: typed "orgin" instead of "origin"
Fix:     git remote remove orgin
         git remote add origin correct-url

### Error 2 - Wrong token
Problem:   Used account password instead of token
Fix:       create token at github.com/settings/tokens
           need repo + workflow permissions checked

### Error 3 - Depreacated action versions
Problem:     Upload-pages-artifact v3 was deprecated
Fix:         updated yml to latest versions
             checkout@v4, configure-pages@v5
             upload-pages-artifact@v3, deploy-pages@v4

### Error 4 - Chrome package error
Problem:    google-chrome-stable needed reinstall
Fix:        sudo dpkg --remove --force-remove-reinstreq google-chrome-stable
            sudo apt --fix-broken install

## CI/CD Pipeline I Created
- PUsh code to GitHub Actions triggers automatically
- Pipeline tests and deploys site
- Zero manual work needed!

## What is CI/CD
CI  =  Continuous Integration  =  auto test code
CD  =  Continuous Deployment   =  auto deploy code
