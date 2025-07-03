# How do I set my local configuration to ensure only fast-forward merges?

In order to set a local configuration to do only fast forward you'll have to create an alias:

```
git config alias.ffmerge "merge --ff-only"
```

Now, when you want to do the fast-forward merge you can use:

```
git ffmerge <branch-name>
```

If you want to do this while using `git pull`, you can use the command:

```
git config pull.ff only
```

