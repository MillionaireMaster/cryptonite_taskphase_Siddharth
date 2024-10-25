# Process exit codes

We can access the exit code of the most recently-terminated command using the special `?` variable and prepending it with `$`.
In this challenge we have to type `/challenge/get-code` then type `echo $?` to get the exit code.
Then we have to type `/challenge/submit-code 123` (where 123 is the exit code) to get the flag.
