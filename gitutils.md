# Git Utils
Quick reference for git use on your projects.

![Git lifecycle](https://ia601400.us.archive.org/12/items/lifecycle_201909/lifecycle.png)

## Setup... And starting !

### Initialization

```console
$ cd /Users/user/project/src
$ git init
```

### Verifying configuration

```console
$ git config --list --show-origin
```

### Getting help

These commands are nice because you can access them anywhere, even offline.

```console
$ git help <verb>
$ git <verb> --help
$ man git-<verb>
```

### Adding files

```console
$ git add *.c
$ git add LICENSE
```

### Commit 

```console
$ git commit -m 'initial project version'
```

### Clonning repository

```console
$ git clone https://github.com/jonatanmv/Git-Utils
```

or

```console
$ git clone https://github.com/jonatanmv/Git-Utils local_directory
```

### Checking status of your files

```console
$ git status
```

### Ignoring files

You can easily create a *.gitignore* file this way:

```console
$ cat .gitignore
*.[oa]
*~
```

Here another *.ignorefile*

```console
# ignore all .a files
*.a

# but do track lib.a, even though you're ignoring .a files above
!lib.a

# only ignore the TODO file in the current directory, not subdir/TODO
/TODO

# ignore all files in any directory named build
build/

# ignore doc/notes.txt, but not doc/server/arch.txt
doc/*.txt

# ignore all .pdf files in the doc/ directory and any of its subdirectories
doc/**/*.pdf
```

### Commit history

```console
$ git clone https://github.com/schacon/simplegit-progitx1x1x
```
