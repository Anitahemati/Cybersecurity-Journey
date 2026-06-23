Linux Day 8

Topics Covered

- Shell and Bash
- PATH Environment Variable
- Built-in vs Executable Commands
- Shell Variables
- Environment Variables (export)
- Aliases
- Introduction to .bashrc

Commands Practiced

echo $USER
echo $HOME
echo $SHELL
echo $PATH

which ls
which cat
which grep

type ls
type cd

name="Anita"
echo $name

export project="AppSec"
env | grep project

alias ll="ls -la"
alias
unalias ll

Key Takeaways

- Bash is a shell that interprets and executes commands.
- PATH determines where executable files are searched for.
- Some commands are shell built-ins (e.g., cd), while others are executable files (e.g., ls).
- Shell variables exist only in the current shell.
- Environment variables can be inherited by child processes.
- Aliases provide shortcuts for frequently used commands.
