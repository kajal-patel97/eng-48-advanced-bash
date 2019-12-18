# Advanced Bash

This lecture will cover concepts as well as commands in bash

## Concepts

- extension-less
- everything is a file
- case sensitive
- STDIN, STDOUT, STDERR (standard in, standard out, standard error)

## Commands

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

### Word Count
wc <filename>

## Piping and Redirection
piping is when you join 2 programs together so that they run

### STDIN, STDOUT, STDERR
these have numbers that identify them.

- STDIN is 0
- STDOUT is 1
- STDERR is 2

### Redirecting
you can take a output of a function and move it to another location

````
$ ls missing_directory
  ls: cannot access 'missing_directory': No such file or Directory
  ls missing_directory 2>> error_logs.txt
````
  - this took the outcome of the ls command and placed it in a file called directory.txt
  - this can capture errors and place them somewhere.

#### Searching for files and inside files

- grep

````
cat example.txt | grep text

````

- grep -v (searches for non matching lines - so takes it out)

````
 cat example.txt | grep -v and | sort -r

````

## Running Processes

1. top
  - like task manager you can see what programmes are running in real time

2. ps
  - shows you your current processes

3. ps aux
  - gives you a full list of processes
  - usually used with grep to find exactly what you are looking for

  ````
  ps aux | grep bio

  ````

4. PID
  -  process id
  kill [pid]

5. eg sleep 120 &
  - the & makes the process run in the background 
