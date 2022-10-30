# some useful, though not necessary, shortcuts to help navigate more quickly the terminal

// clear whole screen
command > clear
||
ctrl-l || cmd-k

// line jumping
ctrl-a to move the cursor the beginning of a line
ctrl-e to move the cursor the end of a line

// moving characters one character at a time
right arrow key || ctrl-f [forward one character]
left arrow key || ctrl-b [backwards one character]

<!-- thought being that dont have to move hands in order to move the cursor (which have to move right hand off center of the keyboard in order to use the arrow keys) -->

// jumping words

alt/option-f to move the cursor forward one word
alt/option-b to move the cursor backwards one word

<!-- note that i changed a keyboard setting in terminal>preferences to "use option as meta key" in order to make these work -->

// swapping
ctrl-t swaps the current character with the preceding character
alt/option-t swaps the current word with the preceding word

// killing (ie cutting text out)
ctrl-k will kill all text on the line after the cursor
ctrl-u will kill all text on the line before the cursor

alt/option-d will kill the text from the cursor forward to the end of a word
ctrl-w || alt-delete will kill the text from the current cursor backwards thru the beginning of the word

ctrl-d will delete/kill the character underneath the cursor (vs pressing delete key will delete the character left of the cursor)

ctrl-y will retreive the most recently killed text //yanking
