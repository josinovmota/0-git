# What does the `--theirs` merge strategy do? How do you invoke it?

Lets imagine that you are trying to do a `git merge` from your `main` with a branch named `feature/answers`. The command `git merge` do something better than just changing the content of `main` to the `feature/answers`. It compares both branches in order to find some problems(thanks merge o/). When the command merge finds a problem, it raises a CONFLICT. Let me show an example:

```shell
CONFLICT (content): Merge conflict in config.txt
Automatic merge failed; fix conflicts and then commit the result.
```

In order to fix this, you'll have to choose what version of the `config.txt` file you would like to keep. To keep the `feature/answers` version of `config.txt` you can use:

```shell
git checkout --theirs config.txt
```

To keep the `main` branch version of `config.txt` you can use:

```shell
git checkout --ours config.txt. Both of them solves the problem
```


