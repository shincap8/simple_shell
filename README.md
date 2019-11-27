<h1 align ="center"> _SHELL() </h1><br>

## Table of Contents 
---
- [Authors](#authors)
- [Introduction](#introduction)
- [Description](#description)
- [Installation](#installation)
- [Test](#Test)
- [Files](#files)
- [Features](#features)
- [Built With](#built-with)
- [Acknowledgments](#acknowledgments)
---
## Authors 
---
* [Kevin Giraldo](https://twitter.com/KevinGiraldo89)
* [Sara Hincapié](https://twitter.com/SaraHincapiMon1)
---
## Introduction
> Project for the end of the first trimester at Holberton School. This project is for us to show what we have learnt in C during these 3 months, the use of loops, conditional, macros, structures, variables, pointers and more, also to test our teamwork skills and our work under pressure.
---
## Description 
---
The _shell() compatible command language interpreter that executes commands read from the standard input or from a file.
---
## Installation 
---
In order to run the shell command interpreter, you must install it in your repository by cloning the following (shown below) in your machine running:
```
git clone direccion del repositorio final
```
---
## Test
---
- In order to compile the function you must run the following line in your shell:
```
gcc -Wall -Werror -Wextra -pedantic *.c -o hsh
```
_Note_: there are two ways of using the command interpreter:

#### Interactive mode:
```
 $ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$
```
#### Non-interactive mode:
```
$ echo "/bin/ls" | ./hsh
hsh main.c shell.c test_ls_2
$
$ cat test_ls_2
/bin/ls
/bin/ls
$
$ cat test_ls_2 | ./hsh
hsh main.c shell.c test_ls_2
hsh main.c shell.c test_ls_2
$
```
---
- To read the manual you man run:
```man ./[FILE]``` taking into account the structure, for our case it would be ```man ./man_hsh```

| File Name | Description and contents |
| --- | --- |
| [manpage](man_1_simple_shell) | This is the manpage for the shell command, this will help us know how to use the shell and the many uses of it, in here we can find examples and the correct sintaxis of the commands.|
| [_library.h](library.h) |This is the headers file where we can find all the prototypes of our functions and the structures used.|
| [_stdio.c](_stdio.c) |In here we have the puts and putchar function it is used to print characters.|
| [_stdlib.c](_stdlib.c) |In here we have the atoi function it is used to make integers into characters, the alloc funcction to allocate memory and the freeall function to free the memory allocated when it is not needed anymore.|
| [_string_0.c](_string_0.c) |Here we can find the function _strtok that splits a string with a delimiter given, _strcat function that concatenates two strings given, _strncmp compares an amount of characters, _strlen counts the characters in a string and _strdup to duplicate strings.|
| [_string_1.c](_string_1.c) |Here we can find the function _strchr that looks for a character in a string and returns a pointer after the match.|
| [additionalFunctions_0.c](additionalFunctions_0.c) |Here we find the function cantCmds that counts commands, parse function that divide a string in different parts, constructor function who calls the execute, print number who prints numbers, execute that executes the command given.|
| [additionalFunctions_1.c](additionalFunctions_1.c) |Here we find the function findpath that looks for the path where the command can be executed, path_concat function that concatenate the path and the command, path_copy function copies the path, help_me this function prints the help for every builtin.|
| [builtinsFunctions.c](builtinsFunctions.c) |Here we find the function exitF that allows the user to exit, path_concat function that concatenate the path and the command, path_copy function copies the path, help_me this function prints the help for every builtin, unsetF this function is to unset the environment, help function is the one who manage the help print.|
| [generate-authors.sh](generate-authors.sh) |This script generate the authors file. |
| [helpFunctions.c](helpFunctions.c) |This file has the messages for the builtin help. |
| [main.c](main.c) |This function has the launch function who starts all the process, the builtin function who calls the builtins, the issame function who compares two strings and the issignals this function is to catch a special key. |
---
## Features 

A simple shell must work with the path and without the path
* /bin/ls
* ls
---
### Examples of use

Below you can find use of some commands.

```
$ ls -a
$ echo Hola
$ pwd
```
Here are the result of this actions:

```
Image of the console using the commands above
```


## Built With

* [C](https://en.wikipedia.org/wiki/C_(programming_language))
* [Vim](https://https://en.wikipedia.org/wiki/Vim_(text_editor)/)
* [Vagrant](https://www.vagrantup.com/)
* [Peppermint](https://www.osboxes.org/peppermint/) Need to change to what Kevin is using
* [Ubuntu](https://www.ubuntu.com/)
* [GCC 4.8.4 Compiler](https://gcc.gnu.org/)
