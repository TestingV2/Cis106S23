---
Name: Juan Baez
Semester: Spring 23
Course: CIS 106 Linux Fundamentals
---

# Final Assignment  

## Question 1

1. **awk**: A scripting language used for processing and displaying text.

Syntax: `awk`

Examples: 
- `awk '{print $1,$2}' eat.txt`
- `awk -F: '{print $NF}' /etc/passwd`

2. **cat**: Command to see content of a file.

Syntax: `cat`

Examples:
- `cat /etc/passwd`
- `cat food_list.txt`

3. **cp**: Command that allows you to copy files and directories.

Syntax: `cp`

Examples:
- `cp Downloads/wall.zip Pictures/`
- `cp -r Downloads/Wall/ Pictures/`

4. **cut**: Is used to extract a specific section of each line of a file and display it to the screen.

Syntax: `cut`

Examples:
- `cut id ':' -f1 /etc/passwd`
- `cut -d ',' -f1,7 --output-delimiter=' : ' etc/passwd`

5. **grep**: Search for text in a file (case sensitive).

Syntax: `grep`

Examples: 
- `grep 'dracula' ~/Documents/dracula.txt`
- `grep -o 'dracula' ~/Documents/Books/dracula.txt`

6. **head**: Displays the top N number of lines of a given file. (prints 10 first lines by default)

Syntax: `head`

Examples:
- `head ~/Documents/dracula.txt`
- `head -5 ~/Documents/dracula.txt`

7. **ls**: list files in directory.

Syntax: `ls`

Examples:
- `ls ~/Downloads/`
- `ls -1 ~/Downloads/`

8. **man**: shows manual of a command.

Syntax: `man`

Examples:
- `man ls`
- `man cut`

9. **mkdir**: Command to make directories.

Syntax: `mkdir`

Examples:
`mkdir Vacation`
`mkdir -p Vacation/beaches`

10. **mv**: Moves and renames directories.

Syntax: `mv`

Examples:
- `mv Downloads/game.sh Documents/`
- `mv essay.txt book_report.txt`

11. **tac**: Displays content of file from bottom to top.

Syntax: `tac`

Examples:
- `tac essay.txt`
- `tac ~/Documents/essay.txt`

12. **tail**: Displays last N number of lines of a given file.(prints last 10 by default)

Syntax: `tail`

Examples:
- `tail ~/Documents/Book/dracula.txt`
- `tail -5 ~/Documents/Book/dracula.txt`

13. **touch**: Used to makes files in directories.

Syntax: `touch`

Examples:
- `touch foods.txt`
- `touch notes.txt homework.py`

14. **tr**: translate (exchange 1 word for another)

Syntax: `tr`

Examples:
- `cat file.txt | tr '.' ','`
- `cat file.txt | tr "[:space:]" '\t'`

15.  **tree**: List contents of directories in a tree-like format.
   
Syntax: `tree`

Examples:
- `tree ~/Downloads/`
- `tree -d ~/Documents/`

## Question 2

1. How to work with multiple terminals open?
- On the top left there are 2 buttons that you can press to add another terminal so that you can work on both at the same time.

2. How to work with manual pages?
- To get the manual for any command you must type `man` followed by the the command you want the manual for.

3. How to parse (search) for specific words in the manual page?
- To search for specific words in the manual page you would use `man ls | grep "list"`.

4. How to redirect output (> and |)?
Examples:
- ` ls -lA ~ > all-files-in-home.txt`
- `man ls | grep "list"`

5. How to append the output of a command to a file?
- To append an output of a command with out overwriting the file you would use `>>`.

6. How to use wildcards?
- *: `mv *.pdf Documents/`
- ?: `mv program?.py Documents/`
- []:`mv document[A-Z].txt Documents/`
- [!]:`mv new-doc[!0-9].docx Documents/`

7. How to use brace expansion?
- `mkdir -p {cats,dogs}/{videos,pictures}`