# opensource
## 2024-2 semester
### lab7
# lee. chaehyun

chyom@chae_ MINGW64 ~/oss (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        end

nothing added to commit but untracked files present (use "git add" to track)

chyom@chae_ MINGW64 ~/oss (main)
$ git add <assessment.txt>
bash: syntax error near unexpected token `newline'

chyom@chae_ MINGW64 ~/oss (main)
$ git add assessment.txt
fatal: pathspec 'assessment.txt' did not match any files

chyom@chae_ MINGW64 ~/oss (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        "Lab3_202031881_Leechaehyun(\354\235\264\354\261\204\355\230\204).md"
        assessment.txt
        end

nothing added to commit but untracked files present (use "git add" to track)

chyom@chae_ MINGW64 ~/oss (main)
$ git add assessment.txt

chyom@chae_ MINGW64 ~/oss (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   assessment.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        "Lab3_202031881_Leechaehyun(\354\235\264\354\261\204\355\230\204).md"
        end


chyom@chae_ MINGW64 ~/oss (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   assessment.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        LAB5.txt
        "Lab3_202031881_Leechaehyun(\354\235\264\354\261\204\355\230\204).md"
        end


chyom@chae_ MINGW64 ~/oss (main)
$ git add .
warning: in the working copy of 'Lab3_202031881_Leechaehyun(이채현).md', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'end', LF will be replaced by CRLF the next time Git touches it

chyom@chae_ MINGW64 ~/oss (main)
$ git add LAB5.txt

chyom@chae_ MINGW64 ~/oss (main)
$ git log
fatal: your current branch 'main' does not have any commits yet

chyom@chae_ MINGW64 ~/oss (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   LAB5.txt
        new file:   "Lab3_202031881_Leechaehyun(\354\235\264\354\261\204\355\230\204).md"
        new file:   assessment.txt
        new file:   end


chyom@chae_ MINGW64 ~/oss (main)
$ cat LAB5.txt
LAB5
 Output & Input
2. Pipelines ( | )
3. File Permissions
4. Superuser Commands
5. Searching Text with grep
Standard Output ( > ): Saves the output of a command to a file
Append Output ( >> ): Adds output to an existing file
Standard Input ( < ): Takes input from a file
Using Pipe: Passes the output of one command as input to another command.
cat file.txt | grep "keyword" : Displays the contents of file.txt and
searches for keyword
Changing file permissions: Use chmod to set the read, write, and execute permissions
of a file.
chmod 644 example.txt : Owner has read and write permissions, while the group
and others have read-only permissions.
chmod 755 script.sh : The owner has read, write, and execute permissions, while
the group and others have read and execute permissions
Executing Commands with Superuser Privileges: Use sudo to execute commands
that require administrative rights.
Using the grep Command: Searches for specific text in files.
grep "error" log.txt : Searches for lines containing "error" in the log.txt file
chyom@chae_ MINGW64 ~/oss (main)
$ git add README.md
fatal: pathspec 'README.md' did not match any files

chyom@chae_ MINGW64 ~/oss (main)
$ remote add origin git@github.com:chaechaecherry/gitpractice-7-.git
bash: remote: command not found

chyom@chae_ MINGW64 ~/oss (main)
$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'origin'

chyom@chae_ MINGW64 ~/oss (main)
$ git remote -v

chyom@chae_ MINGW64 ~/oss (main)
$ git remote add origin https://github.com/chaechaecherry/gitpractice-7-.git

chyom@chae_ MINGW64 ~/oss (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   LAB5.txt
        new file:   "Lab3_202031881_Leechaehyun(\354\235\264\354\261\204\355\230\204).md"
        new file:   assessment.txt
        new file:   end


chyom@chae_ MINGW64 ~/oss (main)
$ git remote -v
origin  https://github.com/chaechaecherry/gitpractice-7-.git (fetch)
origin  https://github.com/chaechaecherry/gitpractice-7-.git (push)

chyom@chae_ MINGW64 ~/oss (main)
$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/chaechaecherry/gitpractice-7-.git'

chyom@chae_ MINGW64 ~/oss (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   LAB5.txt
        new file:   "Lab3_202031881_Leechaehyun(\354\235\264\354\261\204\355\230\204).md"
        new file:   assessment.txt
        new file:   end


chyom@chae_ MINGW64 ~/oss (main)
$ git pussh -u origin main
git: 'pussh' is not a git command. See 'git --help'.

The most similar command is
        push

chyom@chae_ MINGW64 ~/oss (main)
$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/chaechaecherry/gitpractice-7-.git'

chyom@chae_ MINGW64 ~/oss (main)
$ git commit -m 'commit_message'
[main (root-commit) a357148] commit_message
 4 files changed, 121 insertions(+)
 create mode 100644 LAB5.txt
 create mode 100644 "Lab3_202031881_Leechaehyun(\354\235\264\354\261\204\355\230\204).md"
 create mode 100644 assessment.txt
 create mode 100644 end

chyom@chae_ MINGW64 ~/oss (main)
$ git push -u origin main
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/chaechaecherry/gitpractice-7-.git/'

$ git log
commit a35714876edd40128c661b3ae93f32d7a9cd6a7e (HEAD -> main)
Author: Chaehyun,Lee <cchae010912@gachon.ac.kr>
Date:   Sat Oct 19 22:39:16 2024 +0900

    commit_message

chyom@chae_ MINGW64 ~/oss (main)
$ git commit -m "initial commit"
On branch main
nothing to commit, working tree clean

chyom@chae_ MINGW64 ~/oss (main)
$ git add README.md
fatal: pathspec 'README.md' did not match any files

chyom@chae_ MINGW64 ~/oss (main)
$ git add LAB5.txt

chyom@chae_ MINGW64 ~/oss (main)
$ git status
On branch main
nothing to commit, working tree clean

chyom@chae_ MINGW64 ~/oss (main)
$ git add .

chyom@chae_ MINGW64 ~/oss (main)
$ git status
On branch main
nothing to commit, working tree clean

chyom@chae_ MINGW64 ~/oss (main)
$ git remote add origin https://github.com/chaechaecherry/gitpractice-7-
error: remote origin already exists.

chyom@chae_ MINGW64 ~/oss (main)
$ cat LAB%.txt
cat: LAB%.txt: No such file or directory

chyom@chae_ MINGW64 ~/oss (main)
$ cat LAB5.txt
LAB5
 Output & Input
2. Pipelines ( | )
3. File Permissions
4. Superuser Commands
5. Searching Text with grep
Standard Output ( > ): Saves the output of a command to a file
Append Output ( >> ): Adds output to an existing file
Standard Input ( < ): Takes input from a file
Using Pipe: Passes the output of one command as input to another command.
cat file.txt | grep "keyword" : Displays the contents of file.txt and
searches for keyword
Changing file permissions: Use chmod to set the read, write, and execute permissions
of a file.
chmod 644 example.txt : Owner has read and write permissions, while the group
and others have read-only permissions.
chmod 755 script.sh : The owner has read, write, and execute permissions, while
the group and others have read and execute permissions
Executing Commands with Superuser Privileges: Use sudo to execute commands
that require administrative rights.
Using the grep Command: Searches for specific text in files.
grep "error" log.txt : Searches for lines containing "error" in the log.txt file
chyom@chae_ MINGW64 ~/oss (main)
$ git remote -v
origin  https://github.com/chaechaecherry/gitpractice-7-.git (fetch)
origin  https://github.com/chaechaecherry/gitpractice-7-.git (push)

chyom@chae_ MINGW64 ~/oss (main)
$ git push -u origin main
To https://github.com/chaechaecherry/gitpractice-7-.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/chaechaecherry/gitpractice-7-.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

chyom@chae_ MINGW64 ~/oss (main)
$ git commit -m
error: switch `m' requires a value

chyom@chae_ MINGW64 ~/oss (main)
$ git pull origin master
fatal: couldn't find remote ref master

chyom@chae_ MINGW64 ~/oss (main)
$ git pull origin main
remote: Enumerating objects: 12, done.
remote: Counting objects: 100% (12/12), done.
remote: Compressing objects: 100% (7/7), done.
remote: Total 12 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (12/12), 4.31 KiB | 80.00 KiB/s, done.
From https://github.com/chaechaecherry/gitpractice-7-
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
fatal: refusing to merge unrelated histories

chyom@chae_ MINGW64 ~/oss (main)
$ git status
On branch main
nothing to commit, working tree clean

chyom@chae_ MINGW64 ~/oss (main)
$ git commit -m "git practice"
On branch main
nothing to commit, working tree clean

chyom@chae_ MINGW64 ~/oss (main)
$ git push -u origin main
To https://github.com/chaechaecherry/gitpractice-7-.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/chaechaecherry/gitpractice-7-.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. If you want to integrate the remote changes,
hint: use 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

chyom@chae_ MINGW64 ~/oss (main)
$ ^C

chyom@chae_ MINGW64 ~/oss (main)
$ git pull
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> main


chyom@chae_ MINGW64 ~/oss (main)
$ git push -u origin main
To https://github.com/chaechaecherry/gitpractice-7-.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/chaechaecherry/gitpractice-7-.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. If you want to integrate the remote changes,
hint: use 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

chyom@chae_ MINGW64 ~/oss (main)
$ ^C

chyom@chae_ MINGW64 ~/oss (main)
$ git remote set-url origin http://ghp_U48Kn3x@github.com/chaechaecherry/gitpractice-7-

chyom@chae_ MINGW64 ~/oss (main)
$ git status
On branch main
nothing to commit, working tree clean

chyom@chae_ MINGW64 ~/oss (main)
$ git push -u origin main
warning: redirecting to https://github.com/chaechaecherry/gitpractice-7-/
To http://github.com/chaechaecherry/gitpractice-7-
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'http://github.com/chaechaecherry/gitpractice-7-'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. If you want to integrate the remote changes,
hint: use 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

chyom@chae_ MINGW64 ~/oss (main)
$ git push -u origin +main
warning: redirecting to https://github.com/chaechaecherry/gitpractice-7-/
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 2.50 KiB | 2.50 MiB/s, done.
Total 6 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To http://github.com/chaechaecherry/gitpractice-7-
 + 961df03...a357148 main -> main (forced update)
branch 'main' set up to track 'origin/main'.

chyom@chae_ MINGW64 ~/oss (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

chyom@chae_ MINGW64 ~/oss (main)
$ git add README.md
fatal: pathspec 'README.md' did not match any files

chyom@chae_ MINGW64 ~/oss (main)
$ git add gitignore.txt

chyom@chae_ MINGW64 ~/oss (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   gitignore.txt


chyom@chae_ MINGW64 ~/oss (main)
$ git commit -m " ignore file "
[main a84dadf]  ignore file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 gitignore.txt

chyom@chae_ MINGW64 ~/oss (main)
$ git log
commit a84dadf6cb4a0f16988c55fa046111ca9ec04072 (HEAD -> main)
Author: Chaehyun,Lee <cchae010912@gachon.ac.kr>
Date:   Sat Oct 19 23:42:37 2024 +0900

     ignore file

commit a357djfskfljsdfjsdkfjskdfjsdkfjw14876(origin/main)
Author: Chaehyun,Lee <cchae010912@gachon.ac.kr>
Date:   Sat Oct 19 22:39:16 2024 +0900

    commit_message

chyom@chae_ MINGW64 ~/oss (main)
$ git push-u origin +main
git: 'push-u' is not a git command. See 'git --help'.

chyom@chae_ MINGW64 ~/oss (main)
$ git push -u origin +main
warning: redirecting to https://github.com/chaechaecherry/gitpractice-7-/
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 8 threads
Compressing objects: 100% (8/8), done.
Writing objects: 100% (9/9), 2.72 KiB | 1.36 MiB/s, done.
Total 9 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
To http://github.com/chaechaecherry/gitpractice-7-
 + 1c0e3cb...a84dadf main -> main (forced update)
branch 'main' set up to track 'origin/main'.

chyom@chae_ MINGW64 ~/oss (main)
$
