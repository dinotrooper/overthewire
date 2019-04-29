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



