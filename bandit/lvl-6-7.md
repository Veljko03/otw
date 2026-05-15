The password for the next level is stored somewhere on the server and has all of the following properties:

owned by user bandit7
owned by group bandit6
33 bytes in size

bandit6@bandit:~$ pwd
/home/bandit6

1:changed to root dir to check whole system - cd /

2:tryed to use 
find . -user bandit6 -group bandit7 -size 33c
but got too many files with permision deied

3: 2>/dev/null -added in the end

command : 
bandit6@bandit:/$ find . -user bandit7 -group bandit6 -size 33c 2>/dev/null
./var/lib/dpkg/info/bandit7.password

password: morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj