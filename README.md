# Code Fellows Reading Notes

## Prework from Code 102
<sub>Having tested into 201, these are notes compiled while going over the prework derived from 102's overview information.</sub>
- [_Practicing the Terminal_](./terminal-practice)
- [_The Basics of GIT_](./basics-of-git)

## Code 201 Reading Notes
- [Class Reading-01:](./class-01)
- [Class Reading-02:](./class-02)
- [Class Reading 03:](./class-03)
- [Class Reading 04:](./class-04)
- [Class Reading 05:](./class-05)
- [Class Reading 06:](./class-06)
- [Class Reading 07:](./class-07)
- [Class Reading 08:](./class-08)
- [Class Reading 09:](./class-09)
- [Class Reading 10:](./class-10)
- [Class Reading 11:](./class-11)
- [Class Reading 12:](./class-12)
- [Class Reading 13:](./class-13)
- [Class Reading 14:](./class-14)
- [Class Reading 15:](./class-15)

## Code 102 Reading Notes
<sub>Having tested out of Code 102, no notes were taken during the course however while doing the prework for 201, notes were gathered from the suggested reading and tutorials which are visble here in the following entries.</sub>

### 1. Practicing the Terminal - [Linux Tutorials](https://ryanstutorials.net/linuxtutorial)
- #### General Info
  - Everything is a file under Linux, even directories.
  - Linux is an extensionless system. Files can have any extension they like or none at all.
  - Linux is case sensitive. Beware of silly typos.
  - No undo. The Linux command line does not have an undo feature. Perform destructive actions carefully.
  - Command line options. Most commands have many useful command line options. Make sure you skim the man page for new commands so you are familiar with what they can do and what is available.

- #### Basic Commands
  - **pwd** - Print Working Directory - ie. Where are we currently.
  - **ls** - List the contents of a directory.
    - **-l** - Ordered list.
    - **-a** - Show hidden objects.
  - **cd** - Change Directories - ie. move to another directory.
  - **~** - This is a shortcut for your home directory. /home/ryan/Documents or ~/Documents
  - **.** - This is a reference to your current directory. If the current directory is say Documents, then it could also be written as ./Documents 
  - **..** - This is a reference to the parent directory. you could run the command ls ../../ etc.
  - **touch \<filename\>** - Create a blank file. "touch" is actually a command we may use to modify the access and modification times on a file 
  - **rm** - Delete file.
    - **-r** - Can be used to **delete a directory** and everything inside it.
  - **md** - Make directory
  - **rd** - Delete directory. The diretory MUST be empty before it can be deleted.  To bypass this us "**rm -r \<directory\>**".
  - **cp \<source\> \<destination\>** - Copy file.
    - **-r** - Recursive.  Used for copying directories including its contents and subcontents.
  - **mv \<source\> \<destination\>** - Move files. 
    - **mv foo foo2** Rename a file.
  - **\\** - Escape character.  For example **md escape\ test** creates a directory "escape test"
  - **\'\'** or **""** - Used to encapsulate spaced names.  Example **md 'space test'** or **md "space test"**. If no quotes are used, **md space test** will create two directories, **space** and **test**
  - **file** - obtain information about what type of file a file or directory is.

- #### Tips
  - **Tab** - When you start typing a path \(*anywhere on the command line, you're not just limited to certain commands*\) you may hit the Tab key on your keyboard at any time which will invoke an auto complete action. If nothing happens then that means there are several possibilities. If you hit Tab again it will show you those possibilities. You may then continue typing and hit Tab again and it will again try to auto complete for you.
  - **q** is commonly used for "quit". Example, while using the manual, press q to quit.
  - **Manual**
    - **man \<command\>** - Look up the manual page for a particular command.
    - **man -k \<search term\>** - Do a keyword search for all manual pages containing the given search term.
    - **From within the manual**
      - **/\<term\>** - Within a manual page, perform a search for 'term'
      - **n** - After performing a search within a manual page, select the next found item. 

- #### Important Directories
  - **/etc** - Stores config files for the system.
  - **/var/log** - Stores log files for various system programs. \(*You may not have permission to look at everything in this directory. Don't let that stop you exploring though. A few error messages never hurt anyone.*\)
  - **/bin** - The location of several commonly used programs.
  - **/usr/bin** - Another location for programs on the system.

### 2. The Basics of Git - [Git Tutorial: A Comprehensive Guide](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/)
- #### General Info
  - Git is a DVCS Distributed Version Control Systems. A DVCS allows clients to create mirrored repositories. These data backups can be easily be placed on the server to replace any lost information.
    - **Snapshots** - Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project \(git commit\)  Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.
    - **Local Operations** - Git mostly relies on local operations because most necessary information can be found in local resources. This allows for process expediency because a project’s history resides on the local disk, eliminating the need to fetch history information from the server, and allowing one to continue work on a project even when not online or on a VPN.
    - **Tracking Changes** - Every single change applied to any file or directory is tracked by Git. And, as the gatekeeper, Git will always detect file corruption or loss of information in transit.
    - **Loss of Data** - Git is set up to greatly minimize the possibility of irreversible damage to files, such as accidentally lost data. Git makes it extremely difficult for a snapshot of your file that is committed to be lost.
    - **States** - Files in Git can reside in three main states: committed, modified and staged.
      - **Committed** - Data is securely stored in a local database.
      - **Modified** - File has been changed but not committed to the database.
      - **Staged** - Flagged a file’s changed version to be committed in the next snapshot.

- #### Basic Commands
  - **sudo apt-get install git** - Install git for ubuntu.
  - **git config --list** - Check git settings.
  - **git help command || git command --help || man git-command** - 3 ways to access git help.

- #### Useful Links
  - [Git Pages Markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

## Code 201 Reading Notes

#### 1. Daily Reading Assignment
- Notes
- Questions

#### 2. Daily Reading Assignment
- Notes
- Questions

#### 3. Daily Reading Assignment
- Notes
- Questions

#### 4. Daily Reading Assignment
- Notes
- Questions

#### 5. Daily Reading Assignment
- Notes
- Questions

#### 6. Daily Reading Assignment
- Notes
- Questions

#### 7. Daily Reading Assignment
- Notes
- Questions

#### 8. Daily Reading Assignment
- Notes
- Questions

#### 9. Daily Reading Assignment
- Notes
- Questions

#### 10. Daily Reading Assignment
- Notes
- Questions

#### 11. Daily Reading Assignment
- Notes
- Questions

#### 12. Daily Reading Assignment
- Notes
- Questions

#### 13. Daily Reading Assignment
- Notes
- Questions

#### 14. Daily Reading Assignment
- Notes
- Questions

#### 15. Daily Reading Assignment
- Notes
- Questions

##### [\[Return To Top\]](#code-fellows-reading-notes)


