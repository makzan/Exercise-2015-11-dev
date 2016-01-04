# Git Rebase

Description

The git rebase can allows you to modify commits to updated upstream head. You can also reorder, edit, or squash commits together.

Example

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

example 2:
If the upstream branch already contains a change you have made, then that commit will be skipped. For example, running git rebase master on the following history (in which A' and A introduce the same set of changes, but have different committer information):

          A---B---C topic
         /
    D---E---A'---F master
will result in:

                   B'---C' topic
                  /
    D---E---A'---F master




--Any notes when using the commands, such as:
	Related commands that often use together.
	Tips & tricks when using this command.
	Things to be aware when using the command.
--Special examples if any.