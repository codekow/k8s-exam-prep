# Notes for CKAD Exam

Below are a list of notes for preparing for the CKAD.

## Files

`~/.vimrc`
```
set nu
set expandtab
set shiftwidth=2
set tabstop=2
```

`~/aliases`
```
export ns=default
alias k='kubectl -n $ns'
alias kdr='kubectl -n $ns -o yaml --dry-run=client'
```

## Links

* https://github.com/dgkanatsios/CKAD-exercises