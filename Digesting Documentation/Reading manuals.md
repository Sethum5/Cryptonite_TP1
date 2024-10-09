# Reading manuals

```bash
CHALLENGE(1)                                      Challenge Commands                                     CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit

       --cczlke NUM
              print the flag if NUM is 961

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)

pwn.college                                            May 2024                                          CHALLENGE(1)
hacker@man~reading-manuals:~$ /challenge/challenge --cczlke 961
Correct usage! Your flag: pwn.college{cczUK9OIPl_A6WKVkAeqUU1AmAM.dRTM4QDL4IjN0czW}
```

i accessed the flag from the challenge program using the man challenge command and then the the location given to me
