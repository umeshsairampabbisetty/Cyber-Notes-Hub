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
