# Level 11 → Level 12
> The password is encoded by **`ROT13 (A-Z)`**
> 

---

```bash
bandit11@bandit:~$ cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```
---

**`tr`** — (**Translate**) T**ranslate, delete, and squeeze repeated characters** from standard input and write the result to standard output