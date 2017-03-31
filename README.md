# git-tug

`git-tug` is a simple git plugin that provides a simple command to pull all local branches tracking a remote branch.

## How it works

1. Stashes any local changes (including untracked files), if any.
2. Iterates through all local branches with a defined `upstream` branch.
3. If the local branch is behind, perform a `pull --rebase`
4. Restore any changes stashed in 1) 

## Usage

Put the `git-tug` script somewhere in your PATH and simply run `git tug` in a git repository.
