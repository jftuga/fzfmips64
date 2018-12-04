# fzfmips64
fzf for the Linux mips64 architecture including Ubiquiti EdgeRouters

This is a static binary for [fzf](https://github.com/junegunn/fzf) that will run on Ubiquiti EdgeRouters. 

You *must* set the **FZF_DEFAULT_COMMAND** environment variable before running fzf.

```

ubnt@ubnt:~$ export FZF_DEFAULT_COMMAND="find . -path '*/\.*' -prune -o -type f -print -o -type l -print 2> /dev/null | sed s/^..//"

ubnt@ubnt:~$ fzf --version
0.17.5 (b46227d)
```

