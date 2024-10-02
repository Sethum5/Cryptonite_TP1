# implicit relative paths, from /

```bash
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{4I5k5F9YwoZaFH2uXglMNxyTFiy.dlDN1QDL4IjN0czW}
```

i had to change the cwd to / from the existing one using cd command in order to run challenge/run so that i can retrieve the flag
