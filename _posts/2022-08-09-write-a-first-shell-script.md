---
title: Write a first shell script
author: ajilraju
date: 2022-08-08 10:15:53 +8000
categories: [Blogging, Tutorial]
tags: [shell, bash, scripting]
---

## What is Shell Script

A shell script is a list of commands and control flow statements that is run by the Unix and Linux [Shell](https://en.wikipedia.org/wiki/Unix_shell) also known as a command line interpreter. You can perform various system operations through shell scripts such as Reading/Writing files, Redirections, Pipes and various automation.

## Create shell script *File*

Every shell script is composed in the text-based file called shell script file with an extension of ```.sh```. You can create any filename according to the purpose of the script,
the name doesn't matter. So use any text editor of IDE for creating shell script files.

```bash
vim first_script.sh
```

The content inside the file.
```bash
1 #!/bin/bash
2 
3 echo "This is first shell script"
4 echo "I'm listing files in the current directory through a shell script, here"
5 ls -la

```

### Script explained
* Line: 1   ***#!/bin/bash*** is known as Shebang,  Interpreter for execution under UNIX / Linux operating systems.
* Line: 2   Blank line for more readability.
* Line: 3,4 ***echo*** is a bash builtin used to write contents to standard output(Terminal).
* Line: 5   ***ls -la*** is another bash built-in command to display a list of the information of the *files*.

## How to run the shell script

Before running the shell script need to give *execution* permission for our first shell script, otherwise, the shell script won't be executed as a script.

Use the Unix ***chmod*** command to give execution permission for the file.

```bash
chmod u+x first_script.sh

ls -la first_script.sh
-rwxrw-r-- 1 tux tux 0 Aug  9 10:05 first_script.sh
```

### Time to execute 💥

To execute the Shell script, you can simply call the shell script from your favorite terminal program.

```bash
./first_script.sh
```

Or you can try to execute explicitly with a Bash interpreter.

```bash
bash first_script.sh
```
