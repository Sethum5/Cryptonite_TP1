# hidden files

```bash
hacker@commands~hidden-files:~$ ls -a /
.   .dockerenv             bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-241701027225051  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:~$ cat /.flag-241701027225051
pwn.college{kJhxhRyqt9TMqfAWYU0D3rbGRCO.dBTN4QDL4IjN0czW}
```

i used ls -a as the command to read the hidden files and the / to mention the directory and then i read the file which started with a . which otherwise would be hiddent to get the flag
