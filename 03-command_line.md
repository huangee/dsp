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

> > REPLACE THIS TEXT WITH YOUR RESPONSE

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > REPLACE THIS TEXT WITH YOUR RESPONSE

 

