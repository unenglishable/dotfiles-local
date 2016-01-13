An explanation of some of the configurations in this project...

# ~/.aliases.local

I use a ton of custom aliases on a daily basis.  Why?  I guess it's because they
are easy to implement.

## Meta aliases

### `aliens` and `sauce`

These "meta" aliases let me edit my aliases file, and then source it.  How
convenient.

## Git aliases

### `g`

Oh.  What's this?  I only use one command that starts with "g".  Why not alias
`git` to `g` then?  I use this command when I don't already have an alias for
what I want to do, or if I want to do something a little complicated, and I want
to be explicit and verbose about it.

### `gap`, `ghp`, `gss`

I almost exclusively use these instead of the regular commands.  Patch adding,
resetting, and checking out is a really awesome way to get granular control over
your commits.

### `gl`, `gla`

Super useful when on a headless server, these commands will let you see a pretty
diff tree on the command line.


### `gka`

Okay, `gitk` is pretty old and lots of people criticize me for using it, but I
still have yet to find a good replacement that is simple and does everything I
use gitk for.  (Yes, I have tried `gitx`)

### `gc`, `gh`, `gf`, `gp`

These are just shorthands for two word commands that I commonly do.

### `gs`

This two word command is special.  I do it almost every time I start a terminal
session, or focus on a terminal window.  If you're an experienced command line
user, you probably do at least `ls` every single time you start typing in a
window.  My go-to is `ls` then `gs` -- rolls right off the fingers ;)


### `gsm`

I was coding and was frustrated by a huge amount of changed files when I was
rebasing/merging.  I just want to see the damned conflicting files!  This
command should show which files have conflicts. (but does not output in colour)

### `gss`, `gsl`

These are pretty nifty commands for working with stashes.  I pretty much NEVER
do a `git stash pop` because it is unruly to deal with when you fuck up.  In
that case, you want to see what's in the stash stack (`gsl`) and actually diff
that thing against your current working branch (`gss`) before you go and dump
the whole thing *using `git stash apply` instead of `git stash pop`*.  Then, use
`git stash drop` when you know you're done with the stash item for sure.

## bash aliases

Some of these are pretty silly-sounding, but actually have many usecases and can
be quite handy.

### `incognito`

`unset`'s the HISTFILE so you can work without worrying about others looking at
your bash command history.  (Does not protect you from other commands'
histories).

### `jesus`

When you just installed a new command, but it hasn't loaded in, so you can't run
it, this command will reinstate bash for you.  (it kills your session and comes
back from the dead).

### (sudo aliases)

These are mostly just for fun :D

### `duh`

Super useful way to get the size of a file in human-readable format.  Protip:
use `duh -s` to get a summary of the size of a directory.

### `rem`, `cpr`

For creating and destroying ~~entire galaxies~~ directories with ease.

### `la`, (`ll`)

Who wants to ever type `ls -a` or `ls -l`?  Geez...

### `pwd`

My `pwd` will clear the screen and list the current directory at the very top,
because I never need to see the previous output when I want to know where I am.
