# Lab5 : _Lecture Note_
##### 202334470_ParkSuBin

## I/O Redirection
----
#### Standard Output
* \>
: create and save the output in a file
\- Command "cat" displays the content of a text file.
* \>>
: appends output to an extising file (if it already exitsts), or create and write to a new file if it doesn't exist

#### Standard Input
* <
: redirecct input from a file

## Pipelines "|"
----
: feeds output of previous command to input of next command
    ex) command1 | command2 | command3 ...
    
- tip : press "q" key to exit the screen.

## Expansion
----
: Special characters expand its meanings when given to shell commands.

* echo : a command that outputs the text behind echo
* echo * : commands that output the filename in the current directory
* echo ~ : commands that show the current user's home directory

## Permissions
----
#### permissions
* Linux is a multi-user-system
* Files and directories have a permission differently to owner / group / others.

#### changing permissions
* "chmod" change permissions

| Value | Meaning |
| ------ | ------ |
| 777 | (rwxrwxrwx) No restrictions on permissions. Anybody may do anything. Generally not a desirable setting. |
| 755 | (rwxr-xr-x) The file's owner may read, write, and execute the file. All others may read and execute the file. This setting is common for programs that are by all users. |
| 700 | (rwx------) The file's owner may read, write, and execute the file. Nobody else has any rights. This setting is useful programs that only the owner may use and must be kept private from others. |
| 666 | (rw-rw-rw-) All users may read and write the file. |
| 644 | (rw-r--r--) The owner may read and write a file, while all others may only read the file. A common setting for data files that everybody may read, but only the owner may change. |
| 600 | (rw-------) The owner may read and write a file. All others have no rights. A common setting for data files that the owner wants to keep private. |

#### superuser
* A superuser has all system administation authority.
* Some commands need superuser's privilleges.
* Put "sudo" before the command if you are a superuser.
* Type "exit" to get out of a superuser session.

## Text Editors
----
* In Linux, you cna choose CLI-based or GUI-based text editors.

| Name | description | Interface |
| ------ | ------ |------ | 
| vi, vim | The granddaddy of Unix text editors, vi, is infamous for its obtuse user interface. On the bright side, vi is powerful, lighweight, and fast. Learning vi is a Unix rite of passage, since it is universally available on Unix-like systems. On most Linux distributions, an enhanced version of vi called vim is provided in place of vi. vim is a remarkable editor and well worth taking the time to learn it. | command line |
| Emacs | The true giant in the world of text editors is Emacs originally written by Richard Stallman. Emacs contains (or can be made to contain) every feature ever conceived of for a text editor. It should be noted that vi and Emacs fans fight bitter religious wars over which is better. | command line |
| nano | nano is a free clone of the text editor supplied with the pine email program. nano is very easy to use but is very short on features compared to vim and emacs. nano is recommended for first-time users who need a command line editor. | command line |
| gedit | gedit is the editor supplied with the GNOME desktop environment. gedit is easy to use and contains enough features to be a good beginners-level editor. | graphical |
| kwrite | kwrite is the "advanced editor" supplied with KDE. It has syntax highlighting, a helpful feature for programmers and script writers. | graphical |

## Shell Script 
----
* write and run a shell script

## Tip : History
----
* Type "history" to see previous command history.
* Or, save it to text file.
