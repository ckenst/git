# Git

Useful Git commands

## Set upstream branch using git push

```bash
git push --set-upstream <remote> <branch>
```

## Delete remote branch

```bash
git push origin --delete <name of branch>
```

## Ignore a directory

If you've been tracking a directory and later decide to ignore the whole directory, simply adding it to `.gitignore` isn't enough. First you must add the directory to .gitignore, then run this command:

```bash
git rm -r --cached your-directory
```

## Add .gitignore to an existing repository

Similar to above, but if you've added a `.gitignore` with a lot of changes.

```bash
git rm -r --cached .
git add .
git commit -m "Message"
```

## Accidentally committed to develop and want to move that commit to a branch

```bash
git branch new-branch
git reset HEAD~1
git checkout <files>
```

