# Level 14 → Level 15
> The password in this level can be retrieved by sending bandit14’s password to **`port 30000 on localhost`**
> 

---

```bash
bandit14@bandit:~$ nmap -p 30000 localhost
Starting Nmap 7.94SVN ( https://nmap.org ) at 2026-01-27 08:21 UTC

Nmap scan report for localhost (127.0.0.1)

Host is up (0.000087s latency).

PORT      STATE SERVICE

30000/tcp open  ndmps

Nmap done: 1 IP address (1 host up) scanned in 0.04 seconds

bandit14@bandit:~$ echo "Bandit14’s PasswordPasswords" | nc localhost 30000
Correct!
```