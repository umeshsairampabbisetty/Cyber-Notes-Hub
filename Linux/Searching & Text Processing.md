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
    
a very fast file searcher -> locate
    Uses a database, so it may need updating: sudo updatedb

to find where the command is installed -> which

to find binaries, source code, and manuals of command or anything -> whereis

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
    

    

