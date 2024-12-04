# TSSR-2411-P1-G3
# Groupe 2 : Téléassistance  


<img src="https://5.imimg.com/data5/SELLER/Default/2023/10/356050645/JO/YL/IH/185666206/windows-server-2022-standard-500x500.jpg" alt="logo windows" width="200"> <img src="https://a-us.storyblok.com/f/1014140/360x249/5e945b138d/tightvnc.png" alt="logo tightvnc" width="200">




<br>

**Membres du groupes** 
|Membres   | Philippe       | Camille | Angel | Sebastien |
| :--------------- |:---------------:|:---------------:|:---------------:|:---------------:|
|          | Scrum Master | Product Owner | Developer| Developer|
<br>
<br>

## Présentation du projet

A la demande du client, notre groupe à eu pour objectif de configurer un accès sécurisé afin de faire de la téléassistance sur un serveur *Windows 2022* en utilisant le logiciel *TightVNC* ainsi que la connexion bureau à distance.
Le client nous à également demander de créer un script powershell pour faciliter cette connexion.
<br>
## Introduction et mise en contexte

> Contrôler un ordinateur à distance ressemble au pitch d’un épisode de *Black Mirror*, pourtant cette technologie est déjà bien ancrée dans nos habitudes.

La prise en main à distance nous permet de contrôler un ordinateur, un appareil ou un réseau sans avoir à être physiquement sur place. Concrètement, c’est l’assistance technique qui vous aide pour vos problèmes concernant votre ordinateur ou votre réseau.
Cette technologie est d’autant plus pertinente avec la généralisation du télétravail. Grâce à la prise en main à distance, les employés peuvent continuer à accéder à leur ordinateur au bureau et le contrôler comme s'ils étaient au bureau.

TightVNC permet de prendre le contrôle à distance (ou prise de main) d'un autre ordinateur en utilisant un réseau, par exemple Internet. Le poste distant est présenté dans une fenêtre sur le poste client, c'est une présentation dite graphique par opposition aux outils de prise de main à distance en mode texte. Plusieurs personnes, via le logiciel client appelé Visionneuse TightVNC, peuvent voir ce qui se passe sur un autre ordinateur sur lequel s'exécute le logiciel serveur.
<br>
## Choix technique
<br>

|   Choix de l'OS  |  Tight VCN | Windows serveur 2022 |
| :--------------- |:---------------:| :---------------:|
|  choix de la version | version 2.8.85  | Standard evaluation version 21H2 |
<br>

## Difficultées rencontrées
- Difficulté à se connecter sur deux réseaux différents (avec deux adresses IP différentes)
- Difficulté à renforcer la sécurité des connexions avec Tight VNC et bureau à distance

  <br>

## Solutions trouvées
 - Connexion sur le même réseaux avec une même adresse IP

  <br>

## Suggestions d'améliorations possibles :
- Une interfase graphique moins archaïque et plus développé
- Choix d'un mot de passe de session beaucoup plus complexe pour sécurisé l'accès
- Utiliser un tunnel SSH pour renforcer la sécurité de connexion avec TightVNC
