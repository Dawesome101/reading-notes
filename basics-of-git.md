# The Basics of Git - [Git Tutorial: A Comprehensive Guide](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/)

## [_General Info_](#general-info-1)
## [_Basic Commands_](#basic-commands-1)
## [_Useful Links_](#useful-links-1)

- ## General Info
  - Git is a DVCS Distributed Version Control Systems. A DVCS allows clients to create mirrored repositories. These data backups can be easily be placed on the server to replace any lost information.
    - **Snapshots** - Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project \(git commit\)  Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.
    - **Local Operations** - Git mostly relies on local operations because most necessary information can be found in local resources. This allows for process expediency because a project’s history resides on the local disk, eliminating the need to fetch history information from the server, and allowing one to continue work on a project even when not online or on a VPN.
    - **Tracking Changes** - Every single change applied to any file or directory is tracked by Git. And, as the gatekeeper, Git will always detect file corruption or loss of information in transit.
    - **Loss of Data** - Git is set up to greatly minimize the possibility of irreversible damage to files, such as accidentally lost data. Git makes it extremely difficult for a snapshot of your file that is committed to be lost.
    - **States** - Files in Git can reside in three main states: committed, modified and staged.
      - **Committed** - Data is securely stored in a local database.
      - **Modified** - File has been changed but not committed to the database.
      - **Staged** - Flagged a file’s changed version to be committed in the next snapshot.

- ## Basic Commands
  - **sudo apt-get install git** - Install git for ubuntu.
  - **git config --list** - Check git settings.
  - **git help command || git command --help || man git-command** - 3 ways to access git help.

- ## Useful Links
  - [Git Pages Markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
  
  ##### [<sub>Back To Top</sub>](#the-basics-of-git---git-tutorial-a-comprehensive-guide)
