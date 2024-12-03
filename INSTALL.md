1. [Prérequis technique](#1-prérequis-technique)
2. Installation de base des systèmes et de leur environnement
   1. [Machine client sous Windows 10](#machine-client-sous-windows-10)
      1. [Configuration de la VM](#configuration-de-la-vm-windows-10)
      2. [Installation de Windows 10](#installation-de-windows-10)
      3. [Renommage du PC](#renommage-du-pc-windows-10)
      4. [Activation et configuration du bureau à distance](#activation-et-configuration-du-bureau-a-distance-windows-10)
      5. [Téléchargement et installation de TightVNC](#installation-de-tightvnc-windows-10)
      6. [Mises à jour Windows Update](#mises-a-jour-windows-update-windows-10)
      7. [Configuration d'une IP fixe](#configuration-ip-fixe-windows-10)
   2. [Machine administrateur sous Windows Server 2022](#machine-administrateur-sous-windows-server-2022)
      1. [Configuration de la VM](#configuration-de-la-vm-windows-server-2022)
      2. [Installation de Windows Server 2022](#installation-de-windows-server-2022)
      3. [Renommage du PC](#renommage-du-pc-windows-server-2022)
      4. [Ajout du compte "Administrator"](#ajout-du-compte-administrator)
      5. [Activation et configuration du bureau à distance](#activation-et-configuration-du-bureau-a-distance-windows-server-2022)
      6. [Téléchargement et installation de TightVNC](#installation-de-tightvnc-windows-server-2022)
      7. [Mises à jour Windows Update](#mises-a-jour-windows-update-windows-server-2022)
      8. [Configuration d'une IP fixe](#configuration-ip-fixe-windows-server-2022)
3. [Pour aller plus loin dans la configuration](#pour-aller-plus-loin-dans-la-configuration)
   1. [Sécuriser la connexion via le bureau à distance](#securiser-connexion-bureau-a-distance)
   2. [Sécuriser la connexion via Tight VNC](#securiser-connexion-tight-vnc)
   3. [Faciliter la connexion via un script PowerShell](#faciliter-connexion-powershell)



# FAQ



## Côté serveur :
OS : Windows Server 2022 version
Machine virtuelle utilisée : VMware Workstation
Configuration VM :
Processeur : 4 coeurs
RAM : 4 Go
Disque : 60 Go


# Etapes d'installation et de configuration

# Installation TightVNC

L'installation diffère selon que l'on est côté serveur ou côté client.

## Installation TightVNC côté serveur

Téléchargement
Rendez-vous sur le site officiel pour télécharger l'application. Nous avons choisi la version de TightVNC la plus récente (v2.8.85) en cliquant sur "Installer for Windows (64-bit). (ph100)

Une fois l'excutable téléchargé, on lance l'installation (ph101).

On a choisi l'installation "Typical" pour pouvoir se concentrer sur la partie serveur. (ph102)

Et justement, sur l'affichage suivant on a désactivé la partie "Viewer", qui correspond à la partie utilisée par le client. (ph103)

# 1. Prérequis Technique


<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2001.png" alt=""></p>
<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2002.png" alt=""></p>
<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2003.png" alt=""></p>
<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2004.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2005.png" alt=""></p>
<p align="center"><img width="60%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2006.png" alt=""></p>
- choisissez la langue.
<p align="center"><img width="60%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2007.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2008.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2009.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2010.png" alt=""></p>
<p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2011.png" alt=""></p>
<p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2012.png" alt=""></p>
<p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2013.png" alt=""></p>
<p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2014.png" alt=""></p>
<p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2015.png" alt=""></p>
<p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2016.png" alt=""></p>
<p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2017.png" alt=""></p>
<p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2018.png" alt=""></p>
<p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2019.png" alt=""></p>
<p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2020.png" alt=""></p>
<p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2021.png" alt=""></p>
<p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2022.png" alt=""></p>
<p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2023.png" alt=""></p>
<p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2024.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2025.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2026.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2027.png" alt=""></p>
<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2028.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2029.png" alt=""></p>
<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2030.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2031.png" alt=""></p>
<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032a.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032b.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032c.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032d.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032e.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032f.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032g.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032h.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032i.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032j.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032k.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032l.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032m.png" alt=""></p>
<p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2033.png" alt=""></p>
<p align="center"><img width="90%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2034.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2035.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2036.png" alt=""></p>
<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2037.png" alt=""></p>
<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2038.png" alt=""></p>
<p align="center"><img width="90%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2039.png" alt=""></p>
<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2040.png" alt=""></p>
<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2052.png" alt=""></p>
<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2053.png" alt=""></p>
<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2054.png" alt=""></p>
<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2055.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2056.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2057.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2058.png" alt=""></p>
<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2059.png" alt=""></p>
<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2060.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2061.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2062.png" alt=""></p>

# 1. Prérequis techniques


<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2001.png" alt=""></p>
<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2002.png" alt=""></p>
<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2003.png" alt=""></p>
<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2004.png" alt=""></p>
<p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2005.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2006.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2007.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2008.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2009.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2010.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2011.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2012.png" alt=""></p>
<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2013.png" alt=""></p>
<p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2014.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2015.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2016.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2017.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2018.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2019.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2020.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2021.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2022.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2023.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2024.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2025.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2026.png" alt=""></p>
<p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2027.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2027a.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2027b.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2027f.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2027g.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2027h.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2027i.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2027j.png" alt=""></p>
<p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2027k.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2027l.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2028.png" alt=""></p>
<p align="center"><img width="70% src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2028a.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2028b.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2028c.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2028d.png" alt=""></p>
<p align="center"><img width="90%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2029.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2030.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2031.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2032.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2033.png" alt=""></p>
<p align="center"><img width="90%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2034.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2047.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2048.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2049.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2050.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2051.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2052.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2053.png" alt=""></p>
<p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2054.png" alt=""></p>
![image](https://github.com/user-attachments/assets/5fafcac2-9285-41d5-b429-d961e50a6d59)

# 1. Prérequis technique

# 2. Installation de base des systèmes et de leur environnement

## Machine client sous Windows 10

### Configuration de la VM Windows 10

### Installation de Windows 10

### Renommage du PC Windows 10

### Activation et configuration du bureau à distance Windows 10

### Installation de TightVNC Windows 10

### Mises à jour Windows Update Windows 10

### Configuration d'une IP fixe Windows 10

## Machine administrateur sous Windows Server 2022

### Configuration de la VM Windows Server 2022

### Installation de Windows Server 2022

### Renommage du PC Windows Server 2022

### Ajout du compte "Administrator"

### Activation et configuration du bureau à distance Windows Server 2022

### Installation de TightVNC Windows Server 2022

### Mises à jour Windows Update Windows Server 2022

### Configuration d'une IP fixe Windows Server 2022

# 3. Pour aller plus loin dans la configuration

## Sécuriser la connexion via le bureau à distance

## Sécuriser la connexion via Tight VNC

## Faciliter la connexion via un script PowerShell







