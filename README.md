# Overthewire--Bandit
OverTheWire.org provides interactive wargames to learn and practice cybersecurity skills. Challenges like Bandit help users master Linux commands, networking, and more through hands-on problem-solving.


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

- sort readable data in data.txt and search for '=='

```bash
  strings data.txt | grep "="
```

