# Gym-Git-Exercise-Solutions

This repository contains solutions of Git Exercises provided by The Gym

## Bundle 1

### Exercise 1

```console
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle$ mkdir exercise-1
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle$ cd exercise-1/
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git init
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint:
hint: 	git config --global init.defaultBranch <name>
hint:
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint:
hint: 	git branch -m <name>
Initialized empty Git repository in /home/zkaynl7/Documents/git-bundle/exercise-1/.git/
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ echo "Task 2: Add files" > test_file
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	test_file

nothing added to commit but untracked files present (use "git add" to track)
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git branch -m master main
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	test_file

nothing added to commit but untracked files present (use "git add" to track)
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git add
Nothing specified, nothing added.
hint: Maybe you wanted to say 'git add .'?
hint: Turn this message off by running
hint: "git config advice.addEmptyPathspec false"
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git add --all
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git commit -m "changes staged and committed"
[main (root-commit) 6edd66b] changes staged and committed
 1 file changed, 1 insertion(+)
 create mode 100644 test_file
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git remote add origin main https://[sorry can't let u see my token]@github.com/Nick-Lemy/Gym-Git-Exercise-Solutions
usage: git remote add [<options>] <name> <url>

    -f, --[no-]fetch      fetch the remote branches
    --[no-]tags           import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --[no-]track <branch>
                          branch(es) to track
    -m, --[no-]master <branch>
                          master branch
    --[no-]mirror[=(push|fetch)]
                          set up remote as a mirror to push to or fetch from

zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git remote add origin main git@github.com:Nick-Lemy/Gym-Git-Exercise-Solutions
usage: git remote add [<options>] <name> <url>

    -f, --[no-]fetch      fetch the remote branches
    --[no-]tags           import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --[no-]track <branch>
                          branch(es) to track
    -m, --[no-]master <branch>
                          master branch
    --[no-]mirror[=(push|fetch)]
                          set up remote as a mirror to push to or fetch from

zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git remote add origin main https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
usage: git remote add [<options>] <name> <url>

    -f, --[no-]fetch      fetch the remote branches
    --[no-]tags           import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --[no-]track <branch>
                          branch(es) to track
    -m, --[no-]master <branch>
                          master branch
    --[no-]mirror[=(push|fetch)]
                          set up remote as a mirror to push to or fetch from

zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git remote add origin -m main https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git status
On branch main
nothing to commit, working tree clean
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git push --set-upstream origin main
Username for 'https://github.com': Nick-Lemy
Password for 'https://Nick-Lemy@github.com':
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 247 bytes | 247.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git checkout -b dev
Switched to a new branch 'dev'
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git push origin dev
Username for 'https://github.com': Nick-Lemy
Password for 'https://Nick-Lemy@github.com':
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions/pull/new/dev
remote:
To https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
 * [new branch]      dev -> dev
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git checkout -b test
Switched to a new branch 'test'
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git push origin test
Username for 'https://github.com': Nick-Lemy
Password for 'https://Nick-Lemy@github.com':
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions/pull/new/test
remote:
To https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
 * [new branch]      test -> test
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git checkout dev
Switched to branch 'dev'
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git branch -d test
Deleted branch test (was 6edd66b).
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git push origin --delete test
Username for 'https://github.com': Nick-Lemy
Password for 'https://Nick-Lemy@github.com':
To https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
 - [deleted]         test
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ ls
test_file
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ nano README.md
```

### Exercise 2

```console
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ touch home.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git add home.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git stash
Saved working directory and index state WIP on dev: 0613e6a Update README.md
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ touch about.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git add about.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git stash
Saved working directory and index state WIP on dev: 0613e6a Update README.md
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ touch team.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git add team.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git stash
Saved working directory and index state WIP on dev: 0613e6a Update README.md
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git stash list
stash@{0}: WIP on dev: 0613e6a Update README.md
stash@{1}: WIP on dev: 0613e6a Update README.md
stash@{2}: WIP on dev: 0613e6a Update README.md
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (bd2c9daa84c90330100608bd999e9884d3a21f1f)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git stash list
stash@{0}: WIP on main: 0613e6a Update README.md
stash@{1}: WIP on main: 0613e6a Update README.md
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (363403fb82ae4442b01c04dad97a9501b08602a9)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git add --all
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git commit -m "Changes committed and ready to be pushed"
[dev eccf05c] Changes committed and ready to be pushed
 2 files changed, 22 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 519 bytes | 259.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
   0613e6a..eccf05c  dev -> dev
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git stash list
stash@{0}: WIP on dev: 0613e6a Update README.md
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git stash pop stash@{0}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (9f69073eb6f057287c2e50c1b95cb335b93a0556)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git reset --hard
HEAD is now at eccf05c Changes committed and ready to be pushed
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

nothing to commit, working tree clean
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ ls
about.html  home.html  README.md
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$
```

## Bundle 2

### Exercise 1

```console
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ touch service.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git status
On branch ft/bundle-2
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        service.html

nothing added to commit but untracked files present (use "git add" to track)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git add service.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git commit -m "Service created"
[ft/bundle-2 fed067d] Service created
 1 file changed, 11 insertions(+)
 create mode 100644 service.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 442 bytes | 442.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote:
To https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$
```

### Exercise 2

```console
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout main
Already on 'main'
Your branch is behind 'origin/main' by 4 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git pull
Updating e7fff88..c9b68ba
Fast-forward
 about.html   | 11 +++++++++++
 home.html    | 11 +++++++++++
 service.html | 11 +++++++++++
 3 files changed, 33 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 service.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git status
On branch ft/service-redesign
nothing to commit, working tree clean
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ ls
about.html  home.html  README.md  service.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git add --all
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git commit -m "Update service.html"
[ft/service-redesign 1146a69] Update service.html
 1 file changed, 2 insertions(+), 2 deletions(-)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 353 bytes | 353.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote:
To https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git add --all
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git commit -m "service.html changed"
[main 859f4be] service.html changed
 1 file changed, 2 insertions(+), 2 deletions(-)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 347 bytes | 347.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
   c9b68ba..859f4be  main -> main
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git branch
  dev
  ft/bundle-2
  ft/service-redesign
* main
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout ft/service-redesign
Already on 'ft/service-redesign'
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git status
On branch ft/service-redesign
nothing to commit, working tree clean
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ ls
about.html  home.html  README.md  service.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git merge main
Auto-merging service.html
CONFLICT (content): Merge conflict in service.html
Automatic merge failed; fix conflicts and then commit the result.
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git diff -help
error: invalid option: -help
usage: git diff [<options>] [<commit>] [--] [<path>...]
   or: git diff [<options>] --cached [--merge-base] [<commit>] [--] [<path>...]
   or: git diff [<options>] [--merge-base] <commit> [<commit>...] <commit> [--] [<path>...]
   or: git diff [<options>] <commit>...<commit> [--] [<path>...]
   or: git diff [<options>] <blob> <blob>
   or: git diff [<options>] --no-index [--] <path> <path>

common diff options:
  -z            output diff-raw with lines terminated with NUL.
  -p            output patch format.
  -u            synonym for -p.
  --patch-with-raw
                output both a patch and the diff-raw format.
  --stat        show diffstat instead of patch.
  --numstat     show numeric diffstat instead of patch.
  --patch-with-stat
                output a patch and prepend its diffstat.
  --name-only   show only names of changed files.
  --name-status show names and status of changed files.
  --full-index  show full object name on index lines.
  --abbrev=<n>  abbreviate object names in diff-tree header and diff-raw.
  -R            swap input file pairs.
  -B            detect complete rewrites.
  -M            detect renames.
  -C            detect copies.
  --find-copies-harder
                try unchanged files as candidate for copy detection.
  -l<n>         limit rename attempts up to <n> paths.
  -O<file>      reorder diffs according to the <file>.
  -S<string>    find filepair whose only one side contains the string.
  --pickaxe-all
                show all files diff when -S is used and hit is found.
  -a  --text    treat all files as text.


zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git diff main ft/service-redesign
diff --git a/service.html b/service.html
index bb88165..e5741cb 100644
--- a/service.html
+++ b/service.html
@@ -3,9 +3,9 @@
   <head>
     <meta charset="UTF-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Dservice on main branch</title>
+    <title>ft/service-redesign</title>
   </head>
   <body>
-    <h1>Service on main</h1>
+    <h1>Service in ft/service-redesign branch</h1>
   </body>
 </html>
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git merge main
error: Merging is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git add --all
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git merge main
fatal: You have not concluded your merge (MERGE_HEAD exists).
Please, commit your changes before you merge.
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git commit -m "almost done"
[ft/service-redesign da9b0d8] almost done
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git status
On branch ft/service-redesign
nothing to commit, working tree clean
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git merge main
Already up to date.
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ ls
about.html  home.html  README.md  service.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git status
On branch ft/service-redesign
nothing to commit, working tree clean
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ vi service.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ nano service.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git diff main ft/service-redesign
diff --git a/service.html b/service.html
index bb88165..e5741cb 100644
--- a/service.html
+++ b/service.html
@@ -3,9 +3,9 @@
   <head>
     <meta charset="UTF-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Dservice on main branch</title>
+    <title>ft/service-redesign</title>
   </head>
   <body>
-    <h1>Service on main</h1>
+    <h1>Service in ft/service-redesign branch</h1>
   </body>
 </html>
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git add --all
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git commit -m "okay"
[ft/service-redesign c3096e8] okay
 1 file changed, 2 insertions(+), 2 deletions(-)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push origin ft/service-redesign
Enumerating objects: 2, done.
Counting objects: 100% (2/2), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 376 bytes | 376.00 KiB/s, done.
Total 2 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
   1146a69..c3096e8  ft/service-redesign -> ft/service-redesign
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git merge main
Already up to date.
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git status
On branch ft/service-redesign
nothing to commit, working tree clean
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$
```

## Bundle 3

### Exercise 1

```console
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git status
On branch ft/service-redesign
nothing to commit, working tree clean
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ touch team.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git add --all
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git commit -m "Bundle 3, let's goo"
[ft/team-page 9dab256] Bundle 3, let's goo
 1 file changed, 11 insertions(+)
 create mode 100644 team.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 459 bytes | 229.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 6 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git pull
Updating 859f4be..0d6c337
Fast-forward
 README.md | 218 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 1 file changed, 218 insertions(+)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout ft/team-page
Switched to branch 'ft/team-page'
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git log
commit 9dab2564a4ddf2ec95e3d5aad7415ca7145fdc63 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:47:23 2024 +0200

    Bundle 3, let's goo

commit 5f7ff0f94a1a5bdc175efdfab48ec4753a5c8b39 (origin/ft/service-redesign, ft/service-redesign)
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:40:06 2024 +0200

    README.md

commit c3096e8345486a06127f5d437734095cd38eb15a
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:36:33 2024 +0200

    okay

commit da9b0d8c6862bd469ef217133fd05b053630860a
Merge: 1146a69 859f4be
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:33:06 2024 +0200

    almost done

commit 859f4bed40a4b4d9abab2e9e10164773ef93072d
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:14:42 2024 +0200

    service.html changed

commit 1146a69c27e960e617fe3621e7df93d4377fc292
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:07:28 2024 +0200

    Update service.html

commit c9b68baf8d69618bfa2f5e8646a539696f2a1a81
Merge: e7fff88 0bf5e00
Author: Nick-Lemy Niyigena Kayiranga <169042721+Nick-Lemy@users.noreply.github.com>
Date:   Tue Dec 17 14:37:37 2024 +0200

    Merge pull request #1 from Nick-Lemy/ft/bundle-2

    adding html pages

commit e7fff88384a2c8f4ca7d6495c75a1532ca35d2d4
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 14:36:43 2024 +0200

    ll

commit 0bf5e00b8df78a8d1662828b632e1c715f2d835b (origin/ft/bundle-2, ft/bundle-2)
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 14:32:55 2024 +0200

    Description added

commit fed067d37e6355850863328bc1f3936a5e1a5896
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 12:54:06 2024 +0200

    Service created

commit ee4277938cc511c5169b6532541e083f279be17d
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 12:43:21 2024 +0200

    !

commit 1c601d1534bde175ddc196b0d3667eae573ca980 (origin/dev, dev)
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 12:42:00 2024 +0200

    !

commit a31ca6eefa9d951662acdf3d4c32f445f0e508ba
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 12:39:15 2024 +0200

    !

commit 44dd93fa16d8f66c6a4c9922271aa0713b23804d
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 12:34:11 2024 +0200

    !

commit 9af481f67d2ce537cb1b31ec90d8093019f7c3c3
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 11:49:24 2024 +0200

    README.md updated for exercise 2 Bundle 1

commit eccf05cae84372ebbf344829efabe49589060b54
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 11:45:29 2024 +0200

    Changes committed and ready to be pushed

commit 0613e6aacf571633999d4efc1a022d5c22284eae
Author: Nick-Lemy Niyigena Kayiranga <169042721+Nick-Lemy@users.noreply.github.com>
Date:   Tue Dec 17 10:44:38 2024 +0200

    Update README.md

commit 1956995b24665d0d9498a3b34034d31905aa9e24
Author: Nick-Lemy Niyigena Kayiranga <169042721+Nick-Lemy@users.noreply.github.com>
Date:   Tue Dec 17 10:44:13 2024 +0200

    Update README.md

commit 0db4e20fe5b66cbc4148d9c38b12a7c786265f45
Author: Nick-Lemy Niyigena Kayiranga <169042721+Nick-Lemy@users.noreply.github.com>
Date:   Tue Dec 17 10:43:34 2024 +0200

    Update README.md

commit 4658a51ada13ab60824cdbc34d6a9a962ed3969b
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 10:40:16 2024 +0200

    README.md

commit 105331f53708988d278555a699ae15e7b471538c
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 10:37:45 2024 +0200

    README.md

commit 6edd66b0b2966368f55e98756a51c37226ba26db
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 10:16:37 2024 +0200

    changes staged and committed
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git status
On branch ft/team-page
nothing to commit, working tree clean
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git cherry-pick 6edd66b0b2966368f55e98756a51c37226ba26db
[ft/contact-page 7341601] changes staged and committed
 Date: Tue Dec 17 10:16:37 2024 +0200
 1 file changed, 1 insertion(+)
 create mode 100644 test_file
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git cherry-pick 9dab2564a4ddf2ec95e3d5aad7415ca7145fdc63
[ft/contact-page d70007e] Bundle 3, let's goo
 Date: Tue Dec 17 15:47:23 2024 +0200
 1 file changed, 11 insertions(+)
 create mode 100644 team.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ ls
about.html  home.html  README.md  service.html  team.html  test_file
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ rm -rf te
team.html  test_file
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ rm -rf test_file
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ ls
about.html  home.html  README.md  service.html  team.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git --add
unknown option: --add
usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           [--config-env=<name>=<envvar>] <command> [<args>]
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git add --all
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git commit -m "Okayy"
[ft/contact-page c9b2a39] Okayy
 1 file changed, 1 deletion(-)
 delete mode 100644 test_file
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git status
On branch ft/contact-page
nothing to commit, working tree clean
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push origin ft/contact-page
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 8 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (8/8), 889 bytes | 889.00 KiB/s, done.
Total 8 (delta 3), reused 1 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git status
On branch ft/contact-page
nothing to commit, working tree clean
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ ls
about.html  home.html  README.md  service.html  team.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ touch faq.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git add --all
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git commit -m "FAQ page added"
[ft/faq-page 3ec5fe0] FAQ page added
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 437 bytes | 437.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote:
To https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout ft/team-page
Switched to branch 'ft/team-page'
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git log
commit 9dab2564a4ddf2ec95e3d5aad7415ca7145fdc63 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:47:23 2024 +0200

    Bundle 3, let's goo

commit 5f7ff0f94a1a5bdc175efdfab48ec4753a5c8b39 (origin/ft/service-redesign, ft/service-redesign)
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:40:06 2024 +0200

    README.md

commit c3096e8345486a06127f5d437734095cd38eb15a
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:36:33 2024 +0200

    okay

commit da9b0d8c6862bd469ef217133fd05b053630860a
Merge: 1146a69 859f4be
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:33:06 2024 +0200

    almost done
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout ft/faq-page
Switched to branch 'ft/faq-page'
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git log
commit 3ec5fe03a73486d221a7b80e259283b4ce7ba78f (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 16:00:36 2024 +0200

    FAQ page added

commit c9b2a392f692669561ea6267cbfeffc1e4878c0c (origin/ft/contact-page, ft/contact-page)
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:57:14 2024 +0200

    Okayy

commit d70007e65436be6adeb71526d61fb45dcd953ed5
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:47:23 2024 +0200

    Bundle 3, let's goo

commit 7341601ea81e75379334f5fb85c26fe8e1e6eef9
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 10:16:37 2024 +0200

    changes staged and committed

commit 0d6c337925f6cf0a7089629d5bf1fa55b6c74b91 (origin/main, origin/HEAD, main)
Merge: eeb513f 5f7ff0f
Author: Nick-Lemy Niyigena Kayiranga <169042721+Nick-Lemy@users.noreply.github.com>
Date:   Tue Dec 17 15:42:18 2024 +0200

    Merge pull request #3 from Nick-Lemy/ft/service-redesign

    README.md

commit 5f7ff0f94a1a5bdc175efdfab48ec4753a5c8b39 (origin/ft/service-redesign, ft/service-re
design)
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:40:06 2024 +0200

    README.md

commit eeb513fb7e31c7a44d06e78f9a6efa22dc16069a
Merge: 859f4be c3096e8
Author: Nick-Lemy Niyigena Kayiranga <169042721+Nick-Lemy@users.noreply.github.com>
Date:   Tue Dec 17 15:37:27 2024 +0200

    Merge pull request #2 from Nick-Lemy/ft/service-redesign

    Update service.html

commit c3096e8345486a06127f5d437734095cd38eb15a
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:36:33 2024 +0200

    okay

commit da9b0d8c6862bd469ef217133fd05b053630860a
Merge: 1146a69 859f4be
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:33:06 2024 +0200

    almost done

commit 859f4bed40a4b4d9abab2e9e10164773ef93072d
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:14:42 2024 +0200

    service.html changed

commit 1146a69c27e960e617fe3621e7df93d4377fc292
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:07:28 2024 +0200

    Update service.html

commit c9b68baf8d69618bfa2f5e8646a539696f2a1a81
Merge: e7fff88 0bf5e00
Author: Nick-Lemy Niyigena Kayiranga <169042721+Nick-Lemy@users.noreply.github.com>
Date:   Tue Dec 17 14:37:37 2024 +0200

    Merge pull request #1 from Nick-Lemy/ft/bundle-2

    adding html pages

commit e7fff88384a2c8f4ca7d6495c75a1532ca35d2d4
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 14:36:43 2024 +0200

    ll

commit 0bf5e00b8df78a8d1662828b632e1c715f2d835b (origin/ft/bundle-2, ft/bundle-2)
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 14:32:55 2024 +0200

    Description added

commit fed067d37e6355850863328bc1f3936a5e1a5896
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 12:54:06 2024 +0200

    Service created

commit ee4277938cc511c5169b6532541e083f279be17d
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 12:43:21 2024 +0200

    !

commit 1c601d1534bde175ddc196b0d3667eae573ca980 (origin/dev, dev)
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 12:42:00 2024 +0200

    !

commit a31ca6eefa9d951662acdf3d4c32f445f0e508ba
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 12:39:15 2024 +0200

    !

commit 44dd93fa16d8f66c6a4c9922271aa0713b23804d
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 12:34:11 2024 +0200

    !

commit 9af481f67d2ce537cb1b31ec90d8093019f7c3c3
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 11:49:24 2024 +0200

    README.md updated for exercise 2 Bundle 1

commit eccf05cae84372ebbf344829efabe49589060b54
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 11:45:29 2024 +0200

    Changes committed and ready to be pushed

commit 0613e6aacf571633999d4efc1a022d5c22284eae
Author: Nick-Lemy Niyigena Kayiranga <169042721+Nick-Lemy@users.noreply.github.com>
Date:   Tue Dec 17 10:44:38 2024 +0200

    Update README.md

commit 1956995b24665d0d9498a3b34034d31905aa9e24
Author: Nick-Lemy Niyigena Kayiranga <169042721+Nick-Lemy@users.noreply.github.com>
Date:   Tue Dec 17 10:44:13 2024 +0200

    Update README.md

commit 0db4e20fe5b66cbc4148d9c38b12a7c786265f45
Author: Nick-Lemy Niyigena Kayiranga <169042721+Nick-Lemy@users.noreply.github.com>
Date:   Tue Dec 17 10:43:34 2024 +0200

    Update README.md

commit 4658a51ada13ab60824cdbc34d6a9a962ed3969b
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 10:40:16 2024 +0200

    README.md

commit 105331f53708988d278555a699ae15e7b471538c
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 10:37:45 2024 +0200

    README.md

commit 6edd66b0b2966368f55e98756a51c37226ba26db
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 10:16:37 2024 +0200

    changes staged and committed
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git log
commit 3ec5fe03a73486d221a7b80e259283b4ce7ba78f (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 16:00:36 2024 +0200

    FAQ page added

commit c9b2a392f692669561ea6267cbfeffc1e4878c0c (origin/ft/contact-page, ft/contact-page)
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:57:14 2024 +0200

    Okayy

commit d70007e65436be6adeb71526d61fb45dcd953ed5
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:47:23 2024 +0200

    Bundle 3, let's goo

commit 7341601ea81e75379334f5fb85c26fe8e1e6eef9
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 10:16:37 2024 +0200

    changes staged and committed

commit 0d6c337925f6cf0a7089629d5bf1fa55b6c74b91 (origin/main, origin/HEAD, main)
Merge: eeb513f 5f7ff0f
Author: Nick-Lemy Niyigena Kayiranga <169042721+Nick-Lemy@users.noreply.github.com>
Date:   Tue Dec 17 15:42:18 2024 +0200

    Merge pull request #3 from Nick-Lemy/ft/service-redesign

    README.md

commit 5f7ff0f94a1a5bdc175efdfab48ec4753a5c8b39 (origin/ft/service-redesign, ft/service-re
design)
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:40:06 2024 +0200

    README.md

commit eeb513fb7e31c7a44d06e78f9a6efa22dc16069a
Merge: 859f4be c3096e8
Author: Nick-Lemy Niyigena Kayiranga <169042721+Nick-Lemy@users.noreply.github.com>
Date:   Tue Dec 17 15:37:27 2024 +0200

    Merge pull request #2 from Nick-Lemy/ft/service-redesign

    Update service.html

commit c3096e8345486a06127f5d437734095cd38eb15a
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:36:33 2024 +0200

    okay

commit da9b0d8c6862bd469ef217133fd05b053630860a
Merge: 1146a69 859f4be
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:33:06 2024 +0200

    almost done

commit 859f4bed40a4b4d9abab2e9e10164773ef93072d
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:14:42 2024 +0200

    service.html changed

commit 1146a69c27e960e617fe3621e7df93d4377fc292
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:07:28 2024 +0200

    Update service.html

commit c9b68baf8d69618bfa2f5e8646a539696f2a1a81
Merge: e7fff88 0bf5e00
Author: Nick-Lemy Niyigena Kayiranga <169042721+Nick-Lemy@users.noreply.github.com>
Date:   Tue Dec 17 14:37:37 2024 +0200

    Merge pull request #1 from Nick-Lemy/ft/bundle-2

    adding html pages

commit e7fff88384a2c8f4ca7d6495c75a1532ca35d2d4
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 14:36:43 2024 +0200

    ll

commit 0bf5e00b8df78a8d1662828b632e1c715f2d835b (origin/ft/bundle-2, ft/bundle-2)
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 14:32:55 2024 +0200

    Description added

commit fed067d37e6355850863328bc1f3936a5e1a5896
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 12:54:06 2024 +0200

    Service created

commit ee4277938cc511c5169b6532541e083f279be17d
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 12:43:21 2024 +0200

    !

commit 1c601d1534bde175ddc196b0d3667eae573ca980 (origin/dev, dev)
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 12:42:00 2024 +0200

    !

commit a31ca6eefa9d951662acdf3d4c32f445f0e508ba
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 12:39:15 2024 +0200

    !

commit 44dd93fa16d8f66c6a4c9922271aa0713b23804d
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 12:34:11 2024 +0200

    !

commit 9af481f67d2ce537cb1b31ec90d8093019f7c3c3
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 11:49:24 2024 +0200

    README.md updated for exercise 2 Bundle 1

commit eccf05cae84372ebbf344829efabe49589060b54
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 11:45:29 2024 +0200

    Changes committed and ready to be pushed

commit 0613e6aacf571633999d4efc1a022d5c22284eae
Author: Nick-Lemy Niyigena Kayiranga <169042721+Nick-Lemy@users.noreply.github.com>
Date:   Tue Dec 17 10:44:38 2024 +0200

    Update README.md

commit 1956995b24665d0d9498a3b34034d31905aa9e24
Author: Nick-Lemy Niyigena Kayiranga <169042721+Nick-Lemy@users.noreply.github.com>
Date:   Tue Dec 17 10:44:13 2024 +0200

    Update README.md

commit 0db4e20fe5b66cbc4148d9c38b12a7c786265f45
Author: Nick-Lemy Niyigena Kayiranga <169042721+Nick-Lemy@users.noreply.github.com>
Date:   Tue Dec 17 10:43:34 2024 +0200

    Update README.md

commit 4658a51ada13ab60824cdbc34d6a9a962ed3969b
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 10:40:16 2024 +0200

    README.md

commit 105331f53708988d278555a699ae15e7b471538c
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 10:37:45 2024 +0200

    README.md

commit 6edd66b0b2966368f55e98756a51c37226ba26db
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 10:16:37 2024 +0200

    changes staged and committed
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout ft/team-page
Switched to branch 'ft/team-page'
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git log
commit 9dab2564a4ddf2ec95e3d5aad7415ca7145fdc63 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:47:23 2024 +0200

    Bundle 3, let's goo

commit 5f7ff0f94a1a5bdc175efdfab48ec4753a5c8b39 (origin/ft/service-redesign, ft/service-redesign)
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:40:06 2024 +0200

    README.md

commit c3096e8345486a06127f5d437734095cd38eb15a
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:36:33 2024 +0200

    okay

commit da9b0d8c6862bd469ef217133fd05b053630860a
Merge: 1146a69 859f4be
Author: Nick-Lemy <n.kayiranga@alustudent.com>
Date:   Tue Dec 17 15:33:06 2024 +0200

    almost done
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git revert 9dab2564a4ddf2ec95e3d5aad7415ca7145fdc63
[ft/team-page dd068c5] Revert "Bundle 3, let's goo"
 1 file changed, 11 deletions(-)
 delete mode 100644 team.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git add .
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git commit -m "hum"
On branch ft/team-page
nothing to commit, working tree clean
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push origin ft/team-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 265 bytes | 265.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
   9dab256..dd068c5  ft/team-page -> ft/team-page
```

### Exercise 2

```console
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout ft/faq-page
Already on 'ft/faq-page'
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ ls
about.html  faq.html  home.html  README.md  service.html  team.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git add --all
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git commit -m "some changes"
[main 5ce0e23] some changes
 1 file changed, 2 insertions(+), 2 deletions(-)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 306 bytes | 153.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
   4ea7f81..5ce0e23  main -> main
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout ft/home-page-rede
sign
Switched to branch 'ft/home-page-redesign'
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ ls
about.html  faq.html  home.html  README.md  service.html  team.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git add home.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git commit -m "home changed"
[ft/home-page-redesign 055fc8f] home changed
 1 file changed, 2 insertions(+), 2 deletions(-)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git status
On branch ft/home-page-redesign
nothing to commit, working tree clean
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push origin ft/home-page-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 304 bytes | 304.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote:
To https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$
```

## Bundle 4

### Exercise 1

```console
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 4 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git pull
Updating 5ce0e23..e611661
Fast-forward
 README.md | 63 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 home.html |  4 ++--
 2 files changed, 65 insertions(+), 2 deletions(-)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git remote add git-copy https://github.com/Nick-Lemy/Bundle-4-Exercise-1.git
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git remote
git-copy
origin
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git add -all
error: did you mean `--all` (with two dashes)?
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git add --all
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git commit -m "home page updated"
[main dc04489] home page updated
 1 file changed, 2 insertions(+), 2 deletions(-)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 306 bytes | 306.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
   e611661..dc04489  main -> main
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push git-copy main
Enumerating objects: 88, done.
Counting objects: 100% (88/88), done.
Delta compression using up to 8 threads
Compressing objects: 100% (77/77), done.
Writing objects: 100% (88/88), 24.03 KiB | 534.00 KiB/s, done.
Total 88 (delta 32), reused 16 (delta 3), pack-reused 0
remote: Resolving deltas: 100% (32/32), done.
To https://github.com/Nick-Lemy/Bundle-4-Exercise-1.git
 * [new branch]      main -> main
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$
```

### Exercise 2

```console
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout -b ft
/footer
Switched to a new branch 'ft/footer'
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git add --all
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git commit -m "ft/footer created"
[ft/footer 326190b] ft/footer created
 1 file changed, 1 insertion(+), 1 deletion(-)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git add --all
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git commit -m "about modified"
[ft/footer 0751a90] about modified
 1 file changed, 1 insertion(+), 1 deletion(-)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push
fatal: The current branch ft/footer has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/footer

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push --set-upstream origin ft/footer
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 616 bytes | 308.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions/pull/new/ft/footer
remote:
To https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/footer -> ft/footer
branch 'ft/footer' set up to track 'origin/ft/footer'.
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git merge --squashing ft/footer
error: unknown option `squashing'
usage: git merge [<options>] [<commit>...]
   or: git merge --abort
   or: git merge --continue

    -n                    do not show a diffstat at the end of the merge
    --[no-]stat           show a diffstat at the end of the merge
    --[no-]summary        (synonym to --stat)
    --[no-]log[=<n>]      add (at most <n>) entries from shortlog to merge commit message
    --[no-]squash         create a single commit instead of doing a merge
    --[no-]commit         perform a commit if the merge succeeds (default)
    -e, --[no-]edit       edit message before committing
    --[no-]cleanup <mode> how to strip spaces and #comments from message
    --[no-]ff             allow fast-forward (default)
    --ff-only             abort if fast-forward is not possible
    --[no-]rerere-autoupdate
                          update the index with reused conflict resolution if possible
    --[no-]verify-signatures
                          verify that the named commit has a valid GPG signature
    -s, --[no-]strategy <strategy>
                          merge strategy to use
    -X, --[no-]strategy-option <option=value>
                          option for selected merge strategy
    -m, --[no-]message <message>
                          merge commit message (for a non-fast-forward merge)
    -F, --file <path>     read message from file
    --[no-]into-name <name>
                          use <name> instead of the real target
    -v, --[no-]verbose    be more verbose
    -q, --[no-]quiet      be more quiet
    --[no-]abort          abort the current in-progress merge
    --[no-]quit           --abort but leave index and working tree alone
    --[no-]continue       continue the current in-progress merge
    --[no-]allow-unrelated-histories
                          allow merging unrelated histories
    --[no-]progress       force progress reporting
    -S, --[no-]gpg-sign[=<key-id>]
                          GPG sign commit
    --[no-]autostash      automatically stash/stash pop before and after
    --[no-]overwrite-ignore
                          update ignored files (default)
    --[no-]signoff        add a Signed-off-by trailer
    --no-verify           bypass pre-merge-commit and commit-msg hooks
    --verify              opposite of --no-verify

zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git merge --squash ft/footer
Updating ff2a4ed..0751a90
Fast-forward
Squash commit -- not updating HEAD
 about.html | 4 ++--
 1 file changed, 2 insertions(+), 2 deletions(-)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git status
On branch ft/squashing
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   about.html

zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git commit -m "footer changes squashing"
[ft/squashing 7f51093] footer changes squashing
 1 file changed, 2 insertions(+), 2 deletions(-)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push
fatal: The current branch ft/squashing has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/squashing

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push --set-upstream origin ft/squashing
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 339 bytes | 169.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions/pull/new/ft/squashing
remote:
To https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/squashing -> ft/squashing
branch 'ft/squashing' set up to track 'origin/ft/squashing'.
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$
```

## Bundle 5

### Exercise 1

```console
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 3 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git pull
Updating ff2a4ed..7808315
Fast-forward
 README.md  | 136 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 about.html |   4 +-
 2 files changed, 138 insertions(+), 2 deletions(-)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ mv home.html index.html
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git add --all
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git commit -m "home.html to index.html"
[main ced1869] home.html to index.html
 1 file changed, 0 insertions(+), 0 deletions(-)
 rename home.html => index.html (100%)
zkaynl7@zkaynl7-ThinkPad-T480:~/Gym-Git-Exercise-Solutions$ git push origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 245 bytes | 245.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Nick-Lemy/Gym-Git-Exercise-Solutions.git
   7808315..ced1869  main -> main
```

#### Exercise 2

```console
zkaynl7@zkaynl7-ThinkPad-T480:~$ git clone https://[can't show my tokken]@github.com/Nick-Lemy/git-cafe-exercise.git
Cloning into 'git-cafe-exercise'...
remote: Enumerating objects: 107, done.
remote: Counting objects: 100% (14/14), done.
remote: Compressing objects: 100% (10/10), done.
remote: Total 107 (delta 5), reused 4 (delta 4), pack-reused 93 (from 1)
Receiving objects: 100% (107/107), 1.95 MiB | 629.00 KiB/s, done.
Resolving deltas: 100% (5/5), done.
zkaynl7@zkaynl7-ThinkPad-T480:~$ cd git-cafe-exercise/
zkaynl7@zkaynl7-ThinkPad-T480:~/git-cafe-exercise$ code .
zkaynl7@zkaynl7-ThinkPad-T480:~/git-cafe-exercise$ git add --all
zkaynl7@zkaynl7-ThinkPad-T480:~/git-cafe-exercise$ git commit -m "bundle 5 ex 2"
[main a5ec8ae] bundle 5 ex 2
 1 file changed, 399 insertions(+), 239 deletions(-)
zkaynl7@zkaynl7-ThinkPad-T480:~/git-cafe-exercise$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.57 KiB | 401.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Nick-Lemy/git-cafe-exercise.git
   d1d3f9c..a5ec8ae  main -> main
zkaynl7@zkaynl7-ThinkPad-T480:~/git-cafe-exercise$
```
