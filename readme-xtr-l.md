# xtrloker

xtrloker est un outil de sécurité en Python conçu pour protéger vos fichiers et dossiers sensibles.  
Il permet de les verrouiller à l’aide d’un mot de passe robuste et de les déverrouiller uniquement avec la clé correcte.  

Lorsqu’un fichier ou dossier est verrouillé, il est entièrement chiffré et remplacé par un fichier ayant l’extension `.xtrlocked`.  
Les fichiers originaux ne restent pas accessibles : seule la version chiffrée existe, ce qui garantit la confidentialité des données.  

Pour le déverrouillage, l’utilisateur doit entrer le mot de passe défini lors du verrouillage.  
Un système de sécurité intégré limite les tentatives à 5 essais.  
Si le mot de passe est incorrect 5 fois de suite, le fichier ou dossier est automatiquement bloqué pendant 1 heure avant de pouvoir réessayer.  

Cette approche protège vos données contre les accès non autorisés et les attaques par force brute.  
Le code est conçu pour fonctionner tel quel et ne doit pas être modifié.  

## Installation et lancement

1. Rendre le script exécutable (Linux) :  
      bash
   chmod +x xtrloker.py
   

2. Lancer le programme :  
      bash
   ./xtrloker.py
    
   ou  
      bash
   python3 xtrloker.py
   

## Fonctionnement

- Les fichiers et dossiers verrouillés obtiennent l’extension `.xtrlocked`  
- Les données originales sont supprimées après chiffrement  
- Seul le mot de passe choisi permet de récupérer le contenu  
- Après 5 échecs de mot de passe, le fichier reste bloqué pendant 1 heure  

## Licence

Projet créé par xtr – destiné à un usage personnel et éducatif.

