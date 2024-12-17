# Gym-Git-Exercise-Solutions

## Bundle 1

### Exercise 1
```bash
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
zkaynl7@zkaynl7-ThinkPad-T480:~/Documents/git-bundle/exercise-1$ git remote add origin main https://[sorry can\'t let u see my token]@github.com/Nick-Lemy/Gym-Git-Exercise-Solutions
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
