# Learn command line

Please follow and complete the free online [Command Line Crash Course
tutorial](https://web.archive.org/web/20160708171659/http://cli.learncodethehardway.org/book/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. Each "chapter" focuses on a command. Type the commands you see in the _Do This_ section, and read the _You Learned This_ section. Move on to the next chapter. You should be able to go through these in a couple of hours.

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

>> cheat sheet in table below

command | description
---- | ---
pwd | print workign directory aka path of the the current working directory
mkdir *dirname* | make a new directory
rm -r *dirname* | deleted a directory and its contents in pwd
touch *filename* | create a file with filename in pwd
rm *filename* | delete file in pwd
mv *oldname* *newname* | rename file *oldname* to *newname*
ls -a | list contents of directory with flag to show hidden files
cp *filepath/filename* *pathtodesireddirectory* | copy file from directory *filepath* to directory *pathtodesireddirectory*
cat *filename* | reads contents of file to stdout
` > ` *command/file* | redirects stdout to the specified command or file
sort *filename* | sorts lines of file, displays result in stdout
uniq *filename* | removes adjacent duplicate lines, disp res in stdout
<code>*firstCommand* &#124; *secondCommand*</code> | takes output of first command and uses it as input of the second command






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

>> * `ls`  print visible contents of working directory or specified dir
* `ls -a`  print visible and invisible contents of working directory
* `ls -l`  prints ls command results in long format, more info given
* `ls -lh`  prints ls -l command with unit suffix shown for file sizes
* `ls -lah`  same as -lh, but includes invisible files
* `ls -t`  ls with files ordered by last modified time
* `ls -Glp` enable color in the output (names color coded), list the files in long format, and put a slash at the end of directory names

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > * ls -m
* ls -d
* ls -F
* ls -u
* ls -1

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > xargs takes the stdin and executes the provided command with the stdin as parameters.
* `echo random words and stuff | xargs -n 1`
* `cat test.txt | xargs -n 1 echo`
* `find . -name "*.badvirus" | xargs -p rm`
