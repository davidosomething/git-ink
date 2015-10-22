# git-ink (alpha)

Pull out the `[branch]` description from your `.git/config`; quickly edit and
view your branches, with annotations; hashtag branches for easier management.

![Screenshot of output](screenshot.png)

## Support

- OSX - Partial
    - the `git ink` command works but options do not (pending a getopts rewrite)
        - Use `git branch --edit-description` to add descriptions in the interim
-* Linux - Full
    - `git ink` and all its flags work.

## Install

Put `git-ink` somewhere in your path.

## Usage

```shell
git ink -h
```

A `.gitbranch` file will be used as the canonical source of meta data for this
plugin if one is provided. It is in the same format as gitconfig files.
It should be added to `.gitignore` so it can exist in all branches (otherwise
you would not have all the meta for all branches)

## TODO

- sync with the branch info and descriptions stored in `.git/config`.
- find a good way to keep the .gitbranch file distributed across multiple repo,
  but available to all branches
- rewrite in Ruby or Python for better compatibility
- tests

## Changelog

- 2015-10-22 - Updated screenshot

- 2015-10-19 - Change output formatting, indent branch descriptions

