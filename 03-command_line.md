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

> > pwd : shows current working directory path (stands for print working directory).  
    mkdir : creates a directory.  
    rmdir : deletes a directory.   
    touch : quick and easy way to create a new file (also is capable of updating the access date to a file, just happens to create a new file if it doesn't already exist).   
    rm : removes a file.   
    mv : moves (renames) a file.   
    ls -a : lists hidden files.   
    cp : copies one file from one directory to another.   
    pushd: bookmarks my current location and moves to whatever location was specified.   
    popd : "pops" back to the location bookmarked by pushd.   
    less : prints the contents of a file on a new page, "space" to scroll, "q" to quit/escape back to prompt.   

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

> > ls : lists directory contents.  
ls -a : lists directory contents, including hidden files and directories.  
ls -l : lists directory contents in long form. The information contains access rights, the number of hard links (aka labels), file name owner, file name group, size in bytes, date of last modification, file name.  
ls -lh : lists directory contents in long form and include unit suffixes.  
ls -lah : lists directory contents in long form, including hidden files, and include unit suffixes.  
ls -t : lists directory contents ordered by time stamp (newest modification listed first).  
ls -Glp : lists directory contents in long form, include a "/" following any directory names, colorize directory names.  

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > -p : labels directories with a "/" character.  
-F : labels file types with a special character, acts like a detailed -p.  
-d : lists only directories.  
-u : orders files by file access time.  
-R : shows subdirectories.

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > The function xargs is able to divide up a large list of arguments into smaller chunks in order to feed into a function. ie pass **x** number of **arg**(ument)**s**. In this example, I want to find all text files and search for the word "inflammation" in the resulting text files:  
```unix
find . -name "*.txt" | xargs grep "inflammation" 

 

