# more catting practice

```bash
Connected!
You cannot use the 'cd' command in this level, and must retrieve the flag by
absolute path. Plus, I hid the flag in a different directory! You can find it
in the file /usr/libexec/flag. Go cat it out **without** cding into that
directory!
hacker@commands~more-catting-practice:~$ cat /usr/libexec/flag
pwn.college{I_vmU0DNKPGGjC0H-xlIPHS7Zvb.dBjM5QDL4IjN0czW}
```

since i cannot use cd to change the path to that directory and file and directly use cat i just entered the absolute path of the file as the argument of the cat command(the path was given ) and got the flag
