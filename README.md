# UsefulGitCommand
This repo created for collect useful git command and situation that we should use.

# Simaple git command for add change and push to remote repo.
```
git add -A
git commit -m <"Message that you want to commit">
git push origin <branch-id>
```

# if commit wrong in last commit 
```
$ git reset --hard HEAD       (going back to HEAD)
$ git reset --hard HEAD^      (going back to the commit before HEAD)
$ git reset --hard HEAD~1     (equivalent to "^")
$ git reset --hard HEAD~2     (going back two commits before HEAD)
```

# if commit wrong and you already add the new commit
**Step 1: Checkout new branch from master.**
`git checkout -b <branch-name>`

**Step 2: Cherry-pick commit that you want in to new branch.**
`git cherry-pick <commit-id>`

**Step 3: Delete old branch.**
`git branch -D <branch-name>`

**Step 4: Rename new branch to old branch.**
`git branch -m <old-name> <new-name>`

**Step 5: (Optional) Force push to remote repo.**
`git push –force origin <branch-name>`
