# How do you undo changes for the entire workspace

In order to undo all the changes that you've made in the entire workspace you'll have to use the command `git restore .`. The `.` means that you're including everything in the current working directory.

```shell
git restore .
```

If you want to restore everything to a particular HEAD of another branch, you'll have to use the flag `--source=<branch>`.

```shell
git restore --source=feature/answers .
```

