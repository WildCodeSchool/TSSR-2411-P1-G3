1. [Prérequis technique](#1-prérequis-technique)
2. [Installation de base des systèmes et de leur environnement](#2-installation-de-base-des-systèmes-et-de-leur-environnement)
   1. [Machine client sous Windows 10](#1-machine-client-sous-windows-10)
      1. [Configuration de la VM](#1-configuration-de-la-vm-windows-10)
      2. [Installation de Windows 10](#2-installation-de-windows-10)
      3. [Renommage du PC](#3-renommage-du-pc-windows-10)
      4. [Activation et configuration du bureau à distance](#4-activation-et-configuration-du-bureau-à-distance-windows-10)
      5. [Téléchargement et installation de TightVNC](#5-installation-de-tightvnc-windows-10)
      6. [Mises à jour Windows Update](#6-mises-à-jour-windows-update-windows-10)
      7. [Configuration d'une IP fixe](#7-configuration-dune-ip-fixe-windows-10)
   2. [Machine administrateur sous Windows Server 2022](#2-machine-administrateur-sous-windows-server-2022)
      1. [Configuration de la VM](#1-configuration-de-la-vm-windows-server-2022)
      2. [Installation de Windows Server 2022](#2-installation-de-windows-server-2022)
      3. [Renommage du PC](#3-renommage-du-pc-windows-server-2022)
      4. [Ajout du compte Administrator](#4-ajout-du-compte-administrator)
      5. [Activation et configuration du bureau à distance](#5-activation-et-configuration-du-bureau-à-distance-windows-server-2022)
      6. [Téléchargement et installation de TightVNC](#6-installation-de-tightvnc-windows-server-2022)
      7. [Mises à jour Windows Update](#7-mises-à-jour-windows-update-windows-server-2022)
      8. [Configuration d'une IP fixe](#8-configuration-dune-ip-fixe-windows-server-2022)
3. [Pour aller plus loin dans la configuration](#3-pour-aller-plus-loin-dans-la-configuration)
   1. [Sécuriser la connexion via le bureau à distance](#1-sécuriser-la-connexion-via-le-bureau-à-distance)
   2. [Sécuriser la connexion via TightVNC](#2-sécuriser-la-connexion-via-tightvnc)
   3. [Faciliter la connexion via un script PowerShell](#3-faciliter-la-connexion-via-un-script-powershell)
4. [FAQ](#4-FAQ)


# 1. Prérequis technique

## Côté client
- OS : Windows 10 Professionnel version 22h2
- Machine virtuelle utilisée : VMware Workstation
- Configuration VM :
   - Processeur : 4 coeurs
   - RAM : 4 Go
   - Disque : 60 Go


## Côté serveur
- OS : Windows Server 2022 Standard Evaluation 21h2
- Machine virtuelle utilisée : VMware Workstation
- Configuration VM :
   - Processeur : 4 coeurs
   - RAM : 4 Go
   - Disque : 60 Go


# 2. Installation de base des systèmes et de leur environnement


## 1. Machine client sous Windows 10

### 1. Configuration de la VM Windows 10


<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2001.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez la configuration "Typical" pour l'installation</p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2002.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez "Microsoft Windows" et "Windows 10 x64"</p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2003.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez le nom de votre machine virtuel</p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2004.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez la taille du disque</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2005.png" alt=""></p>
<p align="center">:arrow_forward: Télécharger l'iso de votre OS comme indiqué</p>

### 2. Installation de Windows 10


<br><p align="center"><img width="60%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2006.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez la langue</p>
<br><p align="center"><img width="60%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2007.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2008.png" alt=""></p>
<br><p align="center">:arrow_forward: Pour activé Windows sans clé de produit, choisissez " je n'ai pas de clé de produit (product key)"</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2009.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez " Windows 10 professionnel"</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2010.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez votre disque pour continuer l'installation</p>
<br><p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2011.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez Configuration pour une utilisation personnelle</p>
<br><p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2012.png" alt=""></p>
<p align="center">:arrow_forward: Si vous n'avez pas de compte, choisissez "compte Hors connexion"</p>
<br><p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2013.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez "Experience limité" puis, cliquez sur suivant</p>
<br><p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2014.png" alt=""></p>
<p align="center">:arrow_forward: Nommer votre Utilisateur</p>
<br><p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2015.png" alt=""></p>
<p align="center">:arrow_forward: Créer un mot de passe afin de sécuriser votre accès</p>
<br><p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2016.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez "Pas maintenant." puis, cliquez sur suivant</p>
<br><p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2017.png" alt=""></p>
<p align="center">:arrow_forward: Choissisez "non" puis, accepter.</p>
<br><p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2018.png" alt=""></p>
<p align="center">:arrow_forward: Encore une fois "non " puis accepter</p>
<br><p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2019.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez" Envoyer les données de diagnostic obligatoires" puis, accepter</p>
<br><p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2020.png" alt=""></p>
<p align="center">:arrow_forward: Choissisez "non" puis, accepter.</p>
<br><p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2021.png" alt=""></p>
<p align="center">:arrow_forward: Encore une fois "non " puis accepter</p>
<br><p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2022.png" alt=""></p>
<p align="center">:arrow_forward: Encore une fois "non " puis accepter</p>
<br><p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2023.png" alt=""></p>
<p align="center">:arrow_forward: Vous etes libres de personnaliser votre expérience, sinon ignorer cette étape</p>
<br><p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2024.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez "Pas maintenant"</p>

### 3. Renommage du PC Windows 10
Si vous avez besoin de renommer votre utilisateur pc , voici comment procéder :


<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2025.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez "Système"</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2026.png" alt=""></p>
<p align="center">:arrow_forward: Aller dans "A propos de"</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2027.png" alt=""></p>
<p align="center">:arrow_forward: Et la, choisissez "renommer ce pc"</p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2028.png" alt=""></p>
<p align="center">:arrow_forward: Donner lui le nom voulu</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2029.png" alt=""></p>
<p align="center">:arrow_forward: Vous verrez donc le nouveau nom choisi quand vous reviendrais dans " A propos de"</p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2030.png" alt=""></p>
<p align="center">:arrow_forward: L'ordinateur vous conseillera de redémarrer, accepter et attendez le redémarrage.</p>

### 4. Activation et configuration du bureau à distance Windows 10

Voici la marche à suivre pour configurer le bureau à distance sur Windows 10 ainsi qu'un raccourci cliquable que l'on va installer sur le bureau afin de faciliter la connexion :


<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2031.png" alt=""></p>
<p align="center">:arrow_forward: Retourner dans "Système" et choisissez "Bureau à distance" puis activer l'interrupteur</p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032.png" alt=""></p>
<p align="center">:arrow_forward: Confirmer l'activation</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032a.png" alt=""></p>
<p align="center">:arrow_forward: Vous voyez en revenant dans le bureau à distance que l'interrupteur est activé</p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2040.png" alt=""></p>
<p align="center">:arrow_forward: Ensuite, ouvrez le bureau à distance et rentrez le nom du serveur auquel vous voulez vous connecter et son nom d'utilisateur pour vous connecter à distance puis faites "connexion"</p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2052.png" alt=""></p>
<p align="center">:arrow_forward: Une fenêtre va s'ouvrir vous indiquant qu'il est impossible de s'autentifier en raison de problème liés au certificat de sécurité.Choisissez " afficher le certificat"</p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2053.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez "installer un certificat " et cliquez sur ok</p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2054.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez "ordinateur local" et suivant</p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2055.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez "oui"</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2056.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez " placer tout les certificats dans le magasin suivant et arcourez le magasin de certificats et choisissez " autorité de certification racines de confiance"
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2057.png" alt=""></p>
<p align="center">:arrow_forward: Une fois le bon certificat choisi, faite suivant,
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2058.png" alt=""></p>
<p align="center">:arrow_forward: Terminer les modification</p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2059.png" alt=""></p>
<p align="center">:arrow_forward: Un pop-up vous annonce que l'importation à réussi</p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2060.png" alt=""></p>
<p align="center">:arrow_forward: De retour dans le menu de connexion bureau à distance, Choisissez "enregistrer sous"</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2061.png" alt=""></p>
<p align="center">:arrow_forward: Créer un raccourci sur le bureau et enregistrer le</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2062.png" alt=""></p>
<p align="center">:arrow_forward: Voila, vous avez votre raccourci de connexion bureau à distance prêt à l'emploi !</p>


### 5. Installation de TightVNC Windows 10
Nous allons passer à l'installation de TightVNC, voila la procédure :


<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032b.png" alt=""></p>
<p align="center">:arrow_forward: Rendez-vous sur le site de TightVNC et choisissez la dernière version à jours correspondant à votre OS (dans notre cas, sa sera la version 2.8.85 pour Windows). Télécharger le.</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032c.png" alt=""></p>
<p align="center">:arrow_forward: Une fois installé, ouvrer le.</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032d.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez "next"</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032e.png" alt=""></p>
<p align="center">:arrow_forward: Pour l'installation, nous allons choisir l'installation "Custom" puis faites "next"</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032f.png" alt=""></p>
<p align="center">:arrow_forward: Dans le "Custom Setup" cliquer sur "TightVCN Server" et choisissez " Entire feature will be unavailable"</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032g.png" alt=""></p>
<p align="center">:arrow_forward: Puis faite "Next"</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032h.png" alt=""></p>
<p align="center">:arrow_forward: Si ce n'est pas le cas, cocher " Associate.vnc files with TightVNC Viewer" puis choisissez "Next"</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032i.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez "oui"</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032j.png" alt=""></p>
<p align="center">:arrow_forward: Puis terminer l'installation en cliquant sur "finish"</p>

### 6. Mises à jour Windows Update Windows 10
Mettez bien à jour votre OS Windows 10 comme cela :

<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032k.png" alt=""></p>
<p align="center">:arrow_forward: Dans votre barre de recherche, tapez "Rechercher des mises à jour" et accédez au panneau de mise à jour. choisissez "Recherches des mises à jour"</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032l.png" alt=""></p>
<p align="center">:arrow_forward: Si des mises à jour on été trouvées, téléchargé les et redémarrer votre ordinateur</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032m.png" alt=""></p>
<p align="center">:arrow_forward: Vous êtes maintenant à jour !</p>

### 7. Configuration d'une IP fixe Windows 10
Pour configurer une IP fixe sur Windows 10 voici la procédure :

<br><p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2033.png" alt=""></p>
<p align="center">:arrow_forward: Tapez "cmd" dans la barre Windows pour accéder aux invite de commandes</p>
<br><p align="center"><img width="90%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2034.png" alt=""></p>
<p align="center">:arrow_forward: Vous arrivez dans l'invite de commande. Tapez "ipconfig" et voyez ce que l'ordinateur vous affiche. récupérez "l'adresse IPv4"</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2035.png" alt=""></p>
<p align="center">:arrow_forward: Dans les paramètres, chercher la section "réseaux et Internet" et choisissez " Ethernet" Cliquez sur " Modifier les options d'adaptateur"</p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2036.png" alt=""></p>
<p align="center">:arrow_forward: Faites un clique droit sur Eternet0 et choisissez "propriétés"</p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2037.png" alt=""></p>
<p align="center">:arrow_forward: Aller dans "Gestion de réseau" et choisissez " protocole internet version 4( TCP/IPv4)" puis "Propriétés"</p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2038.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez "Utiliser l'adresse IP suivante" comme indiqué sur la capture d'écran puis cliquez sur "ok"</p>
<br><p align="center"><img width="90%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2039.png" alt=""></p>
<p align="center">:arrow_forward: Quand vous retournerez dans l'invite de commande et que vous taperez à nouveau la commande "ipconfig" vous vous apercevrez que l'adresse IPV4 aura changé. La configuration est terminée.</p>

## 2. Machine administrateur sous Windows Server 2022

### 1. Configuration de la VM Windows Server 2022


<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2001.png" alt=""></p>
<p align="center">:arrow_forward: Créer une nouvelle machine virtuelle, choisissez " Microsoft Windows" et la version "Windows server 2022" puis "next"</p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2002.png" alt=""></p>
<p align="center">:arrow_forward: Nommer votre machine virtuelle et placer la ou vous le souhaitez et cliquez sur "Next"</p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2003.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez de crée un disque virtuelle local comme indiqué et cliquez sur "Next"</p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2004.png" alt=""></p>
<p align="center">:arrow_forward: Choisissez "Customize Hardware"</p>
<br><p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2005.png" alt=""></p>
<p align="center">:arrow_forward: Télécharger l'ISO de votre choix (ici un ISO de Windows Server 2022) dans"NEW CD/DVD(SATA)" et fermez avec "close"</p>

### 2. Installation de Windows Server 2022

<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2006.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2007.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2008.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2009.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2010.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2011.png" alt=""></p>

### 3. Renommage du PC Windows Server 2022


<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2012.png" alt=""></p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2013.png" alt=""></p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2014.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2015.png" alt=""></p>

### 4. Ajout du compte Administrator


<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2016.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2017.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2018.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2019.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2020.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2021.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2022.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2023.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2024.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2025.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2026.png" alt=""></p>
<br><p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2027.png" alt=""></p>


### 5. Activation et configuration du bureau à distance Windows Server 2022

<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2031.png" alt=""></p>
<br><p align="center"><img width="50%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win10_complete/install%20windows%2010%20-%2032a.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2047.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2048.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2049.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2050.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2051.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2052.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2053.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2054.png" alt=""></p>


### 6. Installation de TightVNC Windows Server 2022

<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2027a.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2027b.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2027f.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2027g.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2027h.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2027i.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2027j.png" alt=""></p>
<br><p align="center"><img src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2027k.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2027l.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2028.png" alt=""></p>


### 7. Mises à jour Windows Update Windows Server 2022


<br><p align="center"><img width="70% src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2028a.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2028b.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2028c.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2028d.png" alt=""></p>


### 8. Configuration d'une IP fixe Windows Server 2022


<br><p align="center"><img width="90%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2029.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2030.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2031.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2032.png" alt=""></p>
<br><p align="center"><img width="70%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2033.png" alt=""></p>
<br><p align="center"><img width="90%" src="https://github.com/WildCodeSchool/TSSR-2411-P1-G3/blob/main/images/install_win_server_2022_complete/install%20windows%20server%202022%20-%2034.png" alt=""></p>


# 3. Pour aller plus loin dans la configuration

## 1. Sécuriser la connexion via le bureau à distance

## 2. Sécuriser la connexion via TightVNC

## 3. Faciliter la connexion via un script PowerShell


# 4. FAQ






























