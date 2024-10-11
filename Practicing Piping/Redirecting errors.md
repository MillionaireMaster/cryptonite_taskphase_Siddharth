# Redirecting errors

 A File Descriptor (FD) is a number the describes a communication channel in Linux. We're already familiar with three:
 
    FD 0: Standard Input
    FD 1: Standard Output
    FD 2: Standard Error

A `>` without a number implies 1>, which redirects FD 1 (Standard Output).
In this challenge we have to type `/challenge/run > myflag 2> instructions`.
Then we have to type `cat instructions` and then `cat myflag` to get the flag.
