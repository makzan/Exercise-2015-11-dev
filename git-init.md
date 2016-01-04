# Git init

git init marks the current directory as a git-tracked repository.

## Example command

~~~
git init
~~~

This creates a `.git` folder in the current directory. And from now on, you can use all the git command in this directory.

## Notes and Tips

1. Calling `git init` on a git-tracking directory has no effects.
    > Running git init in an existing repository is safe. It will not overwrite things that are already there. The primary reason for rerunning git init is to pick up newly added templates (or to move the repository to another place if --separate-git-dir is given).
    [git-init doc](https://www.kernel.org/pub/software/scm/git/docs/git-init.html)
2. Running `git init --bare` means creating a remote git repository.
3. Usually we name the director of bare repo `something.git`, with the `.git` extension althrough it is a directory.

## Further reading

- [Git add documentation](https://www.kernel.org/pub/software/scm/git/docs/git-init.html)
- [Tutorial on git init bare](https://www.atlassian.com/git/tutorials/setting-up-a-repository/git-init)

