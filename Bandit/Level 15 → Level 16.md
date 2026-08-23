# Level 15 → Level 16
> The password can be retrieved by submitting the password of the current level to **port 30001 on localhost** using SSL/TLS encryption.
> 

---

```bash
bandit15@bandit:~$ echo "Bandit15's Password" | openssl s_client -connect localhost:30001 -quiet
```

---

**`openssl`** — Toolkit for **SSL/TLS** **protocols** and **cryptography**

**`-connect localhost:30001`** — Defines the **target destination**

**`s_client`** — **SSL/TLS client tool**, which **handles the handshakes and data transfer** with a secure server

**`-quiet`** — **Suppresses** standard connection **logs**