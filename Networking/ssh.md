SSH CHEAT SHEET
    1.    STANDARD PASSWORD LOGIN
Connect using a password:
ssh username@hostname -p PORT (default port 22)
Example: ssh bandit13@bandit.labs.overthewire.org -p 2220
-l  Login username (alternative to username@host)
    2.    PRIVATE KEY LOGIN (-i)
Connect using a private key file(identity file):
ssh -i /path/to/keyfile username@hostname -p PORT
Example: ssh -i ssh.private bandit14@bandit.labs.overthewire.org -p 2220
    3.    FIX KEY PERMISSIONS (chmod 600)
SSH blocks keys that are readable by others. Lock it down first:
chmod 600 keyfile
    4.    RUN SINGLE REMOTE COMMAND
Execute a command on the server and immediately exit:
ssh -i keyfile username@hostname -p PORT "command"
Example: ssh -i ssh.private bandit14@bandit.labs.overthewire.org -p 2220 "cat /etc/bandit_pass/bandit14"

