# Understand Git commands

Use Git commands to synchronize content between your local branch and a remote repository.

- `git fetch`
- `git pull`
- `git merge`
- `git push`

## About git fetch

Use the `git fetch` command to add content from a remote repository to your local working branch. Use this command if you want to see the commits that are on the remote branch before you commit them to your local branch. The command doesn't commit content to your local branch. 

To merge content to your local branch, use `git pull` followed by `git merge`.

## About git pull

Use the `git pull` to both fetch commits from a remote branch and merge them into a local branch. Use this command if you do not need first to verify the commits on the remote branch.

Use this command on a regular basis to make sure your local branch is up to date. 

## About git merge

Use the `git merge` command to merge content from a remote branch to your local branch. Specify the names of both the remote and local branches:

`git push <remote-name> <local-name>`

To make sure both branches are synchronized before performing a `git merge`, use the `git status` command.

## About git push

Use the `git push` command to send new or updated content that is stored locally to a remote repository. 

The command first verifies whether there is a remote branch. If a remote branch exists, `git push` sends the content to it. Both your local branch and the remote branch are then synchronized.

If commits in the remote branch are missing from your local branch, the command  recognizes that the branches diverged, and the command fails.

To synchronize both branches before using the `git push` command, first use the `git pull` command.

