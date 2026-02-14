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
