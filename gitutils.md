# Git Utils
Quick reference for git use on your projects.

![Git lifecycle](https://ia601400.us.archive.org/12/items/lifecycle_201909/lifecycle.png)

## Setup... And starting !

### Initialization

```console
$ cd /Users/user/project/src
$ git init
```

### Getting help

These commands are nice because you can access them anywhere, even offline.

```console
$ git help <verb>
$ git <verb> --help
$ man git-<verb>
```

### Verifying configuration

```console
$ git config --list --show-origin
```

### Setup your info 

If not already done (as global config for example) setup your name and email.

```console
$ git config --global user.name "Your Real Name"
$ git config --global user.email "you@email.com"
```

### Setting up local repository

If your start from an existing project clone it.

```console
$ git clone git@github.com:jonatanmv/Git-Utils.git
```
or
```console
$ git clone https://github.com/jonatanmv/Git-Utils local_directory
```

### Setting up remotes

You can check your remotes info with ```git remote```. For example, when you clone a repository it will add automatically the *origin* remote. So ```git fetch origin``` fetches any new work that has been pushed to that server since you cloned or fetched.

```console
$ git remote -v
$ git remote show origin
```

And you add remotes like this:

```console
$ git remote add origin git@github.com:jonatanmv/Git-Utils.git
$ git remote add paul https://github.com/paulboone/Git-Utils
```

So you will download lates changes on remotes with ```git fetch <remote>```. *fetch* only download info not the actual files. For that you will use *pull* (It will fetch and download changes).

```console
$ git pull origin
```

### Adding files

```console
$ git add *.c
$ git add LICENSE
```

### Checking status of your files

```console
$ git status
```

### Commit 

```console
$ git commit -m 'initial project version'
```

### Ignoring files

You can easily create a *.gitignore* file this way:

```console
$ cat .gitignore
```

```
__pycache__
*~
*.pyc
.DS_Store
.gitignore
logfiles/
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
