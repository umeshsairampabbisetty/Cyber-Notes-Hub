to manage permissions of files and folders -> chmod
              chmod [who][operation][permissions][filename]
                        (or)
                    chmod [Octal Number][filename]
    -R -> to recursively apply changes to all stuff in the folder

                --detailed explanation below--
                
*Ownership Classes*
There are mainly 3 types of owners
    1 - user(u) 
    2 - group(g)
    3 - others(o)
    4 - all(a) 
    
*Permission Types*
There are 3 main permissions for any file/folder (both have similar but not same functions)
    
            Value    Symbol
    read          4          r
    write          2          w
    execute          1          x
    
-Permission Strings-
      -   r w x   r - x   r - -
       |   |---|   |---|   |---|
    Type   User   Group   Others
    
   First character: File type (- = normal file, d = directory, l = symlink).
   Chars 2–4 (rwx): User has Read, Write, Execute.
   Chars 5–7 (r-x): Group has Read and Execute (no Write).
   Chars 8–10 (r--): Others have Read-only.
   
*Changing Permissions with chmod*

  A. Octal (Numeric) Notation
    Each permission is mapped to a binary/numeric value. Add them up for each group:
           r = 4   w = 2   x = 1
    Examples:  rwx = 4 + 2 + 1 = 7
               r-x = 4 + 0 + 1 = 5
               --- = 0 + 0 + 0 = 0
    Format: chmod 750 script.sh     # User: rwx (7), Group: r-x (5), Others: --- (0)
    
  B. Symbolic Notation
    Uses symbols to add (+), remove (-), or set (=) specific permissions.
    Syntax:  chmod [who][operation][permissions][filename]
    -R -> to recursively apply changes to all stuff in the folder

YET TO LEARN!!!---->
    
-Special Permissions bits-

   1. SUID (Set User ID)
    Numeric value: 4000 (prepended to standard permissions, e.g., chmod 4755).
    Visual notation: An s in the user's execute field (-rwsr-xr-x).
    Cybersecurity Impact: When executed, the process runs with the file owner's 
                permissions (often root), regardless of who executes it.
    Security Risks: Standard binaries like /usr/bin/passwd need SUID to update /etc/
               shadow. However, if custom or vulnerable binaries have SUID set, 
                attackers can exploit them to gain root access (GTFOBins).

   2. SGID (Set Group ID)
    Numeric value: 2000 (e.g., chmod 2755).
    Visual notation: An s in the group's execute field (-rwxr-sr-x).
    Cybersecurity Impact:
        On files: Runs with the permissions of the file's group.
        On directories: New files created inside automatically inherit the 
           directory's group ownership.

   3. Sticky Bit
    Numeric value: 1000 (e.g., chmod 1777).
    Visual notation: A t at the end (drwxrwxrwt).
    Cybersecurity Impact: Used on shared directories (like /tmp). Allows anyone to 
                read/write, but only the file owner or root can delete 
                  or rename files inside. Prevents malicious users from 
                    wiping other users' temporary files.

                        --end--

to check the current user -> whoami

to check the info of logged in users -> who

to show the identity information of an user -> id

to change the password -> passwd
