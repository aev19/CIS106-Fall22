--- 
Andrew Prieto
CIS-106
---

# Question 1 

## awk 
* Description
  * Awk is scripting language used for processing and displaying text. AWK can work with a text file or from standard output.
* Formula: 
  * awk + option {awk command} + file 
  * Command output | awk + options +{awk command}
  * Examples: 
    * How to print the first field of a file: 
      * awk -F':' '{print$1}' /etc/passwd
    * How to start printing from a different line
      * awk 'NR > 3 {print}' /etc/passwd
    * How to change a field to upper case:
      * awk -F '{print toupper($1)}'
  
## cat 
* Description: 
  * Used for seeing the content of a file. Also used for concatenating files.
* Formula/Syntax:
  * cat + option + file or files to view/concatenate 
* Examples
  * How to see the content of a file: 
    * cat /etc/passwd
  * How to see the content of a file with line numbers:
    * cat -n /etc/passwd
  * How to see the content of a file with ending line character 
    * cat -E /etc/passwd
    * Command Output: 
  
## cp 
* Description: 
  * Copies files/directories from a source to a destination
* Formula/Syntax:
  * cp + files to copy + destination
  * cp -r +directory to copy + destination
* Examples: 
  * To copy a file
    * cp Downloads/wallpapers.zip Pictures/ 
  * To copy a directory with absolute path
    * cp -r ~/Downloads/wallpapers ~/Pictures/
  * To copy multiple files in a single command 
    * sudo cp -r script.sh program.py home.html assets/ var/www/html
  
## cut
* Description: 
  * Used to extract a specific section of each line of a file and display it to the screen
* Formula/Syntax: 
  * cut + option + Files(s)
* Examples: 
  * Display a list of all the users in your system
    * cut -d ':' -f1 /etc/passwd
  * Display a list of all the users in your system with their login shell
    * cut -d ':' -f1,7 /etc/passwd
  * Cut a file excluding a given field 
    * cut -d ',' --complement -s -f3 users.txt
  
## grep
* Description: 
  * Used to search text in given file. Works line by line
* Formula/Syntax:
  * grep + option + search criteria + files(s)
* Examples
  * Search any line that contains the word "dracula" in a given file: 
    * grep 'dracula' ~/Document/dracula.txt
  * Search any line that contains the work "dracula" regardless of case and with number line 
    * grep -in 'dracula' ~/Documents/Books/dracula.txt
  * Search and match only the work 
    * grep -o 'dracula' ~/Documents/Books/dracula.txt
  
## head 
* Description: 
  * Displays the top N number of lines of a given file. By default it's 10 lines.
* Formula/Syntax:
  * head + option + files(s)
* Examples:
  * Display the first 10 lines of a file:
    * head ~/Documents/Book/dracula.txt
  * Display the first 5 lines of a file 
    * head -5 ~/Documents/Book/dracula.txt
  * Display the first 30 lines of a file 
    * head -30 ~/Documents/Book/dracula.txt

## ls
* Description:
  * Used for listing the content of a given directory or the file/directory itself
* Formula/Syntax:
  * ls + option directory to lis 
* Examples: 
  * List the content of the present working directory 
    * ls 
  * List all the flies inside a given directory 
    * ls -a ~/Pictures
  * long list all the files inside a given directory recursively 
    * ls -lR ~/Pictures

## Man 
* Description:
  * Pages of documentation files that describe Linux shell commands, executable programs, system calls, special files, and so forth. 
* Formula/Syntax:
  * man + command 
* Examples: 
  * Show all the available pages of a command 
    * man -a passwd 
  * open the man page of the passwd command 
    * man passwd
  * Show the man page section of the passwd command 
    * man -f passwd

## mkdir 
* Description: 
  * used for creating a single directory or multiple directories 
* Formula/Syntax:
  * mkdir + name of directory 
* Examples: 
  * Create a directory in the present working directory:
    * mkdir wallpapers
  * create multiple directories: 
    * mkdir wallpapers/cars wallpapers/cites wallpapers/forest
  * create a directory with a parent directory at the same time 
    * mkdir -p wallpapers_others/movies
  
## mv
* Description: 
  * moves and renames directories
* Formula/Syntax:
  * mv + source + destination 
* Examples: 
  * To move a file from a directory to another using relative path:
    * mv Downloads/homework.pd Document/
  * To move multiple directories/files to a different directory 
    * mv games/ wallpapers/ rockmusic/ media/student/flashdrive/
  * To rename a file 
    * mv homework.docx cis106homework.docx
  
## tac 
* Description:
  * Used for displaying the content of a file in reverse order 
* Formula/Syntax:
  * tac + option + files(s) to display 
* Examples: 
  * Display the content of a file located in the pwd
    * tac todo.md
  * Display the content of a file using absolute path 
    * tac ~/Documents/todo.md
  * Display the content a file in reverse order 
    * tac /etc/passwd
  
## tail 
* Description:
  * Displays the last N number of lines of a given file. By default it's 10. 
* Formula/Syntax:
  * tail + option + file
* Examples: 
  * Display the last 10 lines of a file 
    * tail ~/Documents/Books/dracula.txt 
  * Display the last 5 lines of a file 
    * tail -5 ~/Documents/Books/dracula.txt
  * Display the last 20 lines of a file
    * tail -20 ~/Documents/Books/dracula.txt
  
## touch 
* Description: 
  * Used for creating files 
* Formula/Syntax:
  * touch + file name 
* ExamplesL 
  * Create a file named list: 
    * touch list 
  * Create a file using absolute path:
    * touch ~/Downloads/games.txt
  * Create serval files
    * touch list_of_cars.txt script.py names.csv
  
## tr 
* Description: 
  * Used for translating or deleing characters from standard output.
* Formula/Syntax:
  * standard output | tr + option + set + set 
* Examples: 
  * Translate white space into tabs 
    * cat program.py | tr "[:space:]" '\t'
  * Translate one character to another (period to comma)
    * cat file.txt | tr '.' ','
  * Translate tabs into space
    * cat file.py | tr -s "[:space:]" ' ' 

## tree 
* Description: 
  * a recursive directory listing program that produces a depth-indented listing of files 
* Formula/Syntax:
  * tree + directory
* Examples: 
  * Tree list current directory 
    * tree
  * Tree list a directory 
    * tree Downloads/
  * Tree list using absolute path 
    * tree ~/Documents/
  
## vim/nano
* Description: e
  * a text editor 
* Formula/Syntax:
  * nano + filename
  * vim + filename
* Examples 
  * Enter nano
    * nano 
  * Enter vim
    * vim 

## Question 2 
 
 * How to work with multiple terminals open 
   * Right click anywhere in the terminal(blank area) click new window
 * how to work is manual pages 
   * use the man command followed by the command you want to use
 * how to parse(search) for specific words in the manual page 
   * use the grep command to filter specific words. 
 * How to redirect output (> and |)
   * The > command saves the output to a file name while the | applies the output to the next command. 
 * How to append the output of a command to a file 
   * use the > command with a file name 
 * How to use wildcards 
   * Wildcards use letters and characters to specify a file name for searches. 
   * ls -A *.txt *.py
 * How to use brace expansion 
   * mkdir -r /challenge-Lab6/{audio/docs/images}