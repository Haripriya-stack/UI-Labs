# UI-Labs
This project was built while learning HTML, CSS, and JavaScript by following an online tutorial.
I implemented the project hands-on to understand layout, DOM manipulation, and basic interactivity

# GIT:
Git Bash provides:

A Linux-like terminal

Inside Windows

Optimized for Git

This makes Git behave the same way across all systems.
USER@DESKTOP-F4M17SG MINGW64 ~
$ This makes Git behave the same way across all systems.
bash: This: command not found

USER@DESKTOP-F4M17SG MINGW64 ~
$ git clone https://github.com/Haripriya-stack/UI-Labs.git
Cloning into 'UI-Labs'...
remote: Enumerating objects: 15, done.
remote: Counting objects: 100% (15/15), done.
remote: Compressing objects: 100% (13/13), done.
remote: Total 15 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (15/15), 6.30 KiB | 184.00 KiB/s, done.
Resolving deltas: 100% (3/3), done.

USER@DESKTOP-F4M17SG MINGW64 ~
$ git checkout local
fatal: not a git repository (or any of the parent directories): .git

USER@DESKTOP-F4M17SG MINGW64 ~
$ git checkout main
fatal: not a git repository (or any of the parent directories): .git

USER@DESKTOP-F4M17SG MINGW64 ~
$ cd UI-Labs

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (main)
$ git checkout local
error: pathspec 'local' did not match any file(s) known to git

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (main)
$ git checkout Local
Switched to a new branch 'Local'
branch 'Local' set up to track 'origin/Local'.

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (Local)
$ git status
On branch Local
Your branch is up to date with 'origin/Local'.

nothing to commit, working tree clean

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (Local)
$ git init
Reinitialized existing Git repository in C:/Users/USER/UI-Labs/.git/

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (Local)
$ echo "pushing from laptop to github" >> "NewFileFromLaptop"

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (Local)
$ git status
On branch Local
Your branch is up to date with 'origin/Local'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        NewFileFromLaptop.txt

nothing added to commit but untracked files present (use "git add" to track)

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (Local)
$ git add  NewFileFromLaptop.txt
warning: in the working copy of 'NewFileFromLaptop.txt', LF will be replaced by CRLF the next time Git touches it

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (Local)
$ git commit "pushfromlaptop"
error: pathspec 'pushfromlaptop' did not match any file(s) known to git

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (Local)
$ git commit -m "pushfromlaptop"
[Local 44dd63f] pushfromlaptop
 1 file changed, 1 insertion(+)
 create mode 100644 NewFileFromLaptop.txt

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (Local)
$ git push origin Local
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 320 bytes | 160.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Haripriya-stack/UI-Labs.git
   c1a24bc..44dd63f  Local -> Local

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (Local)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (main)
$ git pull origin main
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (1/1), done.
remote: Total 3 (delta 1), reused 2 (delta 1), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 987 bytes | 49.00 KiB/s, done.
From https://github.com/Haripriya-stack/UI-Labs
 * branch            main       -> FETCH_HEAD
   4996e70..102bda3  main       -> origin/main
Updating 4996e70..102bda3
Fast-forward
 NewFileFromLaptop.txt | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 NewFileFromLaptop.txt

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (main)
$ git checkout local
Switched to branch 'local'

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (local)
$ git credential-manager version
'version' was not matched. Did you mean one of the following?
--version
Required command was not provided.
Unrecognized command or argument 'version'.

Description:

Usage:
  git-credential-manager [command] [options]

Options:
  --no-ui         Do not use graphical user interface prompts
  --version       Show version information
  -?, -h, --help  Show help and usage information

Commands:
  get          [Git] Return a stored credential
  store        [Git] Store a credential
  erase        [Git] Erase a stored credential
  configure    Configure Git Credential Manager as the Git credential helper
  unconfigure  Unconfigure Git Credential Manager as the Git credential helper
  diagnose     Run diagnostics and gather logs to diagnose problems with Git Credential Manager
  azure-repos  Commands for interacting with the Azure Repos host provider
  github       Commands for interacting with the GitHub host provider


USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (local)
$ git credential-manager --version
2.5.0+d34930736e131ad80e5690e5634ced1808aff3e2

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (local)
$ git remote set-url origin https://tk@github.com/username/repo.git

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (local)
$ git remote -v
origin  https://tk@github.com/username/repo.git (fetch)
origin  https://tk@github.com/username/repo.git (push)

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (local)
$ echo "testign after pattoken" >> "AnotherFile.txt"

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (local)
$ git add .
warning: in the working copy of 'AnotherFile.txt', LF will be replaced by CRLF the next time Git touches it

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (local)
$ git commit -m "FilePushTestAfterPAT"
[local 74e8cd7] FilePushTestAfterPAT
 1 file changed, 1 insertion(+)
 create mode 100644 AnotherFile.txt

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (local)
$ git push origin Local
remote: Repository not found.
fatal: repository 'https://github.com/username/repo.git/' not found

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (local)
$ ^C

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (local)
$ git remote set-url origin https://tk@github.com/Haripriya-stack/UI-Labs.git

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (local)
$ git remote -v
origin  https://tk@github.com/Haripriya-stack/UI-Labs.git (fetch)
origin  https://tk@github.com/Haripriya-stack/UI-Labs.git (push)

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (local)
$ git push origin Local
fatal: Local cannot be resolved to branch

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (local)
$ git config --global credential.helper manager

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (local)
$ git push origin Local
fatal: Local cannot be resolved to branch

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (local)
$ git push origin local
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 316 bytes | 316.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'local' on GitHub by visiting:
remote:      https://github.com/Haripriya-stack/UI-Labs/pull/new/local
remote:
To https://github.com/Haripriya-stack/UI-Labs.git
 * [new branch]      local -> local

USER@DESKTOP-F4M17SG MINGW64 ~/UI-Labs (local)
$
