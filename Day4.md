## Commit only one file to branch

### Make multiple files and add only single file to a branch

```bash
git branch develope
```

```bash
git touch demo.txt
```

```bash
git commit -m "text commit"
```

```bash
git loge --oneline
```

copy the file id (a7bb83f)

```bash
copy commit id
```

```bash
git checkout develope
```

```bash
git cherry-pick a7bb83f
```

```bash
ls
```

To restore the staged file in the commit area (Staged area) when we add file (add .)
 
```bash
git restore --staged demo.txt
```

```bash
git commit -m "msg"
  
git log 
```

To revert the commit file (demo.txt)

```bash
git revert <commit id>
```
