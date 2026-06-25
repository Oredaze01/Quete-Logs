# Quete-Logs


1. Installe un serveur web (Apache ou Nginx) sur une machine virtuelle Linux

Installation du serveur web apache2 réussie.

![[Capture d'écran 2026-06-25 141318.png]](Ressources/Capture d'écran 2026-06-25 141318.png)

![[Capture d'écran 2026-06-25 141720.png]](Ressources/Capture d'écran 2026-06-25 141720.png)

2. Configure le logging pour enregistrer les accès et les erreurs

Ici nous voyons bien que les logs sont enregistrés dans le dossier /var/log/apache2/ avec 3 fichier .log qui enregistré les informations.

![[Capture d'écran 2026-06-25 142204.png]](Ressources/Capture d'écran 2026-06-25 142204.png)


3. Génère du trafic sur le serveur web (utilise des outils comme curl ou un navigateur)


J'ai généré du trafic en me connectant via mon navigateur de ma machine hôte sur le serveur.

![[Capture d'écran 2026-06-25 141720.png]](Ressources/Capture d'écran 2026-06-25 141720.png)




4. Analyse les logs générés et identifie :
    - Les requêtes réussies (code 200)
    - Les erreurs 404 (page non trouvée)
    - Les adresses IP les plus fréquentes

J'ai ici filtré avec les 15 dernieres lignes pour afficher les logs sur le serveur apache2.
Nous voyons bien les codes 200 pour les requetes réussies.
Nous voyos le code 404 pour la page introuvable dans les logs.

![[Capture d'écran 2026-06-25 142204.png]](Ressources/Capture d'écran 2026-06-25 142204.png)

Ici nous voyons les adresses IP qui se sont connectées sur la page que j'ai trié avec la commande "sort" et "awk".

![[Capture d'écran 2026-06-25 143108.png]](Ressources/Capture d'écran 2026-06-25 143108.png)

