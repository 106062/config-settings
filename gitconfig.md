# gitconfig

## path ~/.gitconfig

``` .gitconfig
[user]
    email = 
    name = 
[merge]
    ff = false
[push]
    default = current
[pull]
    default = current
    ff = only
[alias]
    lg = log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --branches
```
