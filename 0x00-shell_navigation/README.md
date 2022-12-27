# Learning Objectives

At the end of this project, you are expected to be able to [explain to anyone](https://fs.blog/feynman-technique/), *without the help of Google:*

## General

  * How to navigate in an Unix system
  * How to list files and directories
  * How to display the content of a file
  * How to create a file or directory
  * How to remove a file or directory
  * How to move or copy a file or directory

# Requirements

  * All tasks *must be* done inside the sandbox `Ubuntu 20.04`
  * Your sandbox *must be available at the end of this project* - the Checker will access to it at midnight for running the correction!

# Tasks

## [0. Create me!]()

Access your sandbox:
```
$ ssh <ssh-tokem>
$ Enter password: ************
```
and:

  * Change your working directory to `/root`
  * Then, create an empty file `so_cool`

*Advices:*

  * Don’t forget to validate your current working directory
  * Don’t forget to display the list of files of your current directory to validate the creation of the new file

```
# change directory & create empty file

$ cd ~/root
root $ touch so_cool


# validate directory & validate created file

root $ pwd
/root
root $ ls -l
drwx------ 2 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 empty_directory
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 not_here
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 old_school
drwx------ 2 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 ready_to_be_removed
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 school
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 so_cool
```

## [1. More of me]()

Access your sandbox:
```
$ ssh <ssh-tokem>
$ Enter password: ************
```
and:

  * Change your working directory to `/root`
  * Then, copy the file `school` to `/tmp`

*Advices:*

  * Don’t forget to validate your current working directory
  * Don’t forget to display the list of files of your current directory to validate the copy of the file

```
# change directory to /root & copy file from /root to /tmp

$ cd /root
root $ cp school /tmp


# change directory to /tmp & validate file

root $ cd /tmp
tmp $ ls -l
drwx------ 2 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 right_school
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 school
tmp $
```

## [2. To old]()

Access your sandbox:
```
$ ssh <ssh-tokem>
$ Enter password: ************
```
and:

  * Change your working directory to `/root`
  * Then, rename the file `old_school` to `new_school` (in the same directory)

*Advices:*

  * Don’t forget to validate your current working directory
  * Don’t forget to display the list of files of your current directory to validate the renaming of the file
```
# change to (and list) /root directory

$ cd /root && ls -l
drwx------ 2 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 empty_directory
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 not_here
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 old_school
drwx------ 2 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 ready_to_be_removed
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 school
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 so_cool


# rename old_school to new_school & list directory

root $ mv old_school new_school && ls -l
drwx------ 2 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 empty_directory
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 new_school
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 not_here
drwx------ 2 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 ready_to_be_removed
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 school
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 so_cool
root $
```

## [3. Not here]()

Access your sandbox:
```
$ ssh <ssh-tokem>
$ Enter password: ************
```
and:

  * Change your working directory to `/root`
  * Then, move the file `not_here` to `/tmp/right_school`

*Advices:*

  * Don’t forget to validate your current working directory
  * Don’t forget to display the list of files of your current directory to validate the move of the file

```
# change to (and list) /root directory

$ cd /root && ls -l
drwx------ 2 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 empty_directory
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 new_school
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 not_here
drwx------ 2 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 ready_to_be_removed
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 school
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 so_cool


# move 'not_here' to /tmp/right_school & list directory

root $ mv not_here /tmp/right_school && ls -l
drwx------ 2 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 empty_directory
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 new_school
drwx------ 2 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 ready_to_be_removed
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 school
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 so_cool


# change to (and list) /tmp/right_school directory
root $ cd /tmp/right_school && ls -l
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 not_here
/tmp/right_school $
```

## [4. Not anymore]()

Access your sandbox:
```
$ ssh <ssh-tokem>
$ Enter password: ************
```
and:

  * Change your working directory to `/root`
  * Then, delete the file `ready_to_be_removed`

*Advices:*

  * Don’t forget to validate your current working directory
  * Don’t forget to display the list of files of your current directory to validate the removal of the file

```
# change to (and list) /root directory

$ cd /root && ls -l
drwx------ 2 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 empty_directory
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 new_school
drwx------ 2 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 ready_to_be_removed
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 school
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 so_cool


# delete 'ready_to_be_removed' & list current directory

root $ rm ready_to_be_removed && ls -l
drwx------ 2 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 empty_directory
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 new_school
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 school
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 so_cool
root $
```
## [5. Organization is key!]()

Access your sandbox:
```
$ ssh <ssh-tokem>
$ Enter password: ************
```
and:

  * Change your working directory to `/root`
  * Then, create a directory `school_is_amazing`

*Advices:*

  * Don’t forget to validate your current working directory
  * Don’t forget to display the list of directories of your current directory to validate the creation of the directory
```
# change to (and list) /root directory

$ cd /root && ls -l
drwx------ 2 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 empty_directory
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 new_school
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 school
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 so_cool


# create 'school_is_amazing' directory and list current directory

root $ mkdir school_is_amazing && ls -l
drwx------ 2 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 empty_directory
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 new_school
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 school
drwx------ 2 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 school_is_amazing
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 so_cool
root $
```

## [6. No need]()

Access your sandbox:
```
$ ssh <ssh-tokem>
$ Enter password: ************
```

  * Change your working directory to `/root`
  * Then, remove the directory `empty_directory`

*Advices:*

  * Don’t forget to validate your current working directory
  * Don’t forget to display the list of directories of your current directory to validate the removal of the directory

```
# change to (and list) /root directory

drwx------ 2 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 empty_directory
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 new_school
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 school
drwx------ 2 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 school_is_amazing
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 so_cool
root $


# delete 'empty_directory' directory and list current directory

root $ rmdir empty_directory && ls -l
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 new_school
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 school
drwx------ 2 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 school_is_amazing
-rw------- 1 okidoki-jpg okidoki-jpg    0 Aug 29 10:37 so_cool
root $
```
