# Bash Command Line Tutorials – Reading Notes

## The Command Line

- The command line allows you to work on many different tasks in the terminal as you like, particularly because you can have many terminal windows open at one time.  
- It’s interesting to think of the command line as a window to the computer’s operating system. It’s a bit intimidating to work with it instead of using a GUI to do the same tasks.  
- I’m running a Zsh shell instead of Bash. I didn’t really understand what these were, even during the 102 and 201 courses. The environment setup instructions didn’t go into detail about why we were downloading Oh my Zsh. Now I know.  

## Basic Navigation

- Admittedly, I haven’t used the **pwd** command a lot because my terminal has done a good job of displaying my location in the system. It seems like a nice check and balance for making sure I’m where I’m supposed to be as I have accidentally created files or directories in the wrong location.  
- For the **ls** command, I use it every time I change directories. It’s become a force of habit at this point. I agree with the tutorial that there is more you can do with the **ls** command, primarily because it shows you more information about where you are in the system.  
- I wasn’t aware of the optional items for the **ls** command. It showed me there were a lot more files in the location than was visible.  
- The **Tab Completion** mechanism is one of the my favorite features of the command line. When coding, it’s nice to cut back on typing where possible. In addition, it’s a helpful feature when I’m not sure of the name of a file or directory I need to access.  

## More about Files

- It’s interesting the tutorial says that Linux views the keyboard and monitor are files, just the same as a text file or directory. I hadn’t thought about it that way, and I’m still not sure I understand it.  
- Before starting my journey to be a software developer, I hadn’t had experience with the command line. It’s been interesting to see now computer logic works.  
- The tutorial talks about how Linux disregards the file extension when determining what type of file something is, but instead looks at what’s inside the file to identify what it is. This is quite interesting to me.  
- Case sensitivity and spaces are important things to keep in mind when creating files and accessing them. The Linux system places meaning to each of these.  

## Manual Page

- Manual Pages show what commands are available to use on your system and what command line argument they’re used with.  
- Manual Pages are accessed my typing **man** and the _command_ you want to know more arguments about.  
- I’ve only used Manual Pages a few times but there is a wealth of information for each command and argument.  
- The search option within Manual Pages seems very helpful. I typically turn to Google to get more information on a term, but search in the command line may be a quick way to figure out what I’m trying to search for.  

## File Manipulation

- The Linux file system is a hierarchical system that starts from the root directory.  
- It’s important to organize your files in a logical, understandable way so that locating them after a period of time is easy to do.  
- It’s important to be methodical about file and directory creation and storage.  
- When ready to make a directory, use the command **mkdir**, and then use the **-p** option to make a parent directory, or the **-v** option to have **mkdir** show what the directory is doing.  
- Removing a directory is similar to creating a directory. The command is **rmdir**.  
- What sets **rmdir** apart is that the directory as to be empty before it can be removed. This seems like a neat feature to ensure against accidental deletion of files.  
- To remove a directory that isn’t empty, use option **-r** with **rmdir**.  
- It’s good practice to use the _interactive_ option **-i** in combination with **-r** so you receive a prompt before removing a non-empty directory.  
- Using the **touch** command, Linux will create a file that does not already exist.  

## Cheat Sheet

- Main commands: pwd, ls [path], cd [path], ~ (tilde), . (dot), .. (dot) (dot), \, CTRL + C, kill [path], CTRL + Z, man <command>, man -k <search term>, q (quit man pages), mkdir <directory name>, rmdir <directory name>, touch <file name>, cp <source> <destination>, mv <source> <destination>, rm <path>, wildcards (*, ?, []).  
