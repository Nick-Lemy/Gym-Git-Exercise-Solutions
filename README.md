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
