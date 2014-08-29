# git-branchmeta

> Alpha
> Pull out the `[branch]` description from your `.git/config`
> Quickly edit and view your branches, with annotations
> Hashtag branches for easier management
> Same format as gitconfig so you can still use `git branch --edit-description` (TODO - compatibility with .gitbranch file)

## Install

Put `git-branchmeta` somewhere in your path.

## Usage

`git branchmeta -h`

A `.gitbranch` file will be used as the canonical source of branchmeta for this
plugin if one is provided. It is in the same format as gitconfig files.
It should be added to `.gitignore` so it can exist in all branches (otherwise
you would not have all the meta for all branches)

## Recommended

Create an alias: `git config --global alias.gm meta`
So you can start using meta with `git gm`

## TODO

* sync with the branch info and descriptions stored in `.git/config`.
* find a good way to keep the .gitbranch file distributed across multiple repo,
  but available to all branches
* tests

