# What is a Git alias?

A Git alias is a way to create a shortcut for some actions. Let's do an example:

```shell
git config --global alias.pr git remote prune origin
```

This command is creating an alias `pr` of the command `git remote prune origin`. Now, when i want to use this whole command, I can easily write:

```shell
git pr
```

And the old branches of Origin will be removed
