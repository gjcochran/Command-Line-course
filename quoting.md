shell will ignore extra spaces, by default.

ex.
echo look at me
#==> look at me

# double quotes

if we wrap text in double quotes, the shell will respect our spacing (views all text as one string) and will ignore special characters except for dollar sign($) [signifies variables], backslash(\), and backtick (`)

pathname expansion, brace expansion, and word splitting will be ignored. however... command substitution and aritmetic expansion will still be performed b/c $ still have meaning inside double quotes

ex.
echo "look at me"
#==> look at me

# single quotes

suppress all forms of substitution (ie $, / and ` characters will now also be ignored)
