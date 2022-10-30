# 3 data streams (standard input, output, and error)

standard input --> command --> standard output || standard error
there are default behaviors, listed below, that can be changed

standard input -- is where a program or command gets its input info from. by default, the shell directs standard input from the keyboard
standard output -- default behavior is commands to output by printing on our terminal screen
standard error also defaults to printing errors to our terminal screen

# redirection describes the ways we can alter the source of standard input, and the destinations for standard output and standard error

<!-- REDIRECTING OUTPUT -->

syntax ...
command > filename
#==> adds the output of the command that runs to that file or a new file with that name

- if the file already exists, it will be completely overwritten by default and contents replaced with the output

<!-- Appending standard output -->

use >> rather than >
#==> allows us to use redirection to an existing file without rewriting that file, instead appending/adding the info from the command we run to the end of that file

# can make a file (and add text to it) using redirection with the echo command, rather than the touch command

ex.
echo meow > cat.txt [[will create a new file cat.txt that contains the text meow inside]]
echo purr >> cat.txt [[will add purr to the text in the cat.txt file]]

<!-- REDIRECTING INPUT -->

syntax ...
command < filename

NOTE that most of the time (100% of time so far in the course) have not used standard input to run commands, so the utility of this redirection is not clear (apparently will be clear with pipelines)

# can redirect standard output and input at the same time

ex.
command < fileprovidedasstandardinput > outputfilethatinputtobeaddedto

<!-- REDIRECTING ERROR -->

syntax ...
command 2> filetoredirectto

typically used to redirect errors to a file to log errors

can append with 2>>

# can redirect standard output and standard error at the same time, just have to put output first

ex. command file(s) > filetooutputto 2> filttosenderrorto

if want to redirect them to same place would write ... 2>&1 || only write &>
ex. command file(s) > filetooutputto 2>&1
ex2. command file(s) &> fileToOutputTo
