rather than using Finder app to navigate to different folders, etc

--- The Root Directory -- the starting point for the file system is the root folder. Everything on my mac is inside this root directory. the directory name is "/" (confusingly, there is a sub-directory called root that is below the actual / root directory)

to see the root directory in finder... > open /

--- The Home Directory -- /home contains a home folder for each user on a machine

#

shorthand
/ => root (root directory)
~ => home (directory of the currently logged in user)

#

pwd
#==> print working directory command asks "where am i?" and will print the path of your current working directory starting from the root /

#

ls
#==> the list command will list the contents of a directory.
with no options or arguments, it prints a list of the files and filters located in the current directory
ls path (ex. ls /Users/gcochran/Desktop OR ls Desktop) will list the contents of a specific directory
// useful ls options

ls -l #==> will give us the "long" format for the directory (ex. permissions, size, modification date, etc)

ls -a #==> will show us all files and folders including hidden files/folders (note that hidden files/folders start with a dot (ex. .cache))

#

cd
#==> the change directory command will move us into another directory

- can provide an absolute or a relative path

#

if press tab while typing, terminal will autocomplete ex. cd De(tab) will autocomplete to cd Desktop/

#

a single dot (.) is used to represent the current directory. two dots (..) references the parent directory -- ex. > cd ..

#

cd'ing into a directory is relative to our current directory, ie cant change to a folder two levels down, only one level, unless provide the relative path

we can use absolute paths to specific a location no matter our current location
-- starts from the top (the root / ) and type out the whole path
