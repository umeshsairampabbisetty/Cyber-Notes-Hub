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
    
to edit text files in terminal -> nano

view large file one page at a time -> less
    Navigation:Space → Next page
               b → Previous page
               /word → Search
           q → Quit
           
to know about basic info of the files -> file

to know about the detailed info of a file -> stat

to print or write text -> echo
    write to a new file -> echo "Hello" > file.txt
    append to a old file (add at the last line) -> echo "World" >> file.txt
    
    
