# Level 28 → Level 29

> The credentials will be in the `README.md` file.
> 

---

```markdown
[liveuser@blackarch]-[~]
>>> git clone ssh://bandit28-git@bandit.labs.overthewire.org:2220/home/bandit28-git/repo

# Bandit Notes
Some notes for level29 of bandit.

## credentials

-   username: bandit29

-   password: xxxxxxxxxx
```

```bash
[liveuser@blackarch]-[~/repo]
>>> git log

commit b5ed4b5a3499533c2611217c8780e8ead48609f6 (HEAD -> master, origin/master, origin/HEAD)

Author: Morla Porla morla@overthewire.org
Date:   Tue Oct 14 09:26:24 2025 +0000
fix info leak

commit 8b7c651b37ce7a94633b7b7b7c980ded19a16e4f

Author: Morla Porla morla@overthewire.org
Date:   Tue Oct 14 09:26:24 2025 +0000
add missing data

commit 6d8e5e607602b597ade7504a550a29ba03f2cca0

Author: Ben Dover noone@overthewire.org
Date:   Tue Oct 14 09:26:24 2025 +0000
initial commit of README.md
```

```markdown
[liveuser@blackarch]-[~/repo]
>>> git checkout 8b7c651b37ce7a94633b7b7b7c980ded19a16e4f

# Bandit Notes
Some notes for level29 of bandit.

## credentials

-   username: bandit29

-   password:
```