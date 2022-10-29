some programmers never use nano, nano is a choice

normal workflow for a user ... use GUI with Finder to open files in an app like TextEdit, MSFT Word, etc

dont need to use VS Code, can work exclusively with a command line editor like Nano (others are vim and emacs (there are many, these 3 are prob the most popular)) so that code exclusively through our terminal

to open an existing file with nano... > nano example_file.txt

to 'save as' the nano file, use the WriteOut shortcut .... ctrl-o
then can save with ctrl-s
to cancel a command, ctrl-c
to exit nano, ctrl-x

can use nano command rather than touch to create a new file that doesn't exist

1. nano ex2file.txt [will open this new file, is not created yet]
2. write some code, etc
3. ctrl-o, decide file name, and now the file will be created

## he doesnt recommend using nano as your main editor, but does recommend using it for making files quickly && occasionally on some machines will not have access to a GUI or text editors and therefore can only use command line editors like nano to program on that machine

ctrl-g will show all the nano shortcuts (there are many) -- note that commands in nano have very different meanings than standard macos shortcut commands
notes that ctrl-g is written as ^G

M-U signifies esc-u keys

ctrl-W searchPhrase #==> allows us to search through a file (forward from the cursor, by default)

esc-shift-4 #==> wraps lines

to search for someting and replace it ... ctrl-\

the spell check is disabled by default ... can edit stuff like this in the nano configuration file @
/etc/nanorc
