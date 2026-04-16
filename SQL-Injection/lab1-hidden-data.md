# SQL Injection - Hidden Data Lab

##  Problem
The application displays only released products, while unreleased products are hidden.

##  Payload
Gifts' OR 1=1--

##  Explanation
The single quote (') is used to close the string.

OR 1=1 makes the condition always true.

-- is used to comment out the remaining part of the query, which removes the condition (AND released = 1).

##  Result
All products were displayed, including the hidden/unreleased ones.
