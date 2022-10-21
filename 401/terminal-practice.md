# Practicing the Terminal - [Linux Tutorials](https://ryanstutorials.net/linuxtutorial)

## Index

[HOME](../README.md)  
[General Info](#general-info)  
[Basic Commands](#basic-commands)  
[Tips](#tips)  
[Important Directories](#important-directories)  

## General Info

- Everything is a file under Linux, even directories.
- Linux is an extensionless system. Files can have any extension they like or none at all.
- Linux is case sensitive. Beware of silly typos.
- No undo. The Linux command line does not have an undo feature. Perform destructive actions carefully.
- Command line options. Most commands have many useful command line options. Make sure you skim the man page for new commands so you are familiar with what they can do and what is available.

## Basic Commands

- `pwd` - Print Working Directory - ie. Where are we currently.
- `ls` - List the contents of a directory.
  - `-l` - Ordered list.
  - `-a` - Show hidden objects.
- `cd` - Change Directories - ie. move to another directory.
- `~` - This is a how you get to your home directory. `/home/ryan/Documents` or `~/Documents`
- `.` - This is a reference to your current directory. If the current directory is say Documents, then it could also be written as '`/Documents`
- `..` - This is a reference to the parent directory. you could run the command ls `../../` etc.
- `touch <filename>` - Create a blank file. "touch" is actually a command we may use to modify the access and modification times on a file
- `rm` - Delete file.
  - `-r` - Can be used to **delete a directory** and everything inside it.
- `md` - Make directory
- `rd` - Delete directory. The diretory MUST be empty before it can be deleted.  To bypass this us "`rm -r <directory>`".
- `cp <source> <destination>` - Copy file.
  - `-r` - Recursive.  Used for copying directories including its contents and subcontents.
- `mv <source> <destination>` - Move files.
  - `mv foo foo2` Rename a file.
- `\\` - Escape character.  For example `md escape\ test` creates a directory "escape test".
- `''` or `""` - Used to encapsulate spaced names.  Example `md 'space test'` or `md "space test"`. If no quotes are used, `md space test` will create two directories, "space" and "test"
- `file` - obtain information about what type of file a file or directory is.

## Tips

- `Tab` - When you start typing a path (_anywhere on the command line, you're not just limited to certain commands_) you may hit the Tab key on your keyboard at any time which will invoke an auto complete action. If nothing happens then that means there are several possibilities. If you hit Tab again it will show you those possibilities. You may then continue typing and hit Tab again and it will again try to auto complete for you.
- `q` is commonly used for "quit". Example, while using the manual, press q to quit.
- **Manual**
  - `man <command>` - Look up the manual page for a particular command.
  - `man -k <search term>` - Do a keyword search for all manual pages containing the given search term.
  - **From within the manual**
    - `/<term>` - Used within a manual page, it will perform a search for 'term'
    - `n` - After performing a search within a manual page, select the next found item.

## Important Directories

- `/etc` - Stores config files for the system.
- `/var/log` - Stores log files for various system programs. (_You may not have permission to look at everything in this directory. Don't let that stop you exploring though. A few error messages never hurt anyone._)
- `/bin` - The location of several commonly used programs.
- `/usr/bin` - Another location for programs on the system.

[Back To Top](#practicing-the-terminal---linux-tutorials)
