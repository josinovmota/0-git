# What is a Git alias?

A Git alias is a way to create a shortcut for some actions. Let's see an example:

```shell
git config --global alias.pr git remote prune origin
```

This command is creating an alias `pr` of the command `git remote prune origin`. Now, when I want to use this whole command, I can easily write:

```shell
git pr
```

And the old origin branches will be removed
