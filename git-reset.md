# Git Reset

This is a short introduction of Git Reset:
It can reset the current HEAD to specified state
It has 3 modes: soft, mixed, and hard
If you not provide any parameter the mode mixed is by default.

Git Reset is different from Git Checkout which will move from one branch to another.
The file stages in Repo, Staged, Working dir having been taken effect 
according to 3 modes of #RESET : soft, mixed, hard

# Example
$ git reset <file>
It will reset the Repo as last commit, but in staged area and working dir it reamins unchange

$ git reset --soft 
All the files will go back to last commit even in staged area

$ git reset --hard HEAD~2
it will go back to last 2 commit, even ##IN Working copy

## Notes
Be careful to use --hard mode: 
#ANY non-committed content in Working copy will be overridded!!

##Reference
[ProGit - Reset](http://git-scm.com/2011/07/11/reset.html)