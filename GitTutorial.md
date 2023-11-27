1. repository actions
    1. create repository
        1. open a new local repository: git init
        2. clone a repository: git clone url
        3. push a repository to github: git push origin master
    2. update:
        1. a cloned repository: git fetch url
        2. a remote repository: git pull url
    3. delete:
        1. only git tracker: git rm -r .git
        2. whole repository: 
            1. git rm -r .
            2. rm -rf .git
        3. what is -r, -rf: recursively, recursive force

2. how prevent git to change line feed(lf) to carriage return lf(crlf)
    1. git config --global core.autocrlf false

3. tracking file
    1. how add a file to git tracker:
        1. add all files: git add -A
        2. add a specific file or folder: git add name
    2. remove a file from git tracker: 
        1. a file: git rm --cached -f name
        2. a directory: git rm --cached -f directory/*


4. commiting
    1. commit a staged file
        1. with message: git commit -m "message"
        2. without message: git commit --allow-emmpty-message
    2. back to past
        1. back on specific commit: git checkput commit-hash
        2. back to previous commit: git checkout HEAD~1
        3. back to previous of first commit: rm -rf .git
    3. remove a file from 
        1. git repostiry: git rm -f name
        2. system drive to: git rm -rf name
        

5. set user identify for git
    1. git config --global user.name "name"
    2. git config --global user.email "email"

6. .gitignore
    1. add a file or directory: name, name/
    2. add a extension: *.txt
    3. exclude a file from be ignored: !directory/*.js

7. see properties
    1. stage of files: git status
    2. commit properties: git log
        1. close git log pager: q
        2. in one line format: git log --pretty=oneline
        3. in graph format: git log --graph
