# TIL 22-04-03
---
* git restore fileName
    - it simply for undoing operation would do the trick and get changes back
* git restore --staged fileName 
    - makes the file go back to Unstaged Area (when it is in Staging Area)

> restore was 'checkout' in old version 

---

* git revert CommitHash
    - reverting undoes a commit by creating a new commit.
    - it means 'revert' create a new commit that introduces the changes form the specified commit
    - it doesn't mess up team member's commit history or remote storage
    - it can be 'safe reset' not to make any troble from commit history


---

* git reset CommitHash
    - reset is based on going back to 'commit hash'
    - plain commit doesn't delete log or change other commits when you go back
    - it is just going back to Working Directory(Unstaged Area) from Repository
    - it needs when you want to remove commits in a private branch or throw away uncommitted changes

* git reset --hard CommitHash 
    - it goes back to your commit that you want to reset and removes all things that you did between commits you set
    - the staged snapshot and Working Directory are both updated to match the specified commit
    - it can help to set clear commit history in local, but can easily makes conflict between local and remote storage

---

* git rebase branchName
    - it literally means 're-base' to combine other commits that you made in the branch before you merge with the other branch
    - sometimes it can be harmful or dangeous to do it in shared branches since it rewrites the commit history 


---