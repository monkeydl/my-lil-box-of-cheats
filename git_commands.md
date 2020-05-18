Prune local git branches
```
git remote prune origin 
git branch -vv | grep 'origin/.*: gone]' | awk '{print $1}' | xargs git branch -d
```

Search for something that's been deleted
```
git log -S 'search phrase' filename.extension     
```
