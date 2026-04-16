# SQL Injection - Login Bypass Lab

##  Problem
The login system checks both username and password. The goal was to log in without knowing the password.

## Payload
administrator'--

##  Explanation
The single quote (') is used to close the string.

-- comments out the remaining query, which removes the password check.

So the query becomes:
SELECT * FROM users WHERE username = 'administrator'

Now the password condition is ignored.

##  Result
Successfully logged in as the administrator without entering the password.
