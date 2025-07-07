# The remote branch is gone! How do I clean up my local workspace of old branches?

You started your daily work and find out that the remote branch `origin/feature/answers` is gone. It means that when you turn on your computer, this branch will still be there -- only locally. To solve this we use the following command:

```shell
git remote prune origin
```

It's good to remember that "Origin" is just a default name from remote. In your project it could have another name like "Upstream"
