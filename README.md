# Overthewire-[Bandit]
[OverTheWire](https://overthewire.org/wargames/bandit/) provides interactive wargames to learn and practice cybersecurity skills. Challenges like Bandit help users master Linux commands, networking, and more through hands-on problem-solving.


## LEVEL 0

Connect to overthewire's ssh server using there ssh information-
- Host: **bandit.labs.overthewire.org**
- Port: **2220**

## LEVEL 0 -> LEVEL 1

- Open the file called readme

```bash
  cat readme
```

## LEVEL 1 -> LEVEL 2

- Open a bash file

```bash
  cat ./-
```

## LEVEL 2 -> LEVEL 3

- Open a file with spaces using ""

```bash
  cat "spaces in this filename"
```

## LEVEL 3 -> LEVEL 4

- Change directory & use find command

```bash
  cd inhere && find | cat ./...Hiding-From-You
```

## LEVEL 4 -> LEVEL 5

- Scan all available files & check type for readable file
 
```bash
  for i in $(ls); do file ./$i; done | cat ./-file07
```

## LEVEL 5 -> LEVEL 6

- Change directory 
- Find readable file with size 1033byte & not executable 

```bash
  cd inhere | find . -readable -size 1033c ! -executable && cat ./inhere/maybehere07/.file2
```

## LEVEL 6 -> LEVEL 7

- Find file with owner bandit7 & group bandit6
- size 33byte

```bash
  find / -user bandit7 -group bandit6 -size 33c 2>/dev/null && cat var/lib/dpkg/info/bandit7.password
```

## LEVEL 7 -> LEVEL 8

- open data.txt & find word 'millionth'

```bash
  cat data.txt | grep "millionth"
````

## LEVEL 8 -> LEVEL 9

- sort data.txt & find unique line

```bash
  sort data.txt | uniq -u
```

## LEVEL 9 -> LEVEL 10

- sort readable data in data.txt and search for '='

```bash
  strings data.txt | grep "="
```

## LEVEL 10 -> LEVEL 11

- open file & decode base64

```bash
  cat data.txt | base64 -d
```

## LEVEL 11 -> LEVEL 12

- open file and rotate data by 13 using website **rot13.com**

```bash
  cat data.txt
```
```bash
  https://rot13.com/
```

## LEVEL 12 -> LEVEL 13

- change directory to /tmp
- make new directory
- check zip type and unzip till password found

```bash
  cat data.txt | cd tmp | mkdir <name> | cd | cp data.txt /tmp/<name> | cd /tmp/<name> | ls | cat data.txt | xxd -r > <name> | file <name> | mv <name> <name>.gz | gzip -d <name>.gz | mv <name> <name>.bz2 | bzip2 -d <name>.bz2 | mv <name> <name>.gz | gzip -d <name>.gz |  tar -xvf <name> | tar -xvf data5.bin | mv data6.bin data6.bin.bz2 | bzip2 -d data6.bin.bz2 | tar -xvf data6.bin | mv data8.bin data8.bin.gz | gzip -d data8.bin.gz | cat data8.bin
```

## LEVEL 13 -> LEVEL 14

- use ssh key to login with username **bandit14**

```bash
  ssh bandit14@localhost -p 2220 -i sshkey.private
```

## LEVEL 14 -> LEVEL 15

- open file **/etc/bandit_pass/bandit14**

```bash
  cd .. | cd .. | cat /etc/bandit_pass/bandit14
```
