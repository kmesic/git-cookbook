# Git Cookbook

### Remote repos
Remove tracking/pushing/pulling from a remote repo
```
git remote rm {name}
git remote rm origin
```

Add a remote repo
```
git remote add {name} {remote_url}
git remote add origin https://github.com/username/repo-to-clone
```

#### Keep fork repo up to date with original repo 
Add another remote branch to pull from
```
git clone {fork-repo-url}
cd fork-repo
git remote add upstream git://github.com/ORIGINAL-DEV-USERNAME/REPO-YOU-FORKED-FROM.git
git fetch upstream
```

Pull and merge changes from original repo into forked repo master branch
```
git pull upstream master
```

