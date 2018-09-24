# Git aliases and configs

## Git-aliases

Add these lines into `alias` section in yours `.gitconfig`

```
[alias]
        a = add .
        co = checkout
        st = status
        lg = log --graph --pretty=format:'%C(110)%h%Creset %C(243)[%an]%Creset | %C(250)%s%Creset (%ad, %ar)%C(cyan)%d%Creset' --date=short -10
        ca = "!git add .;git commit -m"
        caa = "!git add .;git commit --amend --no-edit"
```

Or in console for each alias

```
git config --global alias.[alias] [command]
```

Check the [documentation](https://git-scm.com/book/en/v2/Git-Basics-Git-Aliases)

## Formatting 'git log' output

Run in console following comands:

```
git config --global pretty.verminal format:'%C(#FFCC00)%h%C(reset) %cd | %s%C(#5ac8fa)%d%C(reset) [%an]'
git config --global format.pretty verminal

git config --global log.date format-local:'%F %R'
```
