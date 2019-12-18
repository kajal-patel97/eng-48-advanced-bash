# Advanced Bash

This lecture will cover concepts as well as commands in bash

## Concepts

- extension-less
- everything is a file
- case sensitive

### There are 2 root locations
1. / (root)
2. ~ (user root)

### Print Working Directory
- pwd

### Listing

1. ls (list short)
2. ll (list long) - this can also be used to get permissions
3. ls -a (all)
4. ls * ( the star can be used for any part of a string and returns any files which contains those characters)

### Clear
- clear (clears the command prompt from previous commands executed)

### Go Somewhere
1. cd ( go into a file)
2. cd .. go back a file
3. cd . (shows where you currently are)

### Create a Location or Directory
1. mkdir

### Create a File
1. touch

### How to Remove a file
1. rm
2. rm -rf

### To get the manual
man ls (for the ls command)

### How to open Atom
atom .

### Permissions
 there are 3 things you can do; read, write and execute.
    - ll (to view permissions)
    - chmod [permission bianry] [File] (changes the access permissions to the systems files)


### Reads the file
cat

### Reading the lines
head - <number of lines> (from the top )
tail - <number of lines> (from the bottom)

### Sorting alphabetically
sort

### Numbering Lines
nl <file name>
