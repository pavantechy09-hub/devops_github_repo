PART 1: Foundations of Git & GitHub
Chapter 1: What is GitHub
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --list
git init
git clone <repo-url>
git status
git add <file>
git add .
git commit -m "message"
git remote add origin <repo-url>
git push -u origin main
git pull origin main

Chapter 2: Git Branching
git branch
git branch <branch-name>
git checkout <branch-name>
git checkout -b <branch-name>
git merge <branch-name>
git branch -d <branch-name>
git branch -D <branch-name>

Chapter 3: Git Pull Request
git push origin <branch-name>
git fetch origin
git pull origin main

Chapter 4: Git in Visual Studio
git add .
git commit -m "message"
git pull
git push

PART 2: Advanced Git Commands & Strategies
Chapter 5: Git Reset
git reset --soft HEAD~1
git reset --mixed HEAD~1
git reset --hard HEAD~1
git reset <commit-hash>

Chapter 6: Git Amend
git add <file>
git commit --amend -m "new message"

Chapter 7: Git Cherry Pick
git cherry-pick <commit-hash>

Chapter 8: Git Squash
git rebase -i HEAD~<number-of-commits>
# change 'pick' to 'squash' or 's'

Chapter 9: Git Reorder
git rebase -i HEAD~<number-of-commits>
# rearrange commits in editor

Chapter 10: Git Drop
git rebase -i HEAD~<number-of-commits>
# remove lines or mark commits as 'drop'

Chapter 11: Git Exec
git rebase -i --exec "<command>" HEAD~<number>

Chapter 12: Git Bisect
git bisect start
git bisect bad
git bisect good <commit-hash>
git bisect reset

Chapter 13: Git Stash
git stash save "message"
git stash list
git stash show stash@{0}
git stash apply stash@{0}
git stash pop
git stash drop stash@{0}
git stash clear

Chapter 14: Git Diff
git diff
git diff --cached
git diff <commit1> <commit2>
git diff branch1..branch2
git diff --name-only

PART 3: Best Practices & Problem Solving
Chapter 15: Git Log
git log
git log --oneline
git log --graph --oneline
git log -p
git log --stat
git log -- <file>

Chapter 16: Git Ignore
# create/edit .gitignore
# example entries:
node_modules/
*.log
.DS_Store
.vscode/

Chapter 17: Merge Conflict
git merge <branch-name>
# (resolve conflicts manually)
git add <file>
git commit
git merge --abort

Bonus / Miscellaneous Git Commands
git reflog
git tag
git tag -a v1.0 -m "Release 1.0"
git push origin --tags
git revert <commit-hash>
git show <commit-hash>
git blame <file>
git clean -fd
