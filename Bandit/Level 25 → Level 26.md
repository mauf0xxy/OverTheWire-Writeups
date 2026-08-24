# Level 25 → Level 26

```bash
bandit25@bandit:~$ cat bandit26.sshkey

----BEGIN RSA PRIVATE KEY-----
XxXxxXxXxxxXxXxXxXxXxXxXx
-----END RSA PRIVATE KEY-----
```

```bash
[liveuser@blackarch]-[~]
>>> echo "----BEGIN RSA PRIVATE KEY-----
XxXxxXxXxxxXxXxXxXxXxXxXxxx
-----END RSA PRIVATE KEY-----" > private.key
```

```bash
bandit25@bandit:~$ cat /etc/passwd | grep bandit26

bandit25@bandit:~$ cat /usr/bin/showtext

#!/bin/sh

export TERM=linux
exec more ~/text.txt
exit 0
```

- `more` is a file perusal filter for crt viewing, the idea here is by resizing the terminal like this

![More_Command](https://github.com/mauf0xxy/OverTheWire-Writeups/blob/main/Bandit/images/window_terminal_size.png)

- by pressing **[ v ]** it will switch to **VISUAL mode,** allowing to run commands

```bash
:set shell?

usr/bin/showtext

:set shell=/bin/bash

:shell

bandit26@bandit:~$ cat /etc/bandit_pass/bandit26
```

[def]: mauf0xxy/OverTheWire-Writeups/Bandit/images/window_terminal_size.png