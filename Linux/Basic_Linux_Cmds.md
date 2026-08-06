to check the present working directory -> pwd

to check what files and folders are there -> ls 
	-a -> shows all the files including hidden files
	-l -> shows perms and the sizes of the files
	-h -> human readable sizes
	
to change the pwd -> cd
	.. -> go back one folder
	  (or) ~ -> go home
	/ -> go root
	- -> previous working directory
	
to make a new folder/directory -> mkdir
	-p -> parents/create nested folders

to remove a file/folder -> rm
	-r -> recursive/delete a directory
	-f -> force delete
	
to copy and paste folders or files/with different type -> cp
	syntax -> cp source destination
	-r -> recursive/copy the entire directory

to move/rename files/folders - mv 
	syntax -> mv source destination
	no need of -r -> because its just changing the index/label in the main table

to create new files -> touch

to read and create files/concatenate -> cat 
	syntax for making a file and then writing data into it -> cat > newfilename.ext
								 Ctrl + D to save it (done)

to see the beginning of a file -> head
	default it shows only first 10 lines
	-(number) -> that many no of lines from start, ex head -50 lol.txt
	
to see the end of the file -> tail
	default it shows only last 10 lines
	-(number) -> that many no of lines from end, ex head -50 lol.txt
	-f -> follow/forever continuously watches the file
	
to search text inside files -> grep
	syntax -> grep word file.tct
	-i -> ignore case
	-n -> show line numbers
	-r -> search every file
	
to find files -> find
	syntax -> find location options, "." means current location
	-name -> ex: find ~ -name "*.txt"
	-empty -> finds empty files
	-size -> ex: find . -size +100M
	! -> means "NOT", for commands after this
	-executable -> files which can run
	-type -> file or directory or others
	-user -> which user has access
	-group -> which group has access
	
to manage permissions of files and folders -> chmod
	          chmod [who][operation][permissions][filename]
			    	    (or)
	     	       chmod [Octal Number][filename]
	-R -> to recursively apply changes to all stuff in the folder
	
to see previously exicuted commands -> history
	to search history ->   history | grep cmd

to type out previous command -> !!
to type out nth command -> !n

to see the manual of a cmd -> man
	inside manual "/" opens finder
	
you can Combine commands with pipes (|)
	For example - history | grep ssh
	
to redirect error messages to void -> 2>/dev/null

to print or write text -> echo
	write to a new file -> echo "Hello" > file.txt
	append to a old file (add at the last line) -> echo "World" >> file.txt
	
to edit text files in terminal -> nano

view large file one page at a time -> less
	Navigation:Space → Next page
	           b → Previous page
	           /word → Search
		   q → Quit
		   
to know about basic info of the files -> file

to know about the detailed info of a file -> stat

to find where the command is installed -> which

to find binaries, source code, and manuals of command or anything -> whereis

a very fast file searcher -> locate
	Uses a database, so it may need updating: sudo updatedb
	
to check disk space (disk free) -> df
	-h -> human readable
	
to check usage of storage ( disk usage ) -> du
	-h -> human readable
	-s -> summary of the size of each folder

to sort the contents of a text file -> sort
    By default, it sorts alphabetically (A-Z) and treats numbers as characters, not mathematical values.

   Flag       Name                          What it does   
    -r        Reverse         Sorts backwards (A to Z or highest to lowest)
    -n        Numeric         Sorts numbers by math value, not alphabetically.
    -k      Key (Column)      Sorts based on a specific column of data.


to filter out duplicate lines of text -> uniq
    It only compares a line to the line immediately above or below it.

   Flag        Name                       What it does   
    -u        Unique        Only prints lines that appear exactly once.
    -d       Duplicate      Only prints lines that have duplicates.
    -c         Count        Prefixes each line with its count.
    
to check the current user -> whoami

to check the info of logged in users -> who

to show the identity information of an user -> id

to change the password -> passwd

to check running processes -> ps
	every running process -> ps aux
	
to show real time process monitor - top

A prettier version of top (if installed) -> htop

to terminate a process -> kill
	force kill -> kill -9 ....
	to list all the supported signals -> -l
	
to kill by process name -> pkill










