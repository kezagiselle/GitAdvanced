# GitAdvanced

```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git add app.html && git commit -m "chore: Create initial file"`
[main fbee885] chore: Create initial file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 app.html

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git add index.js && git commit -m "chore: create another file"`
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git add work.js && git commit -m "chore: create another file"`
[main 3f405ba] chore: create another file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 work.js

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$
```

# Challenges: 
## Part1
### 1
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git status`
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git log`
commit 2c21494b76639c7433c1dc7d94112175136f28a0 (HEAD -> main, origin/main, origin/HEAD)
Author: kezagiselle <kezagiselle776@gmail.com>
Date:   Wed Feb 26 15:26:58 2025 +0200
:
```
### 2
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git rebase -i HEAD~2`
Successfully rebased and updated refs/heads/main.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git push origin main --force`
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 513 bytes | 256.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/kezagiselle/GitAdvanced.git
   2c21494..af78a04  main -> main

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$
```
### 3
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git rebase -i HEAD~2`
Successfully rebased and updated refs/heads/main.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git push origin main --force`
Everything up-to-date

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$
```
### 4
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)    
$ `git reset HEAD~1`
Unstaged changes after reset:
M       README.md

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)    
$ `git add stage.html`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)    
$ `git commit -m "another exercise"`
[main cec83c3] another exercise
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 stage.html

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)    
$ `git add stage.js`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)    
$ `git commit -m "another challenge"`
[main 2cd2eb3] another challenge
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 stage.js

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)    
$ `git push origin main --force`
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 447 bytes | 149.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 1 local object.     
To https://github.com/kezagiselle/GitAdvanced.git
 + 7737e3f...2cd2eb3 main -> main (forced update)

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)    
$
```
### 5
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git rebase -i HEAD~2`
Successfully rebased and updated refs/heads/main.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git push --force`
Everything up-to-date

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$