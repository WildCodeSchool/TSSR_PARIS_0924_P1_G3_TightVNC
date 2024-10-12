
### 2. Configurations poste Serveur et poste Client
**Configuration Serveur windows**

**Server Manager**

• Dans **Server Manager**, se rendre dans **Local Server**
![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/Config%20ServeurWin-1.png)
Vérifier les points suivants:

*   Remote management “**Enabled**” (Activer)
    
*   Remote desktop “**Enabled**” (Activer)
    
*   IE Enhanced Security Configuration “**Off**” 
    

**Adresse IP**

• Ouvrir le menu *Démarrer*, chercher le **Panel Control**. Ouvrir le **Panel Control**.
![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/Config%20ServeurWin-2.png)

• Définir la préférence pour afficher les dossiers : "**large**" ou "**small**".
![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/Config%20ServeurWin-3.png)


• Ouvrir “**Network and Sharing center**”.
![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/Config%20ServeurWin-4.png)

• Aller dans la catégorie “**Change adapter settings”**.
![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/Config%20ServeurWin-5.png)

• Sélectionner la carte **“Ethernet 2”**.
![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/Config%20ServeurWin-6.png)

• Effectuer un clic droit puis sélectionner “**Properties**”. 
![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/Config%20ServeurWin-7.png)
  
• Sélectionner “**Internet Protocol Version 4(TCP/IPV4)**” puis cliquer sur “**Properties**”.
![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/Config%20ServeurWin-8.png)
  
• Dans "**IP address**", rentrer les valeurs suivantes: “**172.16.10.10**”, 
puis dans: “Subnet Mask(masque de sous réseaux)”:”**255.255.255.0”**.
![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/Config%20ServeurWin-9.png)


**Firewall/Pare-feu**

• Ouvrir le menu *Démarrer*, chercher le **Panel Control**. Ouvrir le "**Panel Control**". 
![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/Config%20ServeurWin-2.png)
  
• Sélectionner “**Systems and Security**”.
![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/Config%20ServeurWin-10.png)
  
• Ouvrir “**Windows Defender Firewall**”.
![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/Config%20ServeurWin-11.png)
  
• Sélectionner “**Turn Windows Defender Firewall on or off**”.
![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/Config%20ServeurWin-12.png)
  
• Désactiver les "*settings*" *privés* et *publics*.
![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/Config%20ServeurWin-13.png)

### Configuration Poste Client

#### Configuration adresse IP

- Renseigner dans la barre de recherche en bas à gauche de votre écran : “**Panneau de configuration**”. Cliquer sur l’onglet “Panneau de configuration”.

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/Config_poste_cient_1.jpg)


- Ensuite, aller dans l’onglet “**Réseau et Internet**”.

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/config_poste_client_2.jpg)


- Puis l’onglet “**Centre Réseau et partage**”.

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/config_poste_client_3.jpg)


- En suivant, sur la gauche de la fenêtre, cliquer sur l’onglet “**Modifier les paramètres de la carte**”.

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/config_poste_client_4.jpg)


- Sélectionner “**Ethernet 2***”.

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/config_poste_client_5.jpg)


- Effectuer un clic droit > “**Propriétés**”. 

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/config_poste_client_6.jpg)


- Sélectionner “**Protocole Internet version 4 (TCP/IPv4)**” puis cliquer sur “**Propriétés**”.

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/config_poste_client_7.jpg)


- Décocher “Obtenir une adresse IP automatiquement” en cochant “Utiliser l’adresse IP suivante”
Inscrire comme adresse IP : “172.16.10.20”; et comme masque de sous-réseau : “255.255.255.0”.
Laisser le reste par défaut et valider en appuyant sur “OK”.

#### Désactivation des pare-feu

- Depuis le *Panneau de configuration*, aller dans “**Système et sécurité**” > “**Pare-Feu Windows Defender**”

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/config_poste_client_11.jpg)

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/config_poste_client_8.jpg)

- Sur la gauche de la fenêtre, aller dans l’onglet “Activer ou désactiver le Pare-Feu Windows Defender”.

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/config_poste_client_9.jpg)

- Décocher “Activer le Pare-Feu Windows Defender” en cochant “Désactiver le Pare-Feu Windows Defender” pour les paramètres des réseaux privés et publics.

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/config_poste_client_10.jpg)

- Valider l’opération en cliquant sur “OK”.


### 3. Configuration et test de connexion du Bureau d'accès à distance


### ***ACTIVER LE BUREAU A DISTANCE SUR LE POSTE SERVEUR***

#
- Aller dans le menu " **START** "

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/ACTIV%20SERV%20start.jpg)

#
- Aller dans " **SETTINGS** "

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/ACTIV%20SERV%20settings.jpg)

#
- Aller dans " **SYSTEM** " 

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/ACTIV%20SERV%20systeme.jpg)

#
- Aller dans " **REMOTE DESKTOP** "

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/ACTIV%20SERV%20remote%20desktop.jpg)

#
- Cocher l'onglet " **ENABLE REMOTE DESKTOP** "

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/ACTIV%20SERV%20enable.jpg)

#
- Puis " **CONFIRM** " pour valider l'activation

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/ACTIV%20SERV%20confim.jpg?raw=true)


### Test connexion

#
- Sur le poste Client, se rendre dans "**BARRE DES T CHES**".

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/CONNEX%20bad.jpg)

#
- Taper "**CONNEXION BUREAU A DISTANCE**".

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/CONNEX%20%20barre%20co.jpg)

#
- Cliquer sur l'application "**CONNEXION BUREAU A DISTANCE**".

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/CONNEX%20connex%20bad.jpg)

#
- Lors de la première connexion, dans le champs "**ORDINATEUR**" renseigner l'adresse IP ou le nom de l'ordinateur.
- Adresse IP : 172.16.10.10
- Nom de l'ordinateur : SRVWIN01
- Cliquer sur "**CONNEXION**".

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/CONNEX%20connexion.jpg)

#
- Renseigner les champs suivants avec le nom d'utilisateur et le mot de passe du poste Server.
- Nom d'utilisateur : Administrator
- Mot de passe : Azerty1*
- Valider par OK

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/ACTIV%201%20connexion.jpg)

#
- Cette page va s'afficher, vérifier que la navigation est fonctionnelle et que vous pouvez faire des actions sur le poste Serveur.

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/CONNEX%20connecte%C3%A9%20serv.jpg)

#
- Pour faciliter les prochaines connexions, nous allons créer un raccourci.
- Relancer le logiciel "**CONNEXION BUREAU A DISTANCE**" et cette fois appuyer sur sur la flèche allant vers le bas "**AFFICHER LES OPTIONS**"

![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/Option_RDP.jpg)

- Renseigner une nouvelle fois les champs "**ORDINATEUR**" et "**NOM D'UTILISATEUR**" avec les données précédentes.
- Cliquer sur "**ENREGISTRER SOUS**"
- Nommer le fichier RDP et le sauvegarder sur le Bureau.
 
![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/RDP_extend_full.png)

# 
- Tester la connexion via le raccourci et vérfier que tout fonctionne.
  
![](https://raw.githubusercontent.com/WildCodeSchool/TSSR-2402-P1-G2-Teleassistance/main/Images/RDP_shortcut.png)

