to see previously exicuted commands -> history
    to search history ->   history | grep cmd

to type out previous command -> !!
to type out nth command -> !n

In Linux everytime a command is run, these three invisible channels 
    are opened which handle the flow of information
    
            Number           Name          Abbreviation
              0         Standard Input         stdin
              1         Standard Output        stdout
              2         Standard Error         stderr

you can Combine commands with pipes (|)
    For example - history | grep ssh
    
to redirect error messages to void -> 2>/dev/null

*shell operators*

Use & when you want tasks to run simultaneously in the background.
        Starts Command 1 in background, immediately runs Command 2.
        
Use && when tasks must run one after another, and the second task depends on the success of the first.

> means overwrite/newfile

>> means append/add to the last line
