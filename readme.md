# Using Git Large File Ftorage (lfs)

Install
```bash
git lfs install
```

Add file types to store in lfs
```bash
git lfs track "*.csv"
```

Commit and push changes
```
git add .
git commit -m "added csv file"
git push
```

---

Git lfs attributes
- store files as lfs even if not added before installing lfs
- add large file and tracking at the same commit works
- cloning a repo still clones the large file
