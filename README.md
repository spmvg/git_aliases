This is a snippet containing my git aliases.
I type these commands many times every day, so every optimization helps!

```bash
source /mingw64/share/git/completion/git-completion.bash

alias gs='git status'
alias gd='git diff'
__git_complete gd _git_diff
alias gds='git diff --stat=200'
__git_complete gds _git_diff
alias gdw='git diff --word-diff'
__git_complete gdw _git_diff
alias gk='gitk'
alias gc='git commit -m'
alias gca='git commit -am'
alias gp='git push'
alias gpo='git push --set-upstream origin HEAD'
alias ga='git add --all; gitk'
alias gl='git pull'
alias go='git checkout'
__git_complete go _git_checkout
```
