## Files

`vi` / `vim` is a very common cli editor for Linux. Below are some settings to help with yaml formatting.

[~/.vimrc](files/.vimrc)
```
set nu
set expandtab
set shiftwidth=2
set tabstop=2
```

Configuring aliases in your shell can save time and common mistakes.

[~/aliases](files/aliases)
```
# autocomplete
alias k='kubectl'

source <(kubectl completion bash)
complete -F __start_kubectl k
```

## Links

* https://github.com/dgkanatsios/CKAD-exercises
* https://kubernetes.io/docs/reference/kubectl/cheatsheet