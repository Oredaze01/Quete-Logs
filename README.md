# Quete-Logs



1. Installe un serveur web (Apache ou Nginx) sur une machine virtuelle Linux

Installation du serveur web apache2 réussie.

![[quete-logs-3.png]](Ressources/quete-logs-3.png)

![[quete-logs-4.png]](Ressources/quete-logs-4.png)

2. Configure le logging pour enregistrer les accès et les erreurs

Ici nous voyons bien que les logs sont enregistrés dans le dossier /var/log/apache2/ avec 3 fichier .log qui enregistré les informations.

![[quete-logs-6.png]](Ressources/quete-logs-6.png)


3. Génère du trafic sur le serveur web (utilise des outils comme curl ou un navigateur)


J'ai généré du trafic en me connectant via mon navigateur de ma machine hôte sur le serveur.

![[quete-logs-4 1.png]](Ressources/quete-logs-4.png)



4. Analyse les logs générés et identifie :
    - Les requêtes réussies (code 200)
    - Les erreurs 404 (page non trouvée)
    - Les adresses IP les plus fréquentes

J'ai ici filtré avec les 15 dernières lignes pour afficher les logs sur le serveur apache2.
Nous voyons bien les codes 200 pour les requêtes réussies.
Nous voyons le code 404 pour la page introuvable dans les logs.

![[quete-logs-6 1.png]](Ressources/quete-logs-6.png)

Ici nous voyons les adresses IP qui se sont connectées sur la page que j'ai trié avec la commande "sort" et "awk".


![[quete-logs-8.png]](Ressources/quete-logs-8.png)


