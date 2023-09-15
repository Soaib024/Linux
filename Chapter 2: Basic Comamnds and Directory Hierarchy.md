# 2 BASIC COMMANDS AND DIRECTORY HIERARCHY

## 2.1 The Bourne Shell: /bin/sh
A shell is a program that runs commands, like the ones that users enter into a terminal window. These commands can be other programs or built-in features of the shell.

There are many different Unix shells, but all derive features from the Bourne shell (/bin/sh), a standard shell developed at Bell Labs for early versions of Unix. Every Unix system needs a version of the Bourne shell in order to function correctly,

Linux uses an enhanced version of the Bourne shell called bash or the “Bourne-again” shell.

## 2.2 Using the Shell

`$ cat file1 file2 ...`

### 2.2.3 Standard Input and Standard Output

Processes read data from input streams and write data to output streams. the source of an input stream can be a file, a device, a terminal window, or even the output stream from another process. There is a third standard I/O stream, called standard error

## 2.3 Basic Commands
```shell
$ ls
$ ls -l
$ ls -F

$ cp file1 file2
$ cp file dir
$ cp file1 file2 file3 dir

$ mv file1 file2 # mv command can be used to rename or move file

$ touch file

$ rm file # remove a file

$ echo hello world
$ echo $HOME
```
## 2.4 Navigating Directories

```shell
$ cd dir
$ mkdir dir
$ rmdir dir

$ echo * # prints all file in pwd
$ cat * # prints contents of all files in pwd
```

## 2.5 Intermediate Commands

Two of the most important grep options are -i (for case-insensitive matches) and -v (which inverts the search—that is, prints all lines that don’t match). grep understands regular expressions.

When running less, you’ll see the contents of the file one screenful at a time. Press the spacebar to go forward in the file and press b (lowercase) to skip back one screenful. To quit, press q.

```shell
$ grep root /etc/passwd # print all occurrence of string `root` in `/etc/passwd` file
$ grep root /etc/*

$ less /usr/share/dict/words
$ grep ie /usr/share/dict/words | less # connecting stdout of grep to stdin of less

$ pwd

$ diff file1 file2
$ diff -u file1 file2

$ file file_name # Guessing format of the file

$ find dir_name -name file_name -print

$ head /etc/passwd
$ head -5 /etc/passwd
$ tail /etc/passwd

$ sort input_stream
$ sort -r input_stream # reverse order
$ sort -n input_stream # if inputs are numerical
```
