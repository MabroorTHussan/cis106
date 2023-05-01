---
name: Mabroor Hussan
course: CIS106
Semester: Spring 2023
---

# Week Report 6

## Wildcards

### * Wildcard
the * wildcard matches from 0 to any number of characters. 
* Examples:
  * List all the text file in a directory
    * `ls *.txt`
  * List all the files that start with the word file
    * `ls file*`
  * Copy all the mp4 files 
    * `cp Downloads/*.mp4 ~/Videos/Movies/`
  
### ? Wildcard
The ? wildcard matches a single character.
* Examples:
    * list all the files that have 3 characters and are followed by the word file in the name
      * `ls ???File*`
    * list all the files with a three-letter extension in a directory
      * `ls *.???`
    * list all files that have x as the second letter in their name
      * `ls ?x*`
### [] Wildcard
The [] wildcard matches any single character inside the brackets
* Examples:
  * list all the files that have either "a" or "b" as the first character in their name
    * `ls [ab]*`
  * list all the files that have a single digit number as the second letter in their name
    * `ls ?[0-9]*`
  * list all the files that have either an uppercase or lowercase letter as the second character in their names
    * `ls ?[[:alpha:]]*`

### Brace Expansion
Brace expansion allows you to generate multiple strings based on a pattern.
* Examples:
  * create directories named "dir1", "dir2", "dir3", "dir4", and "dir5"
    * mkdir dir{1..5}
  * copy "file1.txt", "file2.txt", "file3.txt", "file4.txt", and "file5.txt" to backup directory
    * cp file{1..5}.txt backup/
  * Create the directories "project1/docs", "project1/src", "project2/docs", "project2/src","project3/docs", and "project3/src"
    * mkdir project{1..3}/{docs/src}