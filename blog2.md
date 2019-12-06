# 5-12-2019
## Today I learnt GIT and Bash commands
1. GIT 
<br> 
I learnt basic commands like GIT pull, GIT add, GIT commit
<br>
  1. git config <br>
  Utility : To set your user name and email in the main configuration file.
  <br>
    2. git init 
    <br>
    Utility : To initialise a git repository for a new or existing project.
    How to : git init in the root of your project directory.

    3. git clone 
   
    Utility : To copy a git repository from remote source, also sets the remote to original source so that you can pull again.
  
    How to : git clone <:clone git url:>

    4. git status

    Utility : To check the status of files you’ve changed in your working directory, i.e, what all has changed since your last commit.
  
    How to : git status in your working directory. lists out all the files that have been changed.

    5. git add 
  
    Utility : adds changes to stage/index in your working directory. 
    
    How to : git add .

    6. git commit
  
    Utility : commits your changes and sets it to new commit object for your remote.
   
    How to : git commit -m”sweet little commit message”

    7. git push/git pull 
   
    Utility : Push or Pull your changes to remote. If you have added and committed your changes and you want to push them. Or if your remote has updated and you want those latest changes.
   
    How to : git pull <:remote:> <:branch:> and git push <:remote:> <:branch:>

    8. git branch 
   
    Utility : Lists out all the branches. 
   
    How to : git branch or git branch -a to list all the remote branches as well.
    
    2. SHELL PROGRAMMING
    Some sample programs-
    
    #!/bin/sh
    echo "what is your name?"
    read name
    echo "How do you do, $name?"
    read remark
    echo "I am $remark too!"
    
    for more read
[shell programs](https://www.learnshell.org/)
