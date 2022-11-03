the shell maintains a set of information during each shell session, known as the environment. it's just a series of key-value pairs that define properties like:

- home directory
- working directory
- name of shell
- name of the logged in user
- etc...

use the printenv command (or > printenv | less) to view the environment variables and their current values

<!--  parameter expansion -->

example:

> echo $environment_variable #==> variable's value
> ex.
> echo $USER #==> gcochran

# defining variables

to define a shell variable, use VARIABLE=VALUE
exs.
num=821
color="purple"

to define an enivornment variable, use export VARIABLE=VALUE
exs.
export num=821
(or can do after ie
num=821
export num)
export color="purple"

- he defines his variables in lowercase b/c all environment-defined variables are in all caps

//
shell variables are similar to local variables, they only exist in our current shell session

environment variables are still local but will persist for child shells

# PROMPT variable (the variable that governs our prompt) [PS1 on linux]

note that since im using oh-my-zsh i cant change my prompt the same way that is standard

# Aliases

we can define our own commands using the alias keyword
ex.
alias ll = 'ls -lh'
... now can just type ll in instead of ls -lh
#==> note that this already exists in zsh

to have these aliases persist for all future sessions, define them in the .bashrc (or .zshrc) file -- in my case, most of my aliases are defined in oh-my-zsh rather than the .zshrc file
https://github.com/agnoster/agnoster-zsh-theme
