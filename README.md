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
alias gc='f() { git commit -m "$1 [$(git branch --show-current)]"; }; f'
alias gca='f() { git commit -am "$1 [$(git branch --show-current)]"; }; f'
alias gp='git push'
alias gpo='git push --set-upstream origin HEAD'
alias ga='git add --all; gitk'
alias gl='git pull'
alias go='git checkout'
__git_complete go _git_checkout
alias pr='start $(git remote get-url origin)/pull/$(git remote show origin | grep "HEAD branch" | awk "{print \$NF}")...$(git branch --show-current | sed "s/#/%23/g")?expand=1'
```
