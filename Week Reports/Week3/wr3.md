---
Name: Andrew Prieto
CIS 106 Fall-22
---

# Week 3 Report

## Summary 
Linux has many fundamentals that must be learned. Learning to use the CLI is a must when starting with linux. One of the basic commands involve using the apt command which allows you to update, install and remove programs. PPAs are packages made by anyone which comes with its own ricks. Overall take the time to learn the CLI and discover commands. 

### Exploring Desktop Environments 

There are many different kinds of desktop environments each with their own GUI. Some examples include: 
* KDE 
* XFCE
* MATE
* Cinnamon
* LXQT

A  GUI stands for graphical user interface. It allows the user to interact with the computer using apps, icons and other visual elements.
A desktop environment works the GUI. It runs on top of the OS where the icons are placed. Hidden under the desktop is nothing but code. There are basic elements to a desktop environment such as: 
* File manager 
* Icons 
* Launcher 
* Panels 
* System Tray

### Bash Shell

The bash shell is just the command-line interface(CLI). It allows the user to issue commands in text form. There are many different kinds of shells such as: 
* Tcsh 
* CSH
* KSH
* Fish 
There are many shortcuts and commands in the shell:

| Shortcut Command   | Function |
| ---------------- | ------------- | 
| Ctrl+A  | go to start of the command line    | 
| Ctrl+E  | go to end of the command line  | 
| Ctrl+R  | Search the history backwards   | 
| Ctrl+P  | Previous command   |
| Ctrl+L  | Clear the Screen   | 
| Ctrl+C  | terminate the command  | 
| Ctrl+Z | suspend/stop the command   | 

| Command   | Function |
|------------   | ----------|
| !!    | run last command | 
|   !blah   |   run the most recent command that starts with "blah" |
|   !$ |    last word of the previous command | 
| !*    |   previous command minus the last work | 

### Managing Software 

Here are some basic commands for messing with programs 

| Command   | Function  |
|---------- | ---------| 
| sudo apt update; sudo apt upgrade | updates ubuntu| 
| sudo apt install *program* | Installs a program
| sudo apt remove *program* | remove a program| 
| apt search "web browser" | search for software| 

Package - an archive that holds software, configuration files, and information about dependencies. 
Library- reusable code that can be used more than one program
Repository- large collection of software able to be downloaded. 

[!apt_Command](apt_command.png)

[!cheat_sheet](../../CheatSheets/Linux%20Workshop%20Ubuntu%20Software%20installation%20cheat%20sheet.png)