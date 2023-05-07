# OverTheWire
Une plateforme de jeu en ligne gratuite offrant des défis de sécurité informatique pour tous les niveaux de compétences. Les joueurs peuvent apprendre et améliorer leurs compétences en résolvant des niveaux progressivement plus difficiles.
#### Principes
- Connaissance des commandes Unix
- Familiarisation avec la ligne de commande
- Pensée critique
- Sécurité informatique

#### Sujet:
-->https://overthewire.org/wargames/bandit/bandit0.html
#### Ojectif:
Trouvez un mots de passe caché pour accéder au niveau suivant
d'où les commandes suivants sont à refaire durant chaque niveau:
```sh
ssh banditX@bandit.labs.overthewire.org -p 2220
password: Y
recherche_des_mots_de_passe
exit
```
>NB: dans le commande "ssh banditX@bandit.labs.overthewire.org -p 2220", X doit être remplacer par le numéro du niveau;et le Y dans "password: Y", par le mots de passe trouver dans le niveau précedent.


--> Les mots de passe séront de forme: NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL
## Les Solutions (bandit) de niveau 0 -- Niveau 34 (...)
------

### Niveau 0:
```sh
ssh bandit.labs.overthewire.org -p 2220 -l bandit0
password: bandit0
```

### Niveau 0 - 1:
```sh
ssh bandit0@bandit.labs.overthewire.org -p 2220
ls
cat readme
```
>NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL
### Niveau 1 - 2:
```sh
ssh bandit1@bandit.labs.overthewire.org -p 2220
ls
chat ./-
```
>rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi

### Niveau 2 - 3:
```sh
ssh bandit2@bandit.labs.overthewire.org -p 2220
ls
cat spaces\ in\ this\ filename
```
>aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG

### Niveau 3 - 4:
```sh
ssh bandit3@bandit.labs.overthewire.org -p 2220
ls
cd inhere/
ls
ls -1a
cat .hidden
```
>2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe

### Niveau 4 - 5:
```sh
ssh bandit4@bandit.labs.overthewire.org -p 2220
ls
ls -1a
cd inhere/
ls file ./*
cat ./-file07
```
>lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR

### Niveau 5 - 6:
```sh
ssh bandit5@bandit.labs.overthewire.org -p 2220
ls
cd inhere/
ls
find . -size 1033c
cat ./maybehere07/.file2
```
>P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU

### Niveau 6 - 7:
```sh
ssh bandit6@bandit.labs.overthewire.org -p 2220
find / -user bandit7 -group bandit6 -size 33c
cat /var/lib/dpkg/info/bandit7.password
```
>z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S

### Niveau 7 - 8:
```sh
ssh bandit7@bandit.labs.overthewire.org -p 2220
ls
cat data.txt | grep millionth
```
>TESKZC0XvTetK0S9xNwm25STk5iWrBvP

### Niveau 8 - 9:
```sh
ssh bandit8@bandit.labs.overthewire.org -p 2220
cat data.txt | sort | uniq -u
```
>EN632PlfYiZbn3PhVK3XOGSlNInNE00t

### Niveau 9 - 10
```sh
ssh bandit9@bandit.labs.overthewire.org -p 2220
ls
strings data.txt | grep =
```
>G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s

### Niveau 10 - 11:
```sh
ssh bandit10@bandit.labs.overthewire.org -p 2220
ls
cat data.txt | base64 --decode
```
>6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM

### Niveau 11 - 12:
```sh
ssh bandit11@bandit.labs.overthewire.org -p 2220
ls
cat data.txt | tr a-zA-Z n-za-mN-ZA-M
```
>JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv

### Niveau 12 - 13:
```sh
ssh bandit12@bandit.labs.overthewire.org -p 2220
ls
cat data.txt
mkdir /tmp/pavan
cp data.txt /tmp/pavan
cd /tmp/pavan
ls
file data.txt
xxd -r data.txt data1
file data1
mv data1 data2.gz
gzip -d data2.gz

file data2
mv data2 data3.bz2
bzip2 -d data3.bz2
file data3
mv data3 data4.gz
gzip -d data4.gz
file data4
tar -xvf data4

file data5.bin
tar -xvf data5.bin
file data6.bin
mv data6.bin data7.bz2
bzip2 -d data7.bz2
file data7
tar -xvf data7

file data8.bin
mv data8.bin data9.gz
gzip -d data9.gz
file data9
cat data9
```
>wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw

### Niveau 13 - 14:
```sh
ssh bandit13@bandit.labs.overthewire.org -p 2220
ls
ssh -i ./sshkey.private -p 2220 bandit14@localhost
```
>fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq

### Niveau 14- 15:
```sh
ssh bandit14@bandit.labs.overthewire.org -p 2220
echo "fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq" | nc localhost 30000
```
>Correct!
>jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt

### Niveau 15 - 16:

```sh
ssh bandit15@bandit.labs.overthewire.org -p 2220
openssl s_client -connect localhost:30001 -ign_eo
jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt
```
>Correct!
>JQttfApK4SeyHwDlI9SXGR50qclOAil1
>closed

### Niveau 16 - 17:
```sh
ssh bandit16@bandit.labs.overthewire.org -p 2220
nmap -A localhost -p 31000-32000
openssl s_client -connect localhost:31790
```
>Maintenant, entrez le mot de passe du niveau précédent
>Copiez la clé privée RSA
>MIIEogIBAAKCAQEAvmOkuifmMg6HL2YPIOjon6iWfbp7c3jx34>YkYWqUH57SUdyJ
>imZzeyGC0gtZPGujUSxiJSWI/oTqexh+cAMTSMlOJf7+BrJObA>rnxd9Y7YT2bRPQ
>Ja6Lzb558YW3FZl87ORiO+rW4LCDCNd2lUvLE/GL2GWyuKN0K5>iCd5TbtJzEkQTu
>DSt2mcNn4rhAL+JFr56o4T6z8WWAW18BR6yGrMq7Q/kALHYW3O>ekePQAzL0VUYbW
>JGTi65CxbCnzc/w4+mqQyvmzpWtMAzJTzAzQxNbkR2MBGySxDL>rjg0LWN6sK7wNX
>x0YVztz/zbIkPjfkU1jHS+9EbVNj+D1XFOJuaQIDAQABAoIBAB>agpxpM1aoLWfvD
>KHcj10nqcoBc4oE11aFYQwik7xfW+24pRNuDE6SFthOar69jp5>RlLwD1NhPx3iBl
>J9nOM8OJ0VToum43UOS8YxF8WwhXriYGnc1sskbwpXOUDc9uX4>+UESzH22P29ovd
>d8WErY0gPxun8pbJLmxkAtWNhpMvfe0050vk9TL5wqbu9Albss>gTcCXkMQnPw9nC
>YNN6DDP2lbcBrvgT9YCNL6C+ZKufD52yOQ9qOkwFTEQpjtF4uN>tJom+asvlpmS8A
>vLY9r60wYSvmZhNqBUrj7lyCtXMIu1kkd4w7F77k+DjHoAXyxc>Up1DGL51sOmama
>+TOWWgECgYEA8JtPxP0GRJ+IQkX262jM3dEIkza8ky5moIwUqY>dsx0NxHgRRhORT
>8c8hAuRBb2G82so8vUHk/fur85OEfc9TncnCY2crpoqsghifKL>xrLgtT+qDpfZnx
>SatLdt8GfQ85yA7hnWWJ2MxF3NaeSDm75Lsm+tBbAiyc9P2jGR>NtMSkCgYEAypHd
>HCctNi/FwjulhttFx/rHYKhLidZDFYeiE/v45bN4yFm8x7R/b0>iE7KaszX+Exdvt
>SghaTdcG0Knyw1bpJVyusavPzpaJMjdJ6tcFhVAbAjm7enCIvG>CSx+X3l5SiWg0A
>R57hJglezIiVjv3aGwHwvlZvtszK6zV6oXFAu0ECgYAbjo46T4h>yP5tJi93V5HDi
>Ttiek7xRVxUl+iU7rWkGAXFpMLFteQEsRr7PJ/lemmEY5eTDAFM>Ly9FL2m9oQWCg
>R8VdwSk8r9FGLS+9aKcV5PI/WEKlwgXinB3OhYimtiG2Cg5JCqI>ZFHxD6MjEGOiu
>L8ktHMPvodBwNsSBULpG0QKBgBAplTfC1HOnWiMGOU3KPwYWt0O>6CdTkmJOmL8Ni
>blh9elyZ9FsGxsgtRBXRsqXuz7wtsQAgLHxbdLq/ZJQ7YfzOKU4>ZxEnabvXnvWkU
>YOdjHdSOoKvDQNWu6ucyLRAWFuISeXw9a/9p7ftpxm0TSgyvmfL>F2MIAEwyzRqaM
>77pBAoGAMmjmIJdjp+Ez8duyn3ieo36yrttF5NSsJLAbxFpdlc1>gvtGCWW+9Cq0b
>dxviW8+TFVEBl1O4f7HVm6EpTscdDxU+bCXWkfjuRb7Dy9GOtt9>JPsX8MBTakzh3
>vBgsyi/sN3RqRBcGU40fOoZyfAMT8s1m/uYv52O6IgeuZ/ujbjY>=

### Niveau 17 - 18:

>Once paste ctrl +x and y

```sh

mkdir /tmp/techyrick_ssh
cd /tmp/techyrick_ssh
nano techyrick.private
```
>Collez la clé privée RSA dans nano techyrick.private, il vous demandera d'appuyer sur Entrée >une fois que vous aurez entré, vous devrez coller la clé
>Une fois coller ctrl + x et y
```sh
chmod 600 pavan.private
ssh -i sshkey17.private bandit17@bandit.labs.overthewire.org -p 2220
 sort passwords.old passwords.new | uniq -u
```
>glZreTEH1V3cGKL6g4conYqZqaEj0mte
>hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg

```sh
cat passwords.new | grep glZreTEH1V3cGKL6g4conYqZqaEj0mte && cat passwords.new | grep hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg
```
>hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg

----------------------
> ------------------------------------- en cours---------------------------------------------

### Niveau 18 - 19:
```sh

```
>
### Niveau 19 - 20:
```sh

```

>

### Niveau 20 - 21:
```sh

```

### Niveau 21 - 22:
```sh

```

### Niveau 22 - 23:
```sh

```

### Niveau 23 - 24:
```sh

```

### Niveau 24 - 25:
```sh

```
### Niveau 25 - 26:
```sh

```

### Niveau 26 - 27:
```sh

```

### Niveau 27 - 28:
```sh

```

### Niveau 28 - 29:
```sh

```

### Niveau 29 - 30:
```sh

```

### Niveau 30 - 31:
```sh

```

### Niveau 31 - 32:
```sh

```

### Niveau 32 - 33:
```sh

```

### Niveau 33 - :
```sh

```
