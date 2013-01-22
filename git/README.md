Git Helpers
===========

A simple guide to getting started with Git

### Cloning a repository

Cloning means copying all files from a remote repository to the current location on your local machine. The simpliest form of cloning is:

```
git clone https://github.com/user/example
```

This copies all files to a new folder called 'example'. You can assign a different name to the folder by using:

```
git clone https://github.com/user/example folder
```

### Forking a repository

Forking a repository is similar to cloning, but instead of giving you access to push to  :

```
git clone https://github.com/user/example
```

This copies all files to a new folder called 'example'. You can assign a different name to the folder by using:

```
git clone https://github.com/user/example folder
```

### Aliases

Aliases are a great way to save some typing by shortening a command (or commands) into an alias.

There are two ways of creating them - either the command line, or editing the `gitconfig` file directly.

When using the command line, as with all config options, you have the choice to make it globally accessible or restrict it to just that repository.

```git
// Globally accessible
git config --global alias.ci commit
```

```git
// Restricted to only that repository
git config alias.ci commit
```

To use the above alias, you type:

```git
git ci -m "This is a commit message"
```

You can also combine multiple commands into an alias, like so:

```git
// You must use single quotes to wrap your expression
git config --global alias.di '!git add -A && git commit'
```

Alternatively, if you want to add them to the `gitconfig` file itself, head to where Git is installed "C:\Program Files\Git\etc\gitconfig" and add the above rules as follows:

```config
[alias]
    ci = commit
    ac = !git add -A && git commit
```

<a href="https://gist.github.com/4596493">Here are some useful aliases</a>