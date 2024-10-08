# linking files 

```bash
Connected!
hacker@commands~linking-files:~$ ln -s /flag /home/hacker/not-the-flag
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{M-gqqwZLcxIuSb0oLteg4y1Hn_d.dlTM1UDL4IjN0czW}
```

i had to create a symbolic link that points /flag to /home/hacker/not-the-flag so when i run /challenge/catflag it will read from /home/hacker/not-the-flag, it will access the /flag file to get the flag.
