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

> > 1. pwd : present working directory
> > 2. mkdir <new directory> : make directory
> > 3. rm  <existing directory> -r : delete directory / 
> > 4.  touch <filename> : create new file
> > 5. mv <filename old> <filename new> : move is used to rename if ir is in the same dir
> > 6. rm <filename>
> > 7. ls -la  : a is mode for all
> > 8. cp <source file path> <destination path>
> > 9. cat <filename> : prints contents of the file
> > 10. wc <filename> : prints word count and line count  for file

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

> > The ls command shows contents of the current directory
> >
> > -a indicates all files including hidden file (start with .)
> >
> > -l indicates list form with extra details
> >
> > -lh  prints the file size in human readable form that is bytes, kilobytes, gigabytes reducing reducing number of digits to three or less
> >
> > -lah prints all files in a directory including hidden files in long format with human readable file size  
> >
> > ls -t  sorts files by time modified most recent at the top
> >
> > ls-Glp prints directory entries in long format with colorized output and adds  / after the names of directories

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > ls -S list files sorted by size
> >
> > ls -R recursively list files in all subdirectories - can get crazy
> >
> > ls -Gla lists all files lin long format that is colorized 
> >
> > ls -u files sorted by last time they were accessed not modified
> >
> > ls -U files sorted by when they were created
> >
> >

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > Xargs commond is used for building an execution pipeline from standard input. xargs can be used with tools like echo, rm, find etc. that cannot take standard input as a parameter to increase their functionality.
> >
> > ```con
> > users-MBP:Data_Science user$ echo 'one two three' | xargs mkdir
> > users-MBP:Data_Science user$ ls
> > Github		Other		References	one		two
> > Metis Test Prep	Python scripts	code_snips.md	three
> > ```
> >
> > we have been able to make several directories. 

 

