# Level 13 → Level 14
> The user bandit13 had the **Private key** so we get access to bandit14
> 

---

```bash
bandit13@bandit:~$ cat sshkey.private

----BEGIN RSA PRIVATE KEY-----
XxXxxXxXxxxXxXxXxXxXxXxXx
-----END RSA PRIVATE KEY-----
```

- Then we copy the key and logout by `exit`

```bash
[liveuser@blackarch]-[~]
>>> echo "----BEGIN RSA PRIVATE KEY-----
XxXxxXxXxxxXxXxXxXxXxXxXx
-----END RSA PRIVATE KEY-----" > private.key
```

- `private.key` file is **too open** by default so **everyone** can read that file

```bash
[liveuser@blackarch]-[~]
>>> chmod 600 private.key

[liveuser@blackarch]-[~]
>>> ssh -i private.key bandit14@bandit.labs.overthewire.org -p 2220

bandit14@bandit:~$ cat /etc/bandit_pass/bandit14
```