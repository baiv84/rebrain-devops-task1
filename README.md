# GIT in a nutshell

<h4 align="center">
  <img alt="rebrainme git module" src="git.jpg">
</h4>

> Programs must be written for people to read, and only incidentally for machines to execute.

> Harold Abelson, Structure and Interpretation of Computer Programs
tags: 1984


## Preamble

Git is a powerful and popular version control system that enables effective tracking of changes in source code. It was developed by Linus Torvalds in 2005 for Linux kernel development and It is used for keeping track of code changes and collaborating with others on code. It uses a decentralized model where each developer has their own copy of the repository and works immediately on the project.


Here are some basic and most important features of Git:

* Distributed System
* Compatibility
* Non-linear Development
* Branching
* Lightweight
* Speed
* Open-Source
* Reliable
* Secure


GIT is hosted at https://git-scm.com/

## Control version systems comparison

|Software|Maintainer|Status|Repository model|Supported platforms|License|
|:-|:-:|:-:|:-:|:-:|:-:|
|GIT|Junio C Hamano|Active|Distributed|POSIX, Windows, macOS| GPLv2.0|
|Mercurial|Mercurial community|Active|Distributed|POSIX, Windows, macOS| GPLv2.0|
|Subversion |Apache Software Foundation|Active|Client-server|Unix-like, Windows, macOS| Apache-2.0|
|CVS|CVS team|partly-supported|Client-server|Unix-like, Windows, macOS|GPLv1.0|


## Use cases

We will explore such cases:
1. [Make simple commit](#make-simple-commit)
2. [Merge branches](#merge-branches)
3. [Control state](#make-control-of-state)


# Make simple commit

#### Modify files and add them to git index
```
$ vi README.md
```

```
$ git add README.md
```

```console
$ cp ~/Downloads/nginx.conf ./nginx.conf
```

```console
$ git add nginx.conf
```

##### Apply git commit
```
$ git commit -m "Make simple commit"
```

##### Push all changes to the git server
```console
$ git push -uf origin main
```

# Merge branches
```
$ git checkout master
Switched to branch 'master'

$ git merge iss53
Merge made by the 'recursive' strategy.
index.html |    1 +
1 file changed, 1 insertion(+)
```

<h4 align="center">
  <img alt="common readme" src="merge.png">
</h4>

# Make control of state

##### Make sure all commits visible in log
```console
$ git log
```

##### Make sure nothing to commit
```console
$ git status
```

# Projects goals

This project was written as a study project for DevOps rebrainme.com course [Rebrainme.com](https://rebrainme.com/)
