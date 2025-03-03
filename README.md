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
```
### 6
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git add unwanted.txt && git commit -m "unwanted commit"`
[main d6ca7f7] unwanted commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 unwanted.txt

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git rebase -i`
Successfully rebased and updated refs/heads/main.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git push --force`
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 328 bytes | 328.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/kezagiselle/GitAdvanced.git
   ce186be..d203b6c  main -> main

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$
```
### 7
``` bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git rebase -i`
Successfully rebased and updated refs/heads/main.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$
```
### 8
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (ft/work)
$ `git checkput main`
git: 'checkput' is not a git command. See 'git --help'.

The most similar command is
        checkout

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (ft/work)
$ `git checkout main`
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git log ft/work`
commit 0a96ce983a7c9e3684294b2cd0603a5a38c63ab5 (ft/work)
Author: kezagiselle <kezagiselle776@gmail.com>
Date:   Thu Feb 27 12:02:31 2025 +0200


lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git cherry-pick 0a96ce983a7c9e3684294b2cd0603a5a38c63ab5`
[main 8b23998] implemented test 5
 Date: Thu Feb 27 12:02:31 2025 +0200
 1 file changed, 11 insertions(+)
 create mode 100644 test.html

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$
```
### 9
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git log --graph`
* commit 8ff4a819598660b0ca47e5785f873cf0775ee2f7 (HEAD -> main)
| Author: kezagiselle <kezagiselle776@gmail.com>
| Date:   Thu Feb 27 12:12:13 2025 +0200
|
:
```
### 10
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git reflog`
8e5d611 (HEAD -> main, origin/main, origin/HEAD) HEAD@{0}: commit: another exercise on part1
8ff4a81 HEAD@{1}: commit: another exercise
8b23998 HEAD@{2}: cherry-pick: implemented test 5
:
```
### Part 2
### 1
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git checkout -b ft/working`
Switched to a new branch 'ft/working'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (ft/working)
$
```
### 2
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (ft/working)
$ `git add feature.txt && git commit -m "Implemented core functionality for new feature"`
[ft/working d8e1b9c] Implemented core functionality for new feature
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 feature.txt

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (ft/working)
$
```
### 3
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (ft/working)
$ `git checkout main`
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git add readme.txt && git commit -m "Updated Project readme"`
[main ebdd06d] Updated Project readme
 1 file changed, 4 insertions(+)
 create mode 100644 readme.txt
```

### 5
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (ft/working)
$ `git branch --merged`  
* ft/working
  main

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (ft/working)
$ `git branch -d ft/workimg`
error: branch 'ft/workimg' not found.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (ft/working)
$ `git branch -d ft/working`
error: Cannot delete branch 'ft/working' checked out at 'C:/Users/lenovo/Documents/THE GYM/GitAdvanced'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (ft/working)
$ `git checkout main`
Switched to branch 'main'
M       README.md
Your branch is up to date with 'origin/main'.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git branch -d ft/working`
error: The branch 'ft/working' is not fully merged.
If you are sure you want to delete it, run 'git branch -D ft/working'.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git branch -D ft/working`
Deleted branch ft/working (was 115b7f7).

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$
```
### 6
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git log --oneline`
5a7cf70 (HEAD -> main, origin/main, origin/HEAD) added some exercises
6a5f33a some other exercises on the readme file
ebdd06d Updated Project readme
a664f6b another exercise here

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git checkout -b ft/commit-Branch <a664f6b>`
bash: syntax error near unexpected token `newline'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git checkout -b ft/commit-Branch a664f6b`
Switched to a new branch 'ft/commit-Branch'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (ft/commit-Branch) 
$
```
### 7
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)     in)
$ `git merge ft/commit-Branch`
Already up to date.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$
```
### 8
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git checkout ft/commit-Branch`
Switched to branch 'ft/commit-Branch'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (ft/commit-Branch)
$ `git rebase main`
Successfully rebased and updated refs/heads/ft/commit-Branch.     

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (ft/commit-Branch)
$
```
### 9
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git branch -m ft/commit-Branch ft/improved-branch`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git checkout ft/improved-branch`
Switched to branch 'ft/improved-branch'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (ft/improved-branch)
$
```
### 10
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git checkout bba1efc`
Note: switching to 'bba1efc'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make 
in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:
  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at bba1efc feat: Branch Rebasing

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced ((bba1efc...))
$
```
## Part 3
### 1
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git stash`
Saved working directory and index state WIP on main: 9342d22 feat: checking Out Detached HEAD

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$
```
### 2
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git stash pop`
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a") 
The stash entry is kept in case you need it again.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$
```
### 3
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git add feature.txt`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git commit -m "Modify example.txt in feature-branch"`
[main 9bf7577] Modify example.txt in feature-branch
 1 file changed, 1 insertion(+)
 create mode 100644 feature.txt

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git checkout main`
Already on 'main'
M       README.md
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git merge ft/improved-branch`
Already up to date.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$
```
### 4
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$ `git mergetool`

This message is displayed because 'merge.tool' is not configured. 
See 'git mergetool --tool-help' or 'git help config' for more details.
'git mergetool' will now attempt to use one of the following tools:
opendiff kdiff3 tkdiff xxdiff meld tortoisemerge gvimdiff diffuse 
diffmerge ecmerge p4merge araxis bc codecompare smerge emerge vimdiff nvimdiff
No files need merging

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Documents/THE GYM/GitAdvanced (main)
$
```


