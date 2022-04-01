# TIL 22-04-01
---
## git merge and branches

    $ git branch
Show available All branch

    $ git branch -r
Show available remote branch

    $ git branch -a
Show available all branch

    $ git branch branchName
Create new branch

    $ git checkout branchName
Change branch to branchName from current branch

    $ git checkout -b branchName
Create new brnach and then change to the branch

    $ git merge branchToMerge    
merge branchTomerge with current branch

---
__merge has 3 types technically__ 
  1. normal merge
       - It is basic type to merge branches
       - Fast-Forward(ff), 3-way-merge(non ff)
       - merge has options to pick ff and non ff way
  
  2. rebase and merge
       - can be simple commit
       - project can keep simple state  

  3. squash and merge
       - merge branch after combining commits
       - can set number of commits that you want before merge

* Check git log, state of branches, remote, files before merge branches

    git branch-r, git branch -a, remote --v, log --branches --graph, git diff, cat

* Also can use 'format-patch', 'checkout --patch' and '--patch' to edit texts into files that you want to change detail
---

    $ git branch -D branchName
delete branch

    $ git push remoteStorageName localBranchName
push branch to save data to remote storage 

    $ git diff branchA branchB
see the difference between two branches
