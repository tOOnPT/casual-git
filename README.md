# casual-git

## How to install
1. `git clone https://github.com/x0st/casual-git`
2. `make`
3. Use `gh` within git repositories to open casual-git

## Docs
```
  d  - push
  f  - force push
  p  - pull
  o  - force pull
  c  - commit
  a  - amend commit
  s  - smart commit
  l  - pretty log
  h  - smart checkout
```

### d
`git push origin {current_branch}`

### f
`git push origin {current_branch} --force`

### p
`git pull origin {current_branch}`

### o
```
git pull origin {current_branch}
git reset --hard "origin/{current_branch}"
```

### c
You will be asked about a message.

`git commit -m "{message}"`

### a
`git commit --amend --no-edit`

### s
```
  d  - push
  f  - force push
  p  - pull
  o  - force pull
  c  - commit
  a  - amend commit
  s  - smart commit
  l  - pretty log
  h  - smart checkout
  
  Delete files from the next commit: 
  [-1] new file: test1
  
  Add files to the next commit: 
  [1] modified:  gulpfile.js
  [2] modified:  package.json
  [3] untracked: test
  
  Enter file numbers separating by spaces: -1 2 3
  
  Enter a comment: my commit
```

### l
```
git log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit
```

### h
```
  
  d  - push
  f  - force push
  p  - pull
  o  - force pull
  c  - commit
  a  - amend commit
  s  - smart commit
  l  - pretty log
  h  - smart checkout
  
  Enter a branch name or a part of name: ma
  
  More than one git branch were found. 
  10 first branches are shown. 
  Please choose a desired branch. 
  
  [0] feature/EGNYTE-20-watermarks-over-documents
  [1] master
  [2] masterfix/EGNYTE-21-big-files-merge
  [3] masterfix/EGNYTE-26
  [4] masterfix/EGNYTE-29-big-files-merge
  [5] masterfix/EGNYTE-33
  [6] masterfix/EGNYTE-41
  
Switched to branch 'feature/EGNYTE-20-watermarks-over-documents'
```
