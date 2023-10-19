# Lab4 : _Lecture Note_
##### 202334470_ParkSuBin

## Shell command
----
#### pwd
: shows the current path in a hierarchical directory
#### cd & ls
1. cs
: change directory
2. ls
: list files and directories

-  arguments [directory name]
    > / root
     \. current directory
    \.\. upper-level directory
    /[directory name]: absolute path
    ./[directory name]: relative path
    \.\./[directory name]: relative path

- options
    > -l : show detailed information (long format)
    -lh : same as above, but size in units

More on ls
| Command | Result |
| ------ | ------ |
| ls | List the files in the working directory |
| ls /bin | List the files in the /bin directory (or any other directory we care to specify) |
| ls -l | List the files in the working directory in long format |
| ls -l /etc /bin | List the files in the /bin directory and the /etc directory in the long format |
| ls -la \.\. | List all files (even ones with names beginning with a period character, which are normally hidden) in the working directory in long format |

#### Tip

- Autocompletion
    :Press "tab" key
- Past commands
    :Press "up arrow" key
- clear

## Manioulation
----
#### cp
: copy files and directories

| Command | Result |
| ------ | ------ |
| cp file1 file2 | Copies the contents of file1 into file2. If file2 does not exist, it is created; otherwise, file2 is silently overwritten with the contents of file1. |
| cp -i file1 file2 | Like above however, since the "-i" (interactive) option is specified, if file2 exists, the user is prompted before it is overwritten with the contents of file1. |
| cp file1 dir1 | Copy the content of file1 (in to a file named file1) inside of directory dir1. |
| cp -R dir1 dir2 | Copy the contents of the directory dir1. If directory dir2 does exist, it is created. Otherwise, it creates a directory named dir1 within directory dir2. |

#### mv
: move files and directiories or rename them

| Command | Result |
| ------ | ------ |
| mv file1 file2 | If file2 does not exist, then file1 is renamed file2. If file2 exists, its contents are silently replaced with the contents of file1. |
| mv -i file1 file2 | Like above however, since the "-i" (interactive) option is specified, if file2 exists=s, the user is prompted before it is overwritten with the contents of file1. |
| mv file1 file2 dir1 | The file1 and file2 are moved ti diretory dir1. If dir1 does not exist, mv will eixt with an error. |
| mv dir1 dir2 | If dir2 not exist, then dir1 renamed dir2. If dir2 exists, the directory dir1 is moved within directory dir2. |

#### rm
: delete files and directories permantely and irreversevely

| Command | Result |
| ------ | ------ |
| rm file1 file2 | Delete file1 and file2. |
| rm -i file1 file2 | Like above however, since the "-i" (interactive) option is specified, the user is prompted before each file is deleted. |
| rm -r dir1 dir2 | Directories dir1 and dir2 are deleted along with all of their contents. |

#### mkdir
: make a new directory
#### Wildcards

| Pattern | Matches | 
| ------ | ------ |
| * | All filenames |
| g* | All filenames that begin with the character "g" |
| b*.txt | All filenames that bigin with the character "b" and end with the characters ".txt" |
| Data??? | Any filenames the begins with the characters "Data" followed by exactly 3 more characters |

| Command | Result |
| ------ | ------ |
| cp *.txt text_files | Copy all files in the current working directory with names ending with the characters ".txt" to an existing directory named text_files |
| mv dir1 \.\./*.bak dir2 | Move the subdirectory dir1 and all the files ending in ".bak" in the current working directory's parent directory to an existing diretory named dir2. |
| rm *~ | Deletes all files in the current working directory that end with the character "~". Some applications create backup files using this naming scheme. Using this command will clean them out of a directory. |