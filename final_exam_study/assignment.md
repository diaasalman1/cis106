#Diaa Salman

# Question 1

## Description, formula/syntax, 3 examples that you understand well

awk
* (Description) a scripting language used for processing and displaying text.
* (formula/syntax) `awk + options + {awk command} + file + file to save (optional)`
* (3 examples)
  * start printing a file from a given line
  * `awk 'NR > { print }' /etc/passwd`

cat
* (Description) used for seeing the content of a file. Also used for concatinating files.
* (formula/syntax) `cat + option + file or files to view/concatinate`
* (3 examples)
  * how to see content of a file:
    * `cat/ etc/passwd`
  * how to see the content of a file with line numbers:
    * `cat -n /etc/passwd`
  * how to see the content of a file with ening line character.
    * `cat -E /etc/passwd`
  
cp
* (Description) copies files/directories from a source to a destination
* (formula/syntax) `cp + files to copy + destination`
* (3 examples)
  * to copy a file
  * `cp Downloads/wallpapers.zip Pictures/`
  * to copy a directory with absolute path
  * `cp -r ~/Downloads/wallpapers ~/Pictures/`
  * to copy the content of a directory to another directory.
  * `cp Downloads/wallpapers/* ~/Pictures/`
  
cut
* (Description) The cut command us used to extract a specific section of each line of a file and display it to the screen
* (formula/syntax) `cut + option + file(s)`
* (3 examples)
  * Display a list of all the users in your system
  * `cut -d ':' -f1 /etc/passwd`
  * Display a list of all the users in your system with their login shell
  * `cut -d ':' -f1,7 /etc/passwd`
  * cut a range of bytes per line
  * `cut -b 1-5 usernames.txt`
  
grep
* (Description) used to search text in given file.
* (formula/syntax) `grep + option + search criteria + file(s)`
* (3 examples)
  * search any line that contains the word "dracula" in the given file
  * `grep 'dracula' ~/Documents/dracula.txt`  
  * search any line that contains the word "dracula" regardless of the case
  * `grep -i 'dracula' ~/Documents/Books/dracula.txt`
  * search any line that contains the word "dracula" regardless of the case and line number
  * `grep -in 'dracula' ~/Documents/Books/dracula.txt`

head
* (Description) displays the top N number of lines of a given file.
* (formula/syntax) `head + option + file(s)`
* (3 examples)
  * display the first 10 lines of a file
  * `head ~/Documents/Book/dracula.txt` 
  * display the first 5 lines of a file
  * `head -5 ~Documents/Book/dracula.txt`
  
ls
* (Description) ls is used for listing the content of a given directory or the file/directory itself.
* (formula/syntax) `ls + option + directory to list`
* (3 examples) 
  * list all the files inside the current working directory including hidden files.
  * `ls -a` 
  * list all the files inside a given directory
  * `ls -a ~/Pictures`
  * long list all the files inside a given directory recursively
  * `ls -1R ~/Pictures`
  
man
* (Description) manuel is to get help
* (formula/syntax)
* (3 examples) `man ls` `man pwd` `man passwd`
  
mkdir
* (Description) used for creating a single directory or multiple directories.
* (formula/syntax) `mkdir + the name of the directory`
* (3 examples)
  * create a directory in the present working directory
  * `mkdir wallpapers`
  * create a directory in a different directory using relative path
  * `mkdir wallpapers/ocean`
  * create a directory ina a different directory using absolute path
  * `mkdir ~/wallpapers/forest`
  
mv
* (Description) mv moves and renames directories.
* (formula/syntax) `mv + source + destination`
* (3 examples)
  * to move a file from a directory to another using relative path
  * `mv Downloads/homework.pdf Documents/` 
  * to move a file from a directory to another using absolute path
  * `sudo mv ~/Downloads/theme /usr/share/themes` 
  * to move a file from a directory to another combining absolute path and relative path
  * `mv Downloads/english_homework.docx /media/student/flashdrive/`
  
tac
* (Description) used for displaying the content of a file in reverse order.
* (formula/syntax) `tac + option + files) to display`
* (3 examples)
  * display the content of a file located in the pwd
  * `tac todo.md`
  * display the content of a file using absolute path
  * `tac ~/Documents/todo.md`
  
tail
* (Description) displays the last N number of lines of a give file.
* (formula/syntax) `tail + option + file`
* (3 examples) 
  * display the last 10 lines of a file
  * `tail ~/Documents/Book/dracula.txt`
  * display the last 5 lines of a file
  * `tail -5 ~/Documents/Book/dracula.txt`
  
touch
* (Description) used for creating files
* (formula/syntax) `touch + file name`
* (3 examples) 
  * to create a file called list
  * `touch list`
  * to create a file using absolute path
  * `touch ~/Downloads/games.txt`
  *  to create a file using relative path
  * `touch Downloads/games2.txt`
  
tr
* (Description) used for translating ot deleting characters from standard output.
* (formula/syntax) `Standard output | tr + option + set + set`
* (3 examples)
  * translate one character to another
  * `cat file.txt | tr '.' ','`
  * translate white space into tabs.
  * `cat program.py | tr "[:space:]" '\t'`
  * translate tabs into space
  * `cat file.py | tr -s "[:space:]" ' '`
  
tree
* (Description) shows you list of your files
* (formula/syntax)
* (3 examples)

vim/nano
* (Description) the vi command line text editor is included in all POSIX compliant operating system.
* (formula/syntax)
* (3 examples) `vim notes.txt`

# Question 2
* How to work with multiple terminals open?
  * open one terminal the open another terminal and set them side by side.
* How to work with manual pages?
  * to navigate the man page of a command, you can use the arrow key or the man command internal shortcuts.
* How to parse (search) for specific words in the manual page
  * using the grep command in combination with the man pages.
* How to redirect output (> and |)
  * we can redirect the output of commands to and from files.
* How to append the output of a command to a file
  * `ls -la > allmyfiles.lst`
* How to use wildcards
  * create files and directories quicker
* For copying and moving multiple files at the same time
  * wildcard
* How to use brace expansion
  * `touch website{1..5}.html`
* For creating entire directory structures in a single command
  * mkdir -p