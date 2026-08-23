# Level 16 → Level 17

```bash
bandit16@bandit:~$ nmap -v --open -p- localhost

31046/tcp open  unknown

31518/tcp open  unknown

31691/tcp open  unknown

31790/tcp open  unknown

31960/tcp open  unknown

bandit16@bandit:~$ echo "Bandit16's Password" | openssl s_client -connect localhost:31790 -quiet

----BEGIN RSA PRIVATE KEY-----
XxXxxXxXxxxXxXxXxXxXxXxXx
-----END RSA PRIVATE KEY-----
```

```bash
[liveuser@blackarch]-[~]
>>> echo "----BEGIN RSA PRIVATE KEY-----
XxXxxXxXxxxXxXxXxXxXxXxXxxx
-----END RSA PRIVATE KEY-----" > private.key

[liveuser@blackarch]-[~]
>>> chmod 600 private.key

[liveuser@blackarch]-[~]
>>> ssh -i private.key bandit17@bandit.labs.overthewire.org -p 2220

bandit17@bandit:~$ cat /etc/bandit_pass/bandit17
```