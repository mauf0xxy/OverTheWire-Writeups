# Level 10 → Level 11
> The password is stored in the file **data.txt** which is encoded in **`Base64`**
> 

---

```bash
bandit10@bandit:~$ cat data.txt | base64 -d 
```
---

**`base64`** — **Encode** binary data into ASCII text and **decode** ASCII text back into binary data

**`-d`** — **Decode**