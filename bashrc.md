# bashrc

## path ~/.bashrc

``` bash

##myscript
git_branch() {
        git branch 2>/dev/null | grep '^*' | colrm 1 2
}
if [ $(id -u) -eq 0 ];
then #super user
    PS1="\[\e[1;32m\]\u\[\e[m\] @ \[\e[0;34m\]\w\[\e[1;30m\] on\[\e[1;36m\] ⎇  \$(git_branch)\n\[\e[0;32m\] ↳ \[\e[0m\]\$ "
else #normal user
    PS1="\[\e[1;34m\]\u\[\e[m\] @ \[\e[1;34m\]\w\[\e[1;30m\] on\[\e[0;36m\] ⎇  \$(git_branch)\[\e[0m\] \$ "
fi

alias ..="cd .."
alias cl="clear"
alias mproj="cd /mnt/c/Users/6655/Documents/Project"
alias mavc="mvn clean"
alias mavp="mvn package"
alias jvr="java -jar"
HISTTIMEFORMAT='<%y/%m/%d %H:%M:%S> '
```
