## Bandle1-exercises1
```bash
PS C:\Users\Malaika\basic-git> git init
Initialized empty Git repository in C:/Users/Malaika/basic-git/.git/
PS C:\Users\Malaika\basic-git> 
PS C:\Users\Malaika\basic-git> git branch --show-current
master
PS C:\Users\Malaika\basic-git> git branch -M main
PS C:\Users\Malaika\basic-git> git branch --show-current
main
PS C:\Users\Malaika\basic-git> git commit -m "README file first updats" 
[main (root-commit) 7265f48] README file first updats
 1 file changed, 7 insertions(+)
PS C:\Users\Malaika\basic-git> git remote add origin https://github.com/GODisALL-FriendOfJesus/basic-git.git
PS C:\Users\Malaika\basic-git> git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking

Enumerating objects: 3, done.
Delta compression using up to 4 threads
Writing objects: 100% (3/3), 364 bytes | 121.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/GODisALL-FriendOfJesus/basic-git.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
PS C:\Users\Malaika\basic-git> git checkout -b dev
Switched to a new branch 'dev'
PS C:\Users\Malaika\basic-git> git checkout -b test
Switched to a new branch 'test'
PS C:\Users\Malaika\basic-git> git checkout dev
Switched to branch 'dev'
PS C:\Users\Malaika\basic-git> git branch -d test
Deleted branch test (was 7265f48).

##Exercise2
PS C:\Users\Malaika\basic-git> git checkout -b test
Switched to a new branch 'test'
PS C:\Users\Malaika\basic-git> git checkout dev
Switched to branch 'dev'
PS C:\Users\Malaika\basic-git> git branch -d test
Deleted branch test (was 7265f48).
PS C:\Users\Malaika\basic-git> git add .
[dev cd00e60] second changes exercise1 bandle1 done
 1 file changed, 32 insertions(+)
PS C:\Users\Malaika\basic-git> git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\Malaika\basic-git>  git push --set-upstream origin dev
Enumerating objects: 5, done.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 896 bytes | 896.00 KiB/s, done.
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/GODisALL-FriendOfJesus/basic-git/pull/new/dev
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.
PS C:\Users\Malaika\basic-git> git stashxercise1 bandle1 done
PS C:\Users\Malaika\basic-git> git add About.html
PS C:\Users\Malaika\basic-git> git stashxercise1 bandle1 done
PS C:\Users\Malaika\basic-git> git add Team.html
PS C:\Users\Malaika\basic-git> git stash
Saved working directory and index state WIP on dev: cd00e60 second changes exercise1 bandle1 done
PS C:\Users\Malaika\basic-git> git stashlist 
PS C:\Users\Malaika\basic-git> git stash list
stash@{0}: WIP on dev: cd00e60 second changes exercise1 bandle1 done
stash@{1}: WIP on dev: cd00e60 second changes exercise1 bandle1 done
stash@{2}: WIP on dev: cd00e60 second changes exercise1 bandle1 done
PS C:\Users\Malaika\basic-git> git stash pop stash@{0}
error: unknown switch `e'

    -q, --[no-]quiet      be quiet, only report errors
    --[no-]index          attempt to recreate the index

PS C:\Users\Malaika\basic-git> git stash pop stash@{0}
error: unknown switch `e'
usage: git stash pop [--index] [-q | --quiet] [<stash>]


PS C:\Users\Malaika\basic-git> git stash pop
Your branch is up to date with 'origin/dev'.

Changes to be committed:
        new file:   Team.html

Dropped refs/stash@{0} (be1a331528eafbcc5f11c6f33ce09160a67fd509)
PS C:\Users\Malaika\basic-git> git add Team.html
PS C:\Users\Malaika\basic-git> git stash
Saved working directory and index state WIP on dev: cd00e60 second changes exercise1 bandle1 done
PS C:\Users\Malaika\basic-git> git stash list
stash@{1}: WIP on dev: cd00e60 second changes exercise1 bandle1 done
stash@{2}: WIP on dev: cd00e60 second changes exercise1 bandle1 done
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   Home.html

Dropped refs/stash@{2} (92e2d2cb4817fa91ec97ebd44b235e1c56886b39)
PS C:\Users\Malaika\basic-git> git stash list
stash@{1}: WIP on dev: cd00e60 second changes exercise1 bandle1 done
PS C:\Users\Malaika\basic-git> git stash pop 1
On branch dev
Your branch is up to date with 'origin/dev'.
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   About.html
        new file:   Home.html

Dropped refs/stash@{1} (7291f26896cac3a22459f9076e1a9b177d4e6da5)
PS C:\Users\Malaika\basic-git> git commit -m "home and about page are done"
[dev 6ee5ef5] home and about page are done
 2 files changed, 22 insertions(+)
 create mode 100644 Home.html
PS C:\Users\Malaika\basic-git> git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 539 bytes | 41.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/GODisALL-FriendOfJesus/basic-git.git
   cd00e60..6ee5ef5  dev -> dev
PS C:\Users\Malaika\basic-git> git stash pop
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   Team.html

Dropped refs/stash@{0} (528d7a4516967b5e939a48ad570aea8f11d4c43c)
PS C:\Users\Malaika\basic-git> git  reset --hard head
HEAD is now at 6ee5ef5 home and about page are done
PS C:\Users\Malaika\basic-git> 



```
## BANDLE 2
```bash 
##exercise1

PS C:\Users\Malaika\basic-git> git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'
PS C:\Users\Malaika\basic-git> git add .                        
PS C:\Users\Malaika\basic-git> git commit -m "service page is done"
[ft/bundle-2 02cfc51] service page is done
 1 file changed, 12 insertions(+)
 create mode 100644 services.html
PS C:\Users\Malaika\basic-git> git push origin ft/bundle-2
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 481 bytes | 43.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.iting:
remote:      https://github.com/GODisALL-FriendOfJesus/basic-git
remote: 
To https://github.com/GODisALL-FriendOfJesus/basic-git.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
PS C:\Users\Malaika\basic-git> git status
On branch ft/bundle-2
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\Malaika\basic-git> git add services.html
PS C:\Users\Malaika\basic-git> git commit -m "service page is ready now"
[ft/bundle-2 cc307e7] service page is ready now
 1 file changed, 1 insertion(+), 1 deletion(-)
PS C:\Users\Malaika\basic-git> git push origin ft/bundle-2
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 341 bytes | 341.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/GODisALL-FriendOfJesus/basic-git.git
   02cfc51..cc307e7  ft/bundle-2 -> ft/bundle-2
PS C:\Users\Malaika\basic-git>


```