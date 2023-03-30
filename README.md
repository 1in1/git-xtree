## git-xtree

Tiny script of mine to pretty-print the history tree, derived from some stuff in [this stackoverflow question](https://stackoverflow.com/questions/1057564/pretty-git-branch-graphs). Pulling into a separate repo to share.

To install, drop `git-xtree` in your `PATH` and add

```
[alias]
    log-with-markers = log --all --graph --decorate=short --date-order --color --format=format:'%C(bold blue)%h%C(reset)§%C(dim normal)(%cr)%C(reset)§%C(auto)%d%C(reset)§§\n§§§       %C(normal)%an%C(reset)%C(dim normal): %s%C(reset)'
```

to your `gitconfig`. Apologies for using `zsh` solely for `colors` :)

Example (calling `git xtree` from repo root):
![Usage example for git-xtree](https://datas.ink/assets/git-xtree.png)
