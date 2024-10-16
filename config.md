




# Guide d'installation et mise en place de la Téléassistance
## Sommaire
1. Pré-requis techniques
2. Configurations poste Serveur et poste Client
3. Configuration et test de connexion du Bureau d'accès à distance
4. Installation et configuration TightVNC poste Serveur et poste Client
5. Test connexion TightVNC
6. Configuration de l'accès sécurisé via TightVNC par filtrage d'adresse IP (depuis serveur)
7. Utilisation d'un script PowerShell pour faciliter la connexion au poste serveur
8. FAQ

### 1. Pré-requis techniques
- Poste Serveur : Windows serveur 2022, firewall désactivé, Remote management et Remote Desktop activés, firewall désactivé
- Poste Client : Windows 10 Pro, firewall désactivé

### 2. Configurations poste Serveur et poste Client
**Configuration Serveur windows**

**Server Manager**

• Dans **Server Manager**, se rendre dans **Local Server**
![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config_poste_cient_1.jpg) Vérifier les points suivants:

*   Remote management “**Enabled**” (Activer)
    
*   Remote desktop “**Enabled**” (Activer)
    
*   IE Enhanced Security Configuration “**Off**” 
    

**Adresse IP**

• Ouvrir le menu *Démarrer*, chercher le **Panel Control**. Ouvrir le **Panel Control**.
![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-2.png)

• Définir la préférence pour afficher les dossiers : "**large**" ou "**small**".
![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-3.png)


• Ouvrir “**Network and Sharing center**”.
![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-4.png)

• Aller dans la catégorie “**Change adapter settings”**.
![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-5.png)

• Sélectionner la carte **“Ethernet 2”**.
![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-6.png)

• Effectuer un clic droit puis sélectionner “**Properties**”. 
![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-7.png)
  
• Sélectionner “**Internet Protocol Version 4(TCP/IPV4)**” puis cliquer sur “**Properties**”.
![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-8.png)
  
• Dans "**IP address**", rentrer les valeurs suivantes: “**172.16.10.10**”, 
puis dans: “Subnet Mask(masque de sous réseaux)”:”**255.255.255.0”**.
![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-9.png)


**Firewall/Pare-feu**

• Ouvrir le menu *Démarrer*, chercher le **Panel Control**. Ouvrir le "**Panel Control**". 
![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config_poste_cient_1.jpg)
  
• Sélectionner “**Systems and Security**”.
![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-10.png)
  
• Ouvrir “**Windows Defender Firewall**”.
![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-11.png)
  
• Sélectionner “**Turn Windows Defender Firewall on or off**”.
![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-12.png)
  
• Désactiver les "*settings*" *privés* et *publics*.
![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-13.png)

### Configuration Poste Client

#### Configuration adresse IP

- Renseigner dans la barre de recherche en bas à gauche de votre écran : “**Panneau de configuration**”. Cliquer sur l’onglet “Panneau de configuration”.

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-2.png)


- Ensuite, aller dans l’onglet “**Réseau et Internet**”.

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-3.png)


- Puis l’onglet “**Centre Réseau et partage**”.

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-4.png)


- En suivant, sur la gauche de la fenêtre, cliquer sur l’onglet “**Modifier les paramètres de la carte**”.

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/config_poste_client_4.jpg)


- Sélectionner “**Ethernet 2***”.

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-5.png)


- Effectuer un clic droit > “**Propriétés**”. 

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-6.png)


- Sélectionner “**Protocole Internet version 4 (TCP/IPv4)**” puis cliquer sur “**Propriétés**”.

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-7.png)


- Décocher “Obtenir une adresse IP automatiquement” en cochant “Utiliser l’adresse IP suivante”
Inscrire comme adresse IP : “172.16.10.20”; et comme masque de sous-réseau : “255.255.255.0”.
Laisser le reste par défaut et valider en appuyant sur “OK”.

#### Désactivation des pare-feu

- Depuis le *Panneau de configuration*, aller dans “**Système et sécurité**” > “**Pare-Feu Windows Defender**”

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/config_poste_client_10.jpg)

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-11.png)

- Sur la gauche de la fenêtre, aller dans l’onglet “Activer ou désactiver le Pare-Feu Windows Defender”.

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-12.png)

- Décocher “Activer le Pare-Feu Windows Defender” en cochant “Désactiver le Pare-Feu Windows Defender” pour les paramètres des réseaux privés et publics.

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/Config%20ServeurWin-13.png)

- Valider l’opération en cliquant sur “OK”.


### 3. Configuration et test de connexion du Bureau d'accès à distance


### ***ACTIVER LE BUREAU A DISTANCE SUR LE POSTE SERVEUR***

#
- Aller dans le menu " **START** "

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/ACTIV%20SERV%20start.jpg)

#
- Aller dans " **SETTINGS** "

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/CONNEX%20%20barre%20co.jpg)

#
- Aller dans " **SYSTEM** " 

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/ACTIV%20SERV%20systeme.jpg)

#
- Aller dans " **REMOTE DESKTOP** "

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/ACTIV%20SERV%20remote%20desktop.jpg)

#
- Cocher l'onglet " **ENABLE REMOTE DESKTOP** "

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/ACTIV%20SERV%20enable.jpg)

#
- Puis " **CONFIRM** " pour valider l'activation

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/ACTIV%20SERV%20confim.jpg)


### Test connexion

#
- Sur le poste Client, se rendre dans "**BARRE DES TÂCHES**".

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/CONNEX%20bad.jpg)

#
- Taper "**CONNEXION BUREAU A DISTANCE**".

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/CONNEX%20connex%20bad.jpg)

#
- Cliquer sur l'application "**CONNEXION BUREAU A DISTANCE**".

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/CONNEX%20connex%20bad.jpg)

#
- Lors de la première connexion, dans le champs "**ORDINATEUR**" renseigner l'adresse IP ou le nom de l'ordinateur.
- Adresse IP : 172.16.10.10
- Nom de l'ordinateur : SRVWIN01
- Cliquer sur "**CONNEXION**".

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/CONNEX%20connexion.jpg)

#
- Renseigner les champs suivants avec le nom d'utilisateur et le mot de passe du poste Server.
- Nom d'utilisateur : Administrator
- Mot de passe : Azerty1*
- Valider par OK

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/ACTIV%201%20connexion.jpg)

#
- Cette page va s'afficher, vérifier que la navigation est fonctionnelle et que vous pouvez faire des actions sur le poste Serveur.

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/CONNEX%20connecte%C3%A9%20serv.jpg)

#
- Pour faciliter les prochaines connexions, nous allons créer un raccourci.
- Relancer le logiciel "**CONNEXION BUREAU A DISTANCE**" et cette fois appuyer sur sur la flèche allant vers le bas "**AFFICHER LES OPTIONS**"

![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/RDP_extend_full.png)

- Renseigner une nouvelle fois les champs "**ORDINATEUR**" et "**NOM D'UTILISATEUR**" avec les données précédentes.
- Cliquer sur "**ENREGISTRER SOUS**"
- Nommer le fichier RDP et le sauvegarder sur le Bureau.
 
![](https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/RDP_shortcut.png)

# 
- Tester la connexion via le raccourci et vérfier que tout fonctionne.
  
![]( https://github.com/WildCodeSchool/TSSR_PARIS_0924_P1_G3_TightVNC/blob/lassana_config/Images/RDP_shortcut.png)
