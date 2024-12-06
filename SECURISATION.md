# Sommaire
1. [Installation Open SSH](#1-installation-open-ssh)
   1. [Windows 10](#1-windows-10)
   2. [Windows Server 2022](#2-Windows-Server-2022)
2. [Sécuriser la connexion Bureau à distance](#2-sécuriser-la-connexion-bureau-à-distance)
   1. [Changement du port utilisé par le bureau à distance](#1-Changement-du-port-utilisé-par-le-bureau-à-distance)
   2. [Echec de la connexion depuis le PC client](#2-Echec-de-la-connexion-depuis-le-PC-client)
   3. [Recherche de solutions](#3-Recherche-de-solutions)
3. [Paramétrage en réseau privé](#3-Paramétrage-en-réseau-privé)
   1. [Windows 10](#1-windows-10)
   2. [Windows Server 2022](#2-Windows-Server-2022)
4. [Installation de MobaXterm sur Windows 10](#4-Installation-de-MobaXterm-sur-Windows-10)
5. [Sécurisation de TightVNC](#5-Sécurisation-de-TightVNC)
6. [Modification du port SSH](#6-Modification-du-port-SSH)
7. [Utilisation de Putty pour se connecter en SSH via un tunnel](#7-Utilisation-de-Putty-pour-se-connecter-en-SSH-via-un-tunnel)


# 1. Installation Open SSH
## 1. Windows 10
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20100.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20101.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20102.png" alt=""></p>
## 2. Windows Server 2022
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20100.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20101.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20102.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20103.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20104.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20105.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20106.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20107.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20108.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20117.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20118.png" alt=""></p>
# 2. Sécuriser la connexion Bureau à distance
## 1. Changement du port utilisé par le bureau à distance
Par défaut 3389, basculé sur 49151.
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20127.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20128.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20129.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20129png.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20130.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20131.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20132.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20133.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20134.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20135.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20136.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20137.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20138.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20139.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20140.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20141.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20142.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20117.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20126.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20127.png" alt=""></p>
## 2. Echec de la connexion depuis le PC client
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20130.png" alt=""></p>
## 3. Recherche de solutions
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20143.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20144.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20145.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20131.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20146.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20147.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20132.png" alt=""></p>
# 3. Paramétrage en réseau privé
## 1. Windows 10
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20153.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20154.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20155.png" alt=""></p>
## 2. Windows Server 2022
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20151.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20152.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20153.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20154.png" alt=""></p>
# 4. Installation de MobaXterm sur Windows 10
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20109.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20110.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20111.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20112.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20113.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20114.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20115.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20133.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20134.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20135.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20136.png" alt=""></p>
# 5. Sécurisation de TightVNC
Port par défaut 5900. Idée : modifier le port pour sécuriser la connexion en passant par le port 25600.
## 1. Windows Server 2022
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%20server%202022%20-%20163.png" alt=""></p>
## 2. Windows 10
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20156.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20157.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20158.png" alt=""></p>
# 6. Modification du port SSH
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20149.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20150.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20164.png" alt=""></p>
<br><p align="center"><img width="70%"  src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20165.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20166.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20167.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20168.png" alt=""></p>
<br><p align="center"><img width="70%"  src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20169.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20170.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20171.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20172.png" alt=""></p>
# 7. Utilisation de Putty pour se connecter en SSH via un tunnel
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20113.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20114.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20115.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20116.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20140.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20141.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20142.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20143.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/securistation/install%20windows%2010%20-%20144.png" alt=""></p>
![image](https://github.com/user-attachments/assets/b6c378a5-ffd6-4e0e-8a87-19e9258a981d)

