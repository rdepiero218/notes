# Git Notes and Basic Workflows

## Pushing and pulling 

These are for when I'm working by myself and the quick and dirty way of backing up a repo.

### Pushing to a repo

```
git add *
git commit -m "add a message"
git push origin main
```
### To pull

`git pull origin main`

### Create a new branch and switch to it

`git checkout -b ＜new-branch＞`

## Removing DS_Store Files

`find . -name .DS_Store -print0 | xargs -0 git rm -f --ignore-unmatch`

Then add it to your  `.gitignore`

```
echo .DS_Store >> .gitignore
git add .gitignore
git commit -m '.DS_Store banished!'
```
