# Linux-notes
Containing my Linux notes and commands as I learn the Linux fundamentals.

## What i'm learning
- Basic Linux commands.
- File system navigation.
- File permissions.
- Package management.

-=-=-=-=-=-=-=-

## Basic commands

## pwd
- Print working directory (shows your current location).

## ls
- List files and directories.
- ls -a # Shows all files including hidden ones.
- ls -l # Displays "Long" list, inclduing file size, permissions, and last modified date.
- ls -lh # Makes files sizes "Human readable".

## cd
- Change directory.
Example : cd /home.
- cd ~ # Returns/resets your back to home directory.

## mkdir
- Create a new directory.
Example : mkdir test-folder.

## cat
- The cat command is generally used for displaying the
contents of a file, but it can also be used to create small files.
- The cat command followed by a filename will display the contents of that
file, but to create a file, we follow the cat command with a redirect, denoted
with the > symbol, and a name for the file we want to create.

## touch
- Create a new file.
Example : touch test-file.

## rm
- Remove files or directories.
Example : rm file.txt.

-=-=-=-=-=-=-=-=-

## File navigation.

## .
- Current directory.

## ..
- Parent directory.

-=-=-=-=-=-=-=-=-

## User Commands

## whoami
- Displays the current logged-in user.

## man
- An extension of help is man. You can type man before the command
  to view the manual page for any chosen command, utility or application.

## ps
- Used to display information about processes running on the machine.

## |
- piping command.
- It allows us to take the output of one command.
- And use it as input for another command.

Example: ps aux | grep apache2
This command tells Linux to display all my services and then send that
output to grep, which will look through the output for the keyword apache2
and then display only the relevant output, thus saving me considerable time.

-=-=-=-=-=-=-=-=-

## Locating commands

## locate
- Type locate followed by a keyword what it is you want to find.
  This command will go through your entire filesystem and locate every occurrence of that word.

## sudo updatedb
- To update the database the locate command uses.
- Note that we updated the command with "sudo", this is important!.
- If a command requires root (superuser) privileges, as updatedb does.
- And you're logged in as a regular user.
- You can provide the command with root privileges using the "sudo" command.
- followed by your password.

## whereis
- To locate a binary.
- This command returns not only the location of the binary.
- But also its source and man page if they're available.

## which
- More specific locating command.
- it returns the location of only the binaries in the PATH variable in Linux.

## find
- Most flexible of the searching commands.
- It is capable of beginning in any designated directory and looking for a number
of different parameters, including, of course, the filename, but also the date
of creation or modification, the owner, the group, permissions, and the size.


## Important subdirectories

## /root
- The home directory of the all-powerful root user.

## /etc
- Generally contains the Linux configuration files—files that control
when and how programs start up.

## /home 
- The user’s home directory.

## /mnt
- Where other filesystems are attached or mounted to the filesystem.

## /media
- Where CDs and USB devices are usually attached or mounted
to the filesystem.

## /bin
- Where application binaries (the equivalent of executables in
Microsoft Windows or applications in macOS) reside.

## /lib
- Where you’ll find libraries (shared programs that are similar to
Windows DLLs).

-=-=-=-=-=-=-=-=-=-=-=-=-=-=-

## Filtering commands

## grep
- Filter to search for keywords
- The grep command is often used when output is piped from one command to
another.


## notes
I will continue to add to this repo as I progress my journey in Linux and cybersecurity.

