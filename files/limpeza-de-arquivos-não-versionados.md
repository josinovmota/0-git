# Cleaning un-versioned files

By utilizing `git status` we have an idea about the state of our **git tree**. Through this command we can see which files exist only locally and are not yet staged(in the staging area). To keep a **clean workspace** without **un-versioned files** we need to be sure that:

- There are no untracked files
- There are no staged files waiting to be committed

# How to clean un-versioned files

To get rid of the **untracked files** we utilize the command:

```shell
git clean
```

This command has some flags:

- `-n`: Shows what would be removed, without actually deleting anything
- `-f`: Actually deletes untracked files
- `-d`: Also deletes directories
- `-x`: Delete files included in `.gitignore`
 

## ⚠️ Very Important⚠️

Deleting files could cause you to lose **important work**, so always be sure of what you're actually deleting
