# How to undo changes on a file added to the index

Let's imagine that your boss asked you to change the `main.py` file language to **Portuguese**. After all the changes, you ran `git add main.py` and when you were about to do `git push` your boss appeared and said "Hey, don't do the changes anymore". Now you have to restore the file to the last **commit(HEAD)** of your **current branch**

In order to do that, you'll have to restore the `main.py` file that is already in **staging area** to the state before your changes. The command to do this is `git restore --staged <file_name>`:

```shell
git restore --staged main.py
```

If you want to specify the staged file state to the HEAD of another branch, you'll also have to use the flag `--source=<branch>`:

```shell
git restore --staged --source=feature/git main.py
```

Here we are restoring staged `main.py` to its current state in the HEAD of the branch `feature/git`

