# Level 9 → Level 10

>The password for is stored in the file **data.txt** in one of the few human-readable strings, preceded by several `=` characters.
>

---

```bash
bandit9@bandit:~$ strings data.txt | grep '=’
```
---

**`strings`** — Extracts and prints sequence-formatted, printable characters from any given file