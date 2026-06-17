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

```