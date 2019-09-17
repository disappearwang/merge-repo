this repository is merged with github-connexion-test.git


As following : 

```
git remote add temps https://github.com/disappearwang/github-connexion-test.git
```

then we can fetch all remote contents and its tags : 

```
git fetch temps --tags
```

so we could merge it into current repo

```
git merge temps/master
```

as some conflits will appear, we may have an another commit for merge : 
```
git add .
git ci -m "merge github-connexion-test to merge-repo"
git push
```

at last we can delete the temps:

```
git remove remote temps
```

check the config is clear : 

```
git config --local -l
```
