I will keep some notes here
Only index.html is related to the developing project.

## reflog

It is different from "git log". "git log" is the real status now. If "reset" has been used to get back to a former version, "git log" could not show the latest version. But "git reflog" will show all the progress you have made.

For example, if you use "git reset --hard" to get back to "function two", with "git reflog" you can see:
```
e77553c (HEAD -> master) HEAD@{0}: reset: moving to e77553c4022921963f680c1c5e9b4cf5df9e1e26
10f5755 HEAD@{1}: commit: feat(index): add fucntion three
e77553c (HEAD -> master) HEAD@{2}: commit: feat(index): add fucntion two
d30d98e HEAD@{3}: commit: adjust(dbhot): adjust the structure of the project and let this be the first version
```

But with "git log", you cannot see function three anymore. So using "git reflog" to check id, you can still get back to function three.

## git status change
![git status](./pic/git_status.png)
Some of these actions can be seen from "git status" as instructions.

## branch
