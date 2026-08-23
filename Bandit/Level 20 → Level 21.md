# Level 20 → Level 21

> Need to provide a **server** (using **`nc`**) that listens on that port.
> 

> **`./suconnect`** program listens to the port you specified as a command line argument
> 
> 
> after both terminals are active and listening to each other, paste bandit20’s password at **`nc`** terminal and **`./suconnect`** will return Bandit21’s Password ****
> 

---

```bash
bandit20@bandit:~$ ./suconnect <port> &

bandit20@bandit:~$ nc -l -p <port>

Input: Bandit20's Password
Output: Bandit21's Password

```
---

**`&`** — **Background Execution**