git-fetch

DESCRIPTION

1. Fetching and Pulling from Your Remotes
$ git fetch [remote-name]
eg : git fetch https://github.com/makzan/Exercise-2015-11-dev.git
The command is to download all objects and references from the remote server to the local. And it will automatically create a repository that names 'orgin'.

2. Adding Remote Repositories
$ git remote add [shortname] [url]
$ git fetch [shortname]
eg : git remote add github https://github.com/makzan/Exercise-2015-11-dev.git
      git fetch github
After this operation, you can use the string 'github' on the command line in lieu of the whole URL.

SYNOPSIS

git fetch [<options>] [<repository> [<refspec>¡K]]
git fetch [<options>] <group>
git fetch --multiple [<options>] [(<repository> | <group>)¡K]
git fetch --all [<options>]

More introduction, please visit https://git-scm.com/docs/git-fetch







