**Creating a README.md file for Shell, init files, variables and expansions**

0.Create a script that creates an alias.
Name: ls
Value: rm *
1.Create a script that prints hello user, where user is the current Linux user.\n
2.Add /action to the PATH. /action should be the last directory the shell looks 
into when looking for a program: export PATH=$PATH:/action
3.Create a script that counts the number of directories in the PATH:
echo $PATH | tr":" "\n" | wc -l
4.Create a script that lists environment variables: printenv
5.Create a script that lists all local variables and environment variables, and functions: set
6.Create a script that creates a new local variable.
Name: BEST
Value: School
BEST="School"
7.Create a script that creates a new global variable.
Name: BEST
Value: School
export BEST="School"
8.Write a script that prints the result of the addition of 128 with the value 
stored in the environment variable TRUEKNOWLEDGE, followed by a new line:
echo $((TRUEKNOWLEDGE+128))
9.Write a script that prints the result of POWER divided by DIVIDE, followed by a new line.
POWER and DIVIDE are environment variables:
echo $((POWER/DIVIDE))
10.Write a script that displays the result of BREATH to the power LOVE

BREATH and LOVE are environment variables
The script should display the result, followed by a new line:
echo $((BREATH\*\*LOVE))
11.Write a script that converts a number from base 2 to base 10.
The number in base 2 is stored in the environment variable BINARY:
echo $((2#$BINARY))
12.Create a script that prints all possible combinations of two letters, except oo.
Letters are lower cases, from a to z
One combination per line
The output should be alpha ordered, starting with aa
Do not print oo
Your script file should contain maximum 64 characters:
echo {a..z}{a..z} | tr" " "\n" | grep -v "oo"
13.Write a script that prints a number with two decimal places, followed by a new line.The number will be stored in the environment variable NUM:
printf "%.2f\n" $NUM
14.Write a script that converts a number from base 10 to base 16.
The number in base 10 is stored in the environment variable DECIMAL:
printf "%.x\n" $DECIMAL 
