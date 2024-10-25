# The SUID Bit

The "Set User ID" `SUID` permissions bit allows the user to run a program as the owner of that program's file.
In this challenge we have to type `ls -l /challenge/getroot` then `chmod u+s /challenge/getroot` then `/challenge/getroot` then `cat /flag` to get the flag.
