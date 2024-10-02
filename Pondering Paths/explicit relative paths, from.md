#Explicit Relative paths, from/

```bash
Connected!
hacker@paths~explicit-relative-paths-from-:~$ /./challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{wiOaGpbqduO7lyn5FhNLwEWVoMS.dBTN1QDL4IjN0czW}
```

i used cd / to change to the correct directory and then ./challenge/run (as it relative path to the current directory i am in)to get the flag
