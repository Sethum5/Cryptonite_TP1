#position yet elsewhere

```bash
Connected!
hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /usr/share/zoneinfo/posix/Asia directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /usr/share/zoneinfo/posix/Asia
hacker@paths~position-yet-elsewhere:/usr/share/zoneinfo/posix/Asia$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{wuh1_hblbfReZ1mYM9Res1s6_hW.dhDN1QDL4IjN0czW}
```

i directly ran /challenge/run and then it gave me in correct directory i am supposed to be in and then i used cd to change the directory to that one and then again ran /challenge/run to retrieve the flag
