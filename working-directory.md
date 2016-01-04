# Working Directory

## git status

#### Description
As you make any change, you will be changing the contents of the working directory. You can check the status of those changes with:
git status

#### Examples
From the terminal, check the status of the your project:
* git status
* git status --short

In the output, notice the file in red under untracked files. Untracked means that Git sees the file but has not started tracking changes yet.

#### Reference
[ProGit](https://git-scm.com/docs/git-status)


## git add

#### Description
In order for Git to start tracking any file changed, the file needs to be added to the staging area.

#### Examples
We can add a file to the staging area with:
* git add readme.txt
We can add all files to the staging area with:
* git add .

After add any file to the staging area, check the status of the project in Git.
In the output, notice that Git indicates the changes to be committed with "new file: readme.txt" in green text. Here Git tells us the file was added to the staging area.

#### Reference
[ProGit](https://git-scm.com/docs/git-add)

## git diff

#### Description
We can check the differences between the working directory and the staging area

#### Examples
Imagine that we type another line in readme.txt. Since the file is tracked, we can check the differences between the working directory and the staging area with:
* git diff readme.txt

From the terminal, use the new command to check the difference between the working directory and the staging area.
IMPORTANT: press q on your keyboard to exit diff mode.

Add the changes to the staging area in Git. Recall that you will need to identify the file by its name.

#### Reference
[ProGit](https://git-scm.com/docs/git-diff)

## git commit

#### Description
A commit is the last step in our Git workflow. A commit permanently stores changes from the staging area inside the repository.

#### Examples
git commit is the command we'll do next. However, one more bit of code is needed for a commit: the option -m followed by a message. Here's an example:
git commit -m "Complete first line of readme.txt"

After commit all changes, check the status of the project in Git. From the terminal, nothing to commit.

#### Reference
[ProGit](https://git-scm.com/docs/git-commit)