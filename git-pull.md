git-pull

DESCRIPTION
git-pull = git fetch + git merge
Fetch from and integrate with another repository or a local branch

$ git pull <remote>
eg : git pull https://github.com/makzan/Exercise-2015-11-dev.git

=========================================================================
A---B---C master on origin
	 /
    D---E---F---G master
	^
	origin/master in your repository

=========================================================================

A---B---C origin/master
	 /         \
    D---E---F---G---H master

SYNOPSIS

git pull [options] [<repository> [<refspec>…?]]

More introduction, please visit https://git-scm.com/docs/git-pull