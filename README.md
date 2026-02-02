# gitTest
62-2


Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode
$ git status
fatal: not a git repository (or any of the parent directories): .git

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode
$ git init
Initialized empty Git repository in C:/Users/Administrator/Desktop/gitcode/.git/

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        hello.txt

nothing added to commit but untracked files present (use "git add" to track)

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (master)
$ git add hello.txt

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (master)
$ git add .

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (master)
$ git commit -m "first file"
[master (root-commit) 2b78e9d] first file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 hello.txt

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (master)
$ git log
commit 2b78e9df0f599b93c452d35e109252b28f516b36 (HEAD -> master)
Author: city62-2 <516212139@qq.com>
Date:   Mon Feb 2 13:52:34 2026 +0800

    first file

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (master)
$ git branch
* master

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (master)
$ git branch dev

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (master)
$ git checkout dev
Switched to branch 'dev'

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (dev)
$ git branch -d dev
error: cannot delete branch 'dev' used by worktree at 'C:/Users/Administrator/Desktop/gitcode'

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (dev)
$ ssh
usage: ssh [-46AaCfGgKkMNnqsTtVvXxYy] [-B bind_interface] [-b bind_address]
           [-c cipher_spec] [-D [bind_address:]port] [-E log_file]
           [-e escape_char] [-F configfile] [-I pkcs11] [-i identity_file]
           [-J destination] [-L address] [-l login_name] [-m mac_spec]
           [-O ctl_cmd] [-o option] [-P tag] [-p port] [-R address]
           [-S ctl_path] [-W host:port] [-w local_tun[:remote_tun]]
           destination [command [argument ...]]
       ssh [-Q query_option]

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (dev)
$ ssh-keygen -t rsa
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/Administrator/.ssh/id_rsa):
Created directory '/c/Users/Administrator/.ssh'.
Enter passphrase for "/c/Users/Administrator/.ssh/id_rsa" (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/Administrator/.ssh/id_rsa
Your public key has been saved in /c/Users/Administrator/.ssh/id_rsa.pub
The key fingerprint is:
SHA256:tUPO5TTxb0nWqgR6NLR9O0AW0mJtOfU4ce4tHV/Z8ag Administrator@CHINAMI-VED2E15
The key's randomart image is:
+---[RSA 3072]----+
|          oo=+o..|
|         .o**o B*|
|         .Bo*.*=B|
|         B B =oB*|
|        S * E =.B|
|         . o . + |
|            .    |
|                 |
|                 |
+----[SHA256]-----+

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (dev)
$ ssh -T git@github.com
The authenticity of host 'github.com (20.205.243.166)' can't be established.
ED25519 key fingerprint is: SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added 'github.com' (ED25519) to the list of known hosts.
Hi city666668-creator! You've successfully authenticated, but GitHub does not provide shell access.

------------------------------------------------------------------------------------------****
Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (dev)
$ https://github.com/city666668-creator/gitTest.git
bash: https://github.com/city666668-creator/gitTest.git: No such file or directory

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (dev)
$ git status
On branch dev
nothing to commit, working tree clean

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (dev)
$ git add .

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (dev)
$ git commit -m "gitTset first file"
On branch dev
nothing to commit, working tree clean

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (dev)
$ git remote

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (dev)
$ git push origin main
error: src refspec main does not match any
error: failed to push some refs to 'origin'

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (dev)
$ git remote add gittest git@github.com:MmlSQ/gitTest.git

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (dev)
$ git pull gittest HEAD
ERROR: Repository not found.
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (dev)
$ git add .
git commit -m "modify README.md"
On branch dev
nothing to commit, working tree clean

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (dev)
$ git push gittest master
ERROR: Repository not found.
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

Administrator@CHINAMI-VED2E15 MINGW64 ~/Desktop/gitcode (dev)
$

62-2
