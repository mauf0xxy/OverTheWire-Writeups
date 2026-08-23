# Level 19 → Level 20

> when the **`bandit20-do`** file is executed, the program runs with the privileges of the file’s owner (`bandit20`).
> 

---

```bash
bandit19@bandit:~$ ****ls -la ./bandit20-do
-rwsr-x---   1 bandit20 bandit19 14884 Oct 14 09:26 bandit20-do

bandit19@bandit:~$ ./bandit20-do cat /etc/bandit_pass/bandit20
```

---

**`-rwsr-x---`** — **Read**, **Write**, **Execute** + **SUID** enabled