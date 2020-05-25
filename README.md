# git-prac
create local repo -
- git clone -b branch url folder-name
- git add 1.txt
- git commit -m "firstCommit"
- git remote -v
- git push origin branch
 
create local repo -
- create maven project using intellij
- git init
- git add pom.xml
- git commit -m "first commit"
- git checkout develop
- git remote add origin https://github.intuit.com/rkandpal/testRepo2.git
- git push origin develop
  
sync local repo from remote repo -
- git fetch --all
- git checkout master
- git pull origin / git merge
  
Reset modified files -
- git checkout -- RealtimeProfileEntityIngestionProcessor.java

create new branch -
- git branch iss53
- git checkout iss53
- git push origin iss53    <this is generic command to push changes to a branch>
- git branch
  
check commit Log -
- git log
- git log -1
- git log --oneline
  
git commit/stage all files before switching branch -
- git checkout iss53
- create new file or modify file
- git stash
- git checkout master
//do work on master
- git checkout iss53
- git stash pop <this will show all the files> 
 
Git checkout is an easy way to “load” any of these saved snapshots onto your development machine.
-git checkout <commit-id>
  
Revert any changes -
-git revert <commit-id>
 
Diff command -
- git diff <commit-id> <commit-id>
- git diff <commit-id> <commit-id> <file-name>
- git diff Head .
 
Merge feature-branch into master
- git checkout master
- git merge <feature-branch>
- git add .
- git commit
- git push origin master

https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf
