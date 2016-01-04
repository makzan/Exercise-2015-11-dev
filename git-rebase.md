# Git Rebase

##Description

The git rebase can allows you to modify commits to updated upstream head. You can also reorder, edit, or squash commits together.

##Example

example 1:
Assume the following history exists and the current branch is "topic":

          A---B---C topic
         /
    D---E---F---G master
From this point, the result of either of the following commands:

git rebase master
git rebase master topic
would be:

                  A'--B'--C' topic
                 /
    D---E---F---G master

##Notes:
If the upstream branch already contains a change you have made, then that commit will be skipped. For example, running git rebase master on the following history (in which A' and A introduce the same set of changes, but have different committer information):

          A---B---C topic
         /
    D---E---A'---F master
will result in:

                   B'---C' topic
                  /
    D---E---A'---F master

If you want to pretend that you forked the topic branch from the latter branch, using rebase --onto.

For example, a feature developed in topic depends on some functionality which is found in next.

    o---o---o---o---o  master
         \
          o---o---o---o---o  next
                           \
                            o---o---o  topic
We want to make topic forked from branch master; for example, because the functionality on which topic depends was merged into the more stable master branch. We want our tree to look like this:

    o---o---o---o---o  master
        |            \
        |             o'--o'--o'  topic
         \
          o---o---o---o---o  next
We can get this using the following command:

git rebase --onto master next topic


##Rerference
[Git Reference](http://git-scm.com/docs/git-rebase)
[Github](https://help.github.com/articles/about-git-rebase/)