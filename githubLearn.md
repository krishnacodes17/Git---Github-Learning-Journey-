## Git 
- git & github  both are different 
- git is Version control, also known as source control, is tracking and managing software code changes.

 ## Dowload git
 - dowload git from his official website git.com

## Setting up Git Global Configuration
- git config --global user.name  "krishna"
   - its save your name globaliy
-  git config --global user.email  "krishnacodes17@gmail.com" 
    - its save your gmail gobaly

##  now how we do version controlling with git 
- mkdir git&Github 
    - its create a folder name with git&Github
- cd git&Github
    - its open git&Github folder
- code .
    - its open this folder git&Github in vsCode

 ***** now here we create a html file github.htm for learning *****

- git  init 
    - its initialize  git crrunt folder when we enter this command its means git will be enable and its track this folder and also we see in right side of folder (U) symbol means this file is untracked 
- install some extension for help learning 
    - git graph
- ls -la 
    when we enter this command in terminal its show github hidden folder  eg: .git/

- git add git.js 
   - when we git this command a perticular folder track started which name is given here we give java.js 
   - git add .    this command track all file (.) means all file 
   - git rm -f --cached git.css
    - its remove git.css file from track and keep in untrack stage

- git diff 
    - its show how many line add or how much line deleted

- git commit -m "this is our first commit"
    - it commit our file all changes with a message of "this is our first commit " 

- git log 
    - its show all commit with a commit id and its show all detail who is commited, what its massage , its email , name , day ,time etc

- git log --oneline
    - its show all commit is sigle sigle line with out more information only show commit is

**** NOTE : when we wand to coomit any file than first add that file track eg: git add git.js  than commit with a good and informative message  ****

- git show eebed65
    - its show all detail of this commit id eebed65 like what is changes in this commit what authore name , date etc

- git blame git.js 
    - its show all git.js file commits and authore info like name , date etc


- git reset --hard 3f2eee5
   - this command help to go particular  commite which commit id we mention in this command we mention 3f2eee5 this commit id 
    - when we go one step back that time our next step will be removed 
    eg: 123456  this is our commit and suppose i am go to 3 commit so his front 4 5 6 this commit will be remove 

- git revert 79037e3
    - its help to reverse our changes means what ever add its remove and which is deleted that all things add 
    
## Github  
 - githb is remote server where we push (keep) our code and any one can pull our code for work on same project 



### Now how to work with our Github and our Local git
 - git remote -v
    - this command help to check any github repositry connect or not
- git remote add origin (https://github.com/krishnacodes17/Git---Github-Learning-Journey-.git) 
    - its connect our github repositry to our local repositry

 
    - this command push our code on github 

- git push -u origin master
    - its push our code on github
- git pull
    - its pull our code from 
    
## Now  we learn ssh key 
   - create ssh key first open our git command line  >> open any folder inside our compute > click right burtton > show more option  >> click open git base here >> ssh-keygen -t rsa -b 4096 -C "your_email@example.com" >> now change our email >> press enter > enter > now copy our ssh key >> clip < ~/.ssh/id_ed25519.pub

    - open github click new ssh keys give title and paste coped ssh key  >>> done

## git branches 
 - git branche
    - to check branch 
- git branch "friend"
    - to create branch 
- git checkout "friend"
    - to switch branch
- git merge "friend"
    - to merge branch  Note: when we merge branch we are in main branch 

### how to keep our branch name meaningful 
 - wip > work in progress 
 - feat > feature 
 - bug > bug fix
 - junk > junk code
 - refactor > code refactoring
 - test > testing code

  eg : git branch feat/login
    eg : git branch bug/login

### for more understanding of branches and understand concept  you van wesite 
 - [link for branch understanding ](https://git-school.github.io/visualizing-git/)


## git stash 
- git stash save "name" 
    - its save our current work and remove from our local folder
- git stash list
    - its show all stash name
- git stash apply "name"
    - its apply our stash name
- git stash pop "name"      
    - its apply our stash name and remove from stash list
- git stash clear
    - its clear our stash list