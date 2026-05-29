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
- Creates a new directory.
Example : mkdir newdirectory.

## cat
- The cat command is generally used for displaying the
contents of a file, but it can also be used to create small files.
- The cat command followed by a filename will display the contents of that
file, but to create a file, we follow the cat command with a redirect, denoted
with the > symbol, and a name for the file we want to create.
- Once you hit enter, linux will go into interactive mode and anything you type will
  be added to the file.
- To exit out of interactive mode, press Cntrl+D which will bring you back to linux.
- To add more to a file we run the the same command but with two denotes this time ">>".
- To overwrite information in the file we use a single donte again ">".
- and to check the newly update info of the file " cat hackingskils".

## touch
- Creates a new file.
Example : touch newfile.

## cp
- copies a chosen file.
- This creates a duplicate of the file in
the new location and leaves the old one in place.

## rm
- To remove a file.
Example : rm file.txt.

## rmdir
- To remove a directory.
Example : rmdir newdirectory

- The command won't remove a directory that is not empty.
- Linux will warn you saying it's not empty.
- You will need to remove the contents of the directory.
- Before removing the directory.
- Also a good way to protect yourself from accidentally deleting items.

- rm -r to remove the directory and alll content in one go.
  example : rm -r newdirectory
- Be wary using this command though!.
- Very easy to delete files and directories by mistake.
- Using rm -r in your home directory for instance.
- Would delete every file and directory there!.

## mv
- Can be used to move a file or directory to a new location.
- Or simply to give an existing file a new name.
  Example : mv newfile newfile2





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

-=-=-=-=-=-=-=-=-=-=-=-=-=-

##  Manipulation of text commands (whilst in a text file)

## head
- Lets you view the beginnig of a text.
- (The first 10 lines by default).
-  adding a -(and a chosen number) after head allows you to choose the number of lines to view.
Example : head -20 /etc/apache2/apache2.conf

## tail
- Lets you view the end of a text.
- (The last 10 lines by default).
-  adding a -(and a chosen number) after tails allows you to choose the number of lines to view.
Example : tail -5 /etc/apache2/apache2.conf

## nl
- displays the text but with the lines numbered.

## s
- Performs a subsitution
- you first give the term you are
searching for (o) and then the term you want to replace it with (0), separated
by a slash (/). The g flag tells Linux that you want the replacement
performed globally. We then save the result to a new file named
unix_passwords2.txt.

Example : sed s/o/0/g /usr/share/metasploitframework/data/wordlists/unix_passwords.txt > /usr/share/m
framework/data/wordlists/unix_passwords2.txt





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

## sed (stream editor)
- lets you search for occurrences of a word or a text pattern
and then perform some action on it.



## notes
I will continue to add to this repo as I progress my journey in Linux and cybersecurity.

