# What is a fast-forward merge?

Lets imagine that you have a `main` branch with the following commits(A, B, C):

```
A -- B -- C
```

Now you created a new branch named `feature/answers` from `main` and did 5 commits there:

```
A -- B -- C
           \
            D -- E -- F -- G -- H
```

After doing all those commits you decide to merge the branch `feature/answers` with `main`. Now, Git, instead of doing all those changes(D, E, F, G, H) as only **one** commit like that:

```
A -- B -- C -- D
```

It will include all the commits from `feature/answers` in the branch `main`:

```
A -- B -- C -- D -- E -- F -- G -- H
```

In this case, the act of preserving the `feature/answers` commits in the branch `main` Tree of commits is named "Fast-forward merge"

