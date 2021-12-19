# Using Git Large File Storage (lfs)

GitHub limits the size of files allowed in repositories. If you attempt to add or update a file that is larger than 50 MB, you will receive a warning from Git.

GitHub blocks pushes that exceed 100 MB.

To track files beyond this limit, you must use Git Large File Storage (Git LFS). 

[Reference](https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-large-files-on-github#file-size-limits)

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
