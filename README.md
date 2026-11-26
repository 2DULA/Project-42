
- .env never gets committed becuase its listed inside the .gitignore file

## Git Workflow Proof

- **Clone URL**: `git@github.com:2DULA/Project-3.git`
- **PR Link**: `https://github.com/2DULA/Project-3/pull/1`
- **Graph Commit**: 
```text 

 *   3e4e54e (HEAD -> master, origin/master) Merge pull request #1 from 2DULA/deploy
|\  
| * 145baa3 (origin/deploy, deploy) Add test file and update README
| * e111ecb Push new README to the deploy branch
|/  
* 3d62558 Add git ignore to exclude node_modules/, __pycahce__/ and .env
* 8e16bcb Add READ.me with developer introduction

```


# 1. Inspect Status, Files & History
- git status
- git branch
- git log --oneline --graph


# 2. Connect Remote & Push Initial Branch
- git remote add origin <repo-url>
- git remote -v
- git push -u origin master

# 3. Stage & Commit Changes
- git add <file>                     # or: git add .
- git commit -m "Commit message"
- git commit -am "Commit messgae" *FOR FILES ALREADY TRACKED*

# 4. Amend Last Commit & Force-Push Safely
- git commit --amend -m "New message"
- git commit --amend --no-edit
- git push --force-with-lease

# 5. Branch, Pull Request Sync & Cleanup
- git checkout -b <branch-name>
- git push -u origin <branch-name>
- git checkout master
- git pull
- git branch -d <branch-name>