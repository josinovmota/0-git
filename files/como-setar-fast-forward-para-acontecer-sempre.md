# How do I set my local configuration to ensure only fast-forward merges?

In order to set a local configuration to only fast forward you'll have to create an alias:

```
git config alias.ffmerge "merge --ff-only"
```

Now, when you want to do a fast-forward merge you can use:

```
git ffmerge <branch-name>
```

If you want to do this while using `git pull`, you can use the command:

```
git config pull.ff only
```

Also, theres a more direct way to enforce fast-forward to all merges:

```
git config --global merge.ff only
```

The whole difference is that `git config --global merge.ff only` enables fast-forward to `git pull` and `git merge` simultaneously, instead of `git config pull.ff only`, which only enables it to `git pull` 
