# This code has many errors!
### I am learning and improving myself.

---

```
git config --global user.name "MrMrProgrammer"
git config --global user.email "mrmrprogrammer@gmail.com"
```

```
git init
```

```
git status
```

```
git add <file>
```

```
git commit -m "commit message"
```

```
git add <file_1> <file_2> ...
```

```
git log
```

```
git commit -a -m "commit message"
```
just for modified files. NOT new file!


```
git add -A
```
for add all files.
you can use this command to add all files instead of using git add for each file individually.

```
git show <commit hash>
```
for see commit changes in details


```
git diff
```

```
git diff -u
```

```
git diff -u <file_1> <file_2> > changes.diff
git patch changes.txt < changes.diff
```

```
git diff --staged
```

```
git diff <hash>
```
or
```
git diff <hash_1> <hash_2>
```

```
git add -p
```
for check each file

```
git mv <file>
```

```
git rm file
```
---

```
git checkout <file>
git restore <file>
git restore --staged <file>
git reset <file>
```

```
git commit --amend
```
با این دستور میتوانیم یک کامیت رو جایگزین آخرین کامیت کنیم
اگر هیچ فایلی staged نشده باشه، فقط متن کامیت تغییر میکنه
اگر فایلی رو staged کرده باشیم، اون فایل هم به این کامیت اضافه میشه
توجه شود که هش کامیت تغییر خواهد کرد

```
git revert <git-hash>
```

```
git pull
```

for syncy local system with github/gitlab


```
git branch
git branch -v
```

```
git branch <branch_name>
```
create new branch

```
git checkout <branch_name>
```


```
git branch X
git checkout X
```

```
git checkout -b X
```
there are same. it is shortcut.

```
git branch -d <branch_name>
```
for delete branch


## Merge
```
git checkout main
git merge <branch_name>
```

we have some kind of merge. one of them is `FastForvard`
other one is `3Way`

```
git merge --abort
```
used when we have conflict in merge process. for cancel merge


```
git branch -D <branch_name>
```
for delete branch that has unmerged commit


## Git Log
```
git log --graph
git log --oneline
git log --graph --oneline
```

```
git remote
git remote -v
```

---
you can create issue on github and close this issues with one of these key words:

```
| Message       | Result     |
| ------------- | ---------- |
| `#2`          | Just links |
| `Fixes #2`    | Closes     |
| `Closes #2`   | Closes     |
| `Resolves #2` | Closes     |
```

for example you can close issue #2 automatically when use one of these kew words + issue number in commit message


```
git push
git pull
```

```
git remote show origin
```
just get data about remote

```
git fetch
git fetch --all
```

```
git log origin/main
```

```
git merge origin/main
```

```
git remote update
```

```
git fetch
git merge origin/main
```
this commands equale to this command
```
git pull
```

```
git log --graph --oneline --all
```
for see logs in one line


## Conflict
when you have Conflict, you can use 3way merge
```
git merge --no-ff

ff = fast forward
```
در این زمان باید ابتدا کانفلیکت را رفع کنیم و سپس مانند یک کامیت معمولی آن تغییرات رو کامیت کنیم


fast forward
یعنی بتونیم راحت تغییرات شاخه من رو بزاریم انتهای شاخه اصلی
