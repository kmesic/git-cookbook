# GIT CHEATSHEET
Basic commands to work with Git, along more complex flows and situations.

**Some of the examples have --- between lines. This indicates that everything above the line is the command structure, while everything below is an example**
## Basics
Clone a repo
```
git clone {repo_https_or_ssh_url}
git clone https://github.com/username/repo-to-clone
```

Add to staging area
```
git add {file_name_or_directory}
---
git add test_file
```

Commit
```
git commit -m "Message about commit"
```

## Branches
View current branches locally. Current branch will be marked with a `*`
```
git branch
```

View all remote branches fetched locally.
```
git branch -r
```

View all branches (local and remote)
```
git branch -a
```
*Note: Remote branches must be fetched first to be seen*

Create a new local branch
```
git branch {branch_name}
git checkout {branch_name}
---
git branch new_branch
git checkout new_branch
```

Shorthand
```
git checkout -b {branch_name}
```

## Remote Repos
Conventions: 
- **origin** is your root remote repo
- **upstream** is the repo you forked from

### Basics
Be able to fetch/push/pull from a remote repo
```
git remote add {name} {repo_https_or_ssh_url}
---
git remote add origin https://github.com/username/repo-to-clone
```

Remove a remote repo
```
git remote rm {name}
---
git remote rm origin
```

Push to a remote repo
```
git push {remote_repo} {local_branch}
```

### Keeping a forked repo up to date with original repo

1. Add another remote branch to pull from
2. Fetch remote branch into a local branch
3. Merge the remote branch into a local branch
```
git clone {forked-repo-url}
cd forked-repo
git remote add upstream git://github.com/ORIGINAL-DEV-USERNAME/REPO-YOU-FORKED-FROM.git
git pull upstream master
```

git pull is the same as doing a fetch and merge
```
git fetch upstream
git merge upstream/master master
```