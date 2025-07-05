# chmod, change mode(permissions)

## Context: 

1 - POSIX files have permissions for owner(user), group, other to read, write, or execute.

2 - ```ls -la``` lists current working directory's files including all hidden files(-a) and in the long list format(-l)

3 - The 10 char file permissions string. The first char denotes if it is a file(-) or directory(d) and each set of three chars after it are the read(r), write(w) and execution(x), three sets of three chars for user/owner(u), group(g) and other(o)
```
trevorstahl@Mac chmod_temp % ls -la
total 0
drwxr-xr-x   3 trevorstahl  staff    96 Jul  5 14:59 .
drwxr-x---+ 53 trevorstahl  staff  1696 Jul  5 14:59 ..
-rw-r--r--   1 trevorstahl  staff     0 Jul  5 14:59 somet.txt
trevorstahl@Mac chmod_temp %
```
-rw-r--r--, first char - means file, and user can read and write, group can read, other can read,


## Basic Usages:

```chmod u-x some.xyz``` change mode, user loses execution, on file some.xyz

```chmod g+rw any.txt``` change mode, group gets read and write, one any.txt
