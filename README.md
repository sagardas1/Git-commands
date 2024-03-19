#### GIT COMMANDS:

1. Delete branch locally:
   ```git branch -D <branch_name>```

2. Patch apply:
   ```cd /c
   cd -
   git apply /c/Users/sada1022/...
   ```


3. resolve incomming and outgoing commint and make it indentical with remote branch.
   ```git reset --hard origin/<branch_name>```

4. git squash:

```git rebase -i HEAD~10
p
f
f
f
f
f
f
f
f
f
f
f
s- will give one more time to change the comit message.
git push -f
or

git push -f origin <branch name> 
```

5. git multiple commit message:
   ```
   git commit -m "fix"
   git commit --amend
   press i
   add commit message then press Esc :wq
   git push -f
   ```


6. to check changes in git bash
```gitk```

7. to check latest log
```git log```

8. git rebase locally
```
git checkout main branch
git pull
git checkout current branch
git pull
git rebase <OriginBranch>
if merge conflit comes
resolve it from idea.
git add those merge conflit files
git rebase --continue
git push -f
```

9. send localchanges to new brach:
```
git push origin <old_branch>:<new_branch>
```

10. change branchName in repo::
```
1.git branch -m "<new name>"
2.git push origin :<old_branch>
3.git push -u origin <new name>
```

11. Command to edit the commit message
```
git commit --amend
press i
edit the comment
press ESC then :wq enter
git push -f
```

12. git push to a branch thats not there in repository
```
git push -u origin <branch name>
```
13. create a branch:
```
go to the branch from where you want to create:
git checkout master

git pull

git checkout -b <new branch name>
```

14. change local branch name:
```
git checkout <old_branch>
git branch -m <new branchname>

git push new local branch to repo
git push -u origin <branchName>
```


