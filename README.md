# Adhesions
Saisie d'adhésions sur une tablette. 
Un fichier contient toutes les inscriptions en format csv.
Il peut être visualisé par exemple avec ADB : adb shell cat /sdcard/Android/data/com.gosimpleapp.adhesions/adhesions.csv

## Contrôles effectués :

* Date < aujourd'hui
* Prénom et Nom : ^[A-Za-z\-éèàâêç ]{2,}$
* Adresse : ^[0-9A-Za-z,\-éèàâêç ]{5,}$
* CP      : <99000
* Ville : ^[A-Za-z\-éèàâêç ]{2,}$
* Tel : ^[0-9 \-]+$
* Montant : >1
* Clause : checkée

# Compilation 
C'est un projet Cordova qui utilse le plugin "File". Il suffit donc de placer le contenu de www, et de recompiler avec cordova.

# Crédits

* Lucas : idée 
* Antoine : facilitateur
* Guillaume : désign
* Stéphane : architecture, réalisation

