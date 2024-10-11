# Grepping errors

The `>` operator redirects a given file descriptor to a file, and we have used `2>` to redirect fd 2, which is standard error. The | operator redirects only standard output to another program. It can only redirect standard output (file descriptor 1).
The shell has `a >&` operator, which redirects a file descriptor to another file descriptor.
This means that we can have a two-step process to grep through errors: first, we redirect standard error to standard output `(2>& 1)` and then pipe the now-combined stderr and stdout as normal `(|)`
In this challenge we have to type `/challenge/run 2>& 1 | grep pwn.college` to get the flag.
