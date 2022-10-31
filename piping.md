ie constructing pipelines

using the pipe character | to connect two commands

we can take the output of one command and redirect it (aka pipe it) to the input of the second command

> command1 | command2

ex. piping ls content to less command

> ls filePath | less

[[note that ls -1 will put each on its one line]]

ex2. how many total files are in a folder?

> ls folderPath -1a | wc -l

- note that combine redirection and piping ... ex. ls filePath -1a | wc -l > outputIn

- can pipe multiple times in a row
  ex. find the 3 largest files in a directory ... [note that is an inefficient way to find this info, simply using as demo]
  > ls directoryPath -lh | sort -k5hr | head -3 > newFile
  > explained ^... print the long-form, human-readable info for a directory; pipe this to the sort command so that it sorts this info by the 5th column (which is the size column), and sorts by human readable so that will correctly sort the sizes of each file in order from smallest to largest, and reverse this so that is from largest to smallest (largest at top of list), then pipe this info to the head command so that only prints the 3 files at the top of the list (ie the 3 largest) and put this as the output for a new file
