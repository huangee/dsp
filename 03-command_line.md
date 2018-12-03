# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

`pwd`: prints working directory, or shows current working directory path  
`mkdir sample-dirname`: makes (empty) directory  
`rmdir sample-dirname`: removes (empty) directory  
`rm -rf sample-dirname/`: removes directory with all contents  
`rm -rf *`: removes directory contents and keep directory  
`touch sample-filename.txt`: creates (empty) file  
`mv current-filename.txt new-filename.txt`: moves/renames file  
`rm sample-filename.txt`: removes file  
`ls -a`: lists all files, including hidden files  
`cp filename.txt sample-dirname`: copies a file from one directory to another  

---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

`ls`: lists all files in the directory that match the name. If name is left blank, it will list all of the files in the directory.  
`ls -a`: displays all files, including hidden files  
`ls -l`: displays long format listing  
`ls -lh`: displays long format with readable file size  
`ls -lah`: displays all files, including hidden files, in long format with readable file size  
`ls -t`: displays newest files first, based on timestamp  
`ls -Glp`: displays long format without group names and appends "/" indicator to directories  

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

`ls -d`:	displays only directories.
`ls -f`:	interprets each name as a directory, not a file.
`ls -m`:	displays the names as a comma-separated list.
`ls -R`: displays subdirectories as well.
`ls -u`:	displays files by the file access time.

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

#### What is the xargs command in UNIX?  

The `xargs` command in UNIX is a command line utility for building an execution pipeline from standard input. Whilst tools like `grep` can accept standard input as a parameter, many other tools cannot. Using `xargs` allows tools like `echo` and `rm` and `mkdir` to accept standard input as arguments.

#### How to use xargs  

By default `xargs` reads items from standard input as separated by blanks and executes a command once for each argument. In the following example standard input is piped to `xargs` and the `mkdir` command is run for each argument, creating three folders.

```
echo 'one two three' | xargs mkdir
ls
one two three
```

#### How to use xargs with find  

The most common usage of `xargs` is to use it with the `find` command. This uses `find` to search for files or directories and then uses `xargs` to operate on the results. Typical examples of this are removing files, changing the ownership of files or moving files.

`find` and `xargs` can be used together to operate on files that match certain attributes. In the following example files older than two weeks in the temp folder are found and then piped to the `xargs` command which runs the `rm` command on each file and removes them.

```
find /tmp -mtime +14 | xargs rm
```


