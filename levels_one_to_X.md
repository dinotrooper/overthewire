## Level One

Pretty straight forward:

`ssh bandit0@bandit.labs.overthewire.org -p 2220`

My OS is Windows 10, but I installed the Ubuntu LTS from the Mircosoft Store.

## Level One

As straight forward as the last level:

`cat readme`

`ssh bandit1@bandit.labs.overthewire.org -p 2220`

Then I used the password stored in the readme file.

## Level Two

A bit more tricky. In order to view the password with `cat`, I had to refer to filename as `./-`.

## Level Three

In order to view this password, I used the terminal autofill shortcut (tab). Spaces in a file name can be escaped by a `\`.

`cat spaces\ in\ this\ filename`

## Level Four

The file is hidden. Using `ls -a` views all hidden files and directories.

`cat .hidden`

## Level Five

Not all of the files in the `inhere` directory are text files. Using `file ./-file0*`, I discovered that `-file07` is a `ASCII text` file while the others were just `data` files. 

## Level Six

There were several directories and files to look through. I focused on one of the provided hints, `1033 bytes in size`. 

I used the ls command piped into grep to find any files that were 1033 bytes in size; `ls -l -a -R | grep -C 10 -a "1033"`.  I found only one file with that size and it contained the password for the next level.


