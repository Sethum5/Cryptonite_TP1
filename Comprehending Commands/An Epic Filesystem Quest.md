# An Epic filesystem quest

```bash
Connected!
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
SPOILER  boot       dev  flag  lib    lib64   media  nix  proc  run   srv  tmp  var
bin      challenge  etc  home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~an-epic-filesystem-quest:/$ cat flag
cat: flag: Permission denied
hacker@commands~an-epic-filesystem-quest:/$ cat SPOILER
Lucky listing!
The next clue is in: /usr/lib/python3/dist-packages/twisted/conch/insults/__pycache__

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/lib/python3/dist-packages/twisted/conch/insults/__pycache__
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/twisted/conch/insults/__pycache__$ ls -a
.   .TRACE                   client.cpython-38.pyc  helper.cpython-38.pyc   text.cpython-38.pyc
..  __init__.cpython-38.pyc  colors.cpython-38.pyc  insults.cpython-38.pyc  window.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/twisted/conch/insults/__pycache__$ cat .TRACE
Yahaha, you found me!
The next clue is in: /opt/gef/.git/objects/info
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/twisted/conch/insults/__pycache__$ cd /opt/gef/.git/objects/info
hacker@commands~an-epic-filesystem-quest:/opt/gef/.git/objects/info$ ls
MESSAGE
hacker@commands~an-epic-filesystem-quest:/opt/gef/.git/objects/info$ ls -a
.  ..  MESSAGE
hacker@commands~an-epic-filesystem-quest:/opt/gef/.git/objects/info$ cat MESSAGE
Great sleuthing!
The next clue is in: /usr/lib/debug/.build-id/2c

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/gef/.git/objects/info$ cd /usr/lib/debug/.build-id/2c
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/2c$ ls -a
.  ..  LEAD  bf146454ea398dbf739865399b78be1aee0431.debug
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/2c$ cat LEAD
Great sleuthing!
The next clue is in: /usr/lib/jvm/java-17-openjdk-amd64
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/2c$ cd /usr/lib/jvm/java-17-openjdk-amd64
hacker@commands~an-epic-filesystem-quest:/usr/lib/jvm/java-17-openjdk-amd64$ ls -a
.  ..  POINTER  bin  conf  docs  include  jmods  legal  lib  man  release
hacker@commands~an-epic-filesystem-quest:/usr/lib/jvm/java-17-openjdk-amd64$ cat POINTER
Lucky listing!
The next clue is in: /opt/linux/linux-5.4/arch/mips/emma/markeins

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/lib/jvm/java-17-openjdk-amd64$ ls /opt/linux/linux-5.4/arch/mips/emma/markeins
ALERT-TRAPPED  Makefile  irq.c  led.c  platform.c  setup.c
hacker@commands~an-epic-filesystem-quest:/usr/lib/jvm/java-17-openjdk-amd64$ cat ALERT-TRAPPED
cat: ALERT-TRAPPED: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/lib/jvm/java-17-openjdk-amd64$ cat /opt/linux/linux-5.4/arch/mips/emma/markeins/ALERT-TRAPPED
Tubular find!
The next clue is in: /opt/aflplusplus/nyx_mode/libnyx/libnyx/target/release/build/libc-e14c74911966ae82
hacker@commands~an-epic-filesystem-quest:/usr/lib/jvm/java-17-openjdk-amd64$ cd /opt/aflplusplus/nyx_mode/libnyx/libnyx/target/release/build/libc-e14c74911966ae82
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/libnyx/libnyx/target/release/build/libc-e14c74911966ae82$ ls -a
.  ..  WHISPER  invoked.timestamp  out  output  root-output  stderr
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/libnyx/libnyx/target/release/build/libc-e14c74911966ae82$ cat Whisper
cat: Whisper: No such file or directory
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/libnyx/libnyx/target/release/build/libc-e14c74911966ae82$ cat WHISPER
Lucky listing!
The next clue is in: /usr/lib/python3/dist-packages/sage_setup/autogen/__pycache__

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/libnyx/libnyx/target/release/build/libc-e14c74911966ae82$ ls /usr/lib/python3/dist-packages/sage_setup/autogen/__pycache__
HINT-TRAPPED  __init__.cpython-38.pyc  __main__.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/libnyx/libnyx/target/release/build/libc-e14c74911966ae82$ ls /usr/lib/python3/dist-packages/sage_setup/autogen/__pycache__/HINT-TRAPPED
/usr/lib/python3/dist-packages/sage_setup/autogen/__pycache__/HINT-TRAPPED
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/libnyx/libnyx/target/release/build/libc-e14c74911966ae82$ CAT /usr/lib/python3/dist-packa
ges/sage_setup/autogen/__pycache__/HINT-TRAPPED
ssh-entrypoint: CAT: command not found
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/libnyx/libnyx/target/release/build/libc-e14c74911966ae82$ cat /usr/lib/python3/dist-packa
ges/sage_setup/autogen/__pycache__/HINT-TRAPPED
Tubular find!
The next clue is in: /usr/lib/python3/dist-packages/docutils/languages

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/libnyx/libnyx/target/release/build/libc-e14c74911966ae82$ cd /usr/lib/python3/dist-packages/docutils/languages
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/docutils/languages$ ls -a
.   MEMO         __pycache__  ca.py  da.py  en.py  es.py  fi.py  gl.py  it.py  ko.py  lv.py  pl.py     ru.py  sv.py     zh_tw.py
..  __init__.py  af.py        cs.py  de.py  eo.py  fa.py  fr.py  he.py  ja.py  lt.py  nl.py  pt_br.py  sk.py  zh_cn.py
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/docutils/languages$ cat MEMO
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{wQMqW0YxnWLmgQfhd1u3EaHPSVb.dljM4QDL4IjN0czW}
```


i followed the instructions ony by one by following which command to use, whcich directory to search, etc. and then found the flag
