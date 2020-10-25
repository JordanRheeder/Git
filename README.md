# Git tutorial

https://learngitbranching.js.org/

How to initialise a Git repository:
$ git init

*You must have git installed on your system.

How to create a new project do the following:
- Navigate through the terminal to your folders or use VSCode terminal then type: "git init" when you're inside the folder.
[url=https://postimg.cc/mPFxf4Cs][img]https://i.postimg.cc/mPFxf4Cs/Stages-of-git.png[/img][/url]
[Stages-of-git.png](https://postimg.cc/mPFxf4Cs)

How to check for changes in the git repo:
$ git status
*This will return all the files and folders that have been changed (usually in red)
*You can also type 'git diff <file name>' on the files name to get a output of changes on the file.

How to stage your work is by doing the following:

$ git add ./
$ git commit -m "insert useful message"
$ git push

Creating branches:
git checkout -b <branch name> 
i.e: git checkout -b <option WIP>WP|Ticket number/name|what you're working on

Check what branch you're on:
$ git branch

Best practice:

Pull master before you work on a new piece of code to avoid merge conflicts.
so do the following:

$ git branch
$ master
$ br-1* 

* *indicates that you're on that branch*

If you want to merge your branch to master, follow the below steps:

push your branch say 'br-1' to remote using *git push origin br-1*.
switch to master branch on your local repository using *git checkout master*.
update local master with remote master using *git pull origin master*.
merge br-1 into local master using *git merge br-1*. This may give you conflicts which need to be resolved and changes committed before moving further.
Once merge of br-1 to master on local is committed, push local master to remote master using *git push origin master*
*This will merge 'br-1' into master. If there are conflicts it will highlight it in your IDE.*

