# Leak report
checkwhitespace.c has one leak problem which is caused by Uncleaned passed pointer. So what we need to do is just freeing the memory at the end of the code. 
check_whitespace_test.cpp has 8 leak problems, but all of them are caused by the same reason: strip test. So what we need to do is creating a variable first. Then using the variable running the test. Finally, we free the variable to avoid leak problem. 
_Use this document to describe whatever memory leaks
you find in `clean_whitespace.c` and how you might fix
them. You should also probably remove this explanatory
text._
