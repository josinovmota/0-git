# How to undo change on a single file

Let's imagine that your boss asked you to change the `main.py` file language to **Portuguese** but in the middle of the process he said "It's ok, no need to do this anymore". Now, you have to restore the file to the last commit.

In order to do that, you'll have to restore the `main.py` file to its state before changes. The command to do this is `git restore <file-name>`:

```shell
git restore main.py
```

If you want to specify the file state to the HEAD of another branch, you'll have to use the flag: `--source=<branch>`:

```shell
git restore --source=feature/git main.py
```

Here we are restoring `main.py` to its current state in the HEAD of the branch `feature/git`
