# Lab6 : _Lecture Note_
##### 202334470_ParkSuBin

## Changes vs. Snapshots
----
#### changes
: Only the changed parts are recorded and added to the base when fetched.

#### snapshots
:The changed version itself (= full information of the file) is recorded.

## Local, Centralized, and Distributed Version Control
----
#### local
: It's only fixed in a personal computer.

#### centralized
:A central server exists and versions are recorded on that central server.

#### distributed
:A central server exists and versions are recorded on that central server, but copies of the versions are stored on the personal computer.
\+ When the central server goes down or is damaged, it can be recovered because the copy was stored on the personal computer.

## Three Stated in Git
----
: Git is made up of Modified, Staged, and Committded.

## Git config: First-time setup
----
* Git configurations are stored in three levels:
(1) System level: --system option. Affects all uses and repositories on the system (administrative).
(2) Global (user) level: global option. Affects all repositories of a current user.
(3) Local level: --local option. Specific to the current repository.
* Each level overrides values in the previous level: system -> global -> local

## Modified
----
#### $ git init
: It runs in the directory, resulting in a subdirectory called git.

#### $ git status
: Indicates the status of the current git.

## Modified
----
#### $ git add [file_name]
: Commands used when you want to upload a particular file to the staging area

#### $ git add .
: Command to git add all files currently in the directory

#### $ git rm -cached [file_name]
: It's one of the ways to un-staging again.

#### history_filename
: You can have the files you want to ignore.

## Commit
----
#### $ git commit -m "commit message"
: It's a command to commit. You can write a message explaining the git in the commit massage.

#### $ git log
: You can check what you have committed to so far.