# Level 18 → Level 19

> The password is stored in a file **readme** in the homedirectory. Someone has modified **`.bashrc`** to log you out when you log in with **`ssh`**
> 

---

```bash
[liveuser@blackarch]-[~]
>>> ssh bandit18@bandit.labs.overthewire.org -p 2220 'cat readme'
```