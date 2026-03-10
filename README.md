Tu es un développeur senior spécialisé en JavaScript, Progressive Web Apps (PWA) et synchronisation de données.

Je vais te fournir le fichier complet de mon application de budget (HTML + JavaScript).

Objectif : transformer cette application en Progressive Web App robuste et installable, tout en améliorant la fiabilité de la sauvegarde et de la synchronisation.

Tâches à réaliser :

1. Analyse le code existant avant toute modification.

2. Ne réécris pas toute l'application.
   Conserve la structure existante et modifie uniquement les parties nécessaires.

3. Transformer l’application en Progressive Web App (PWA) :

* créer un fichier manifest.json
* créer un service worker
* permettre l'installation de l'application sur mobile et desktop
* permettre l'utilisation hors ligne

4. Le service worker doit :

* mettre en cache les fichiers principaux
* permettre l'utilisation offline
* mettre à jour le cache proprement quand une nouvelle version est disponible

5. Améliorer le système de sauvegarde et synchronisation :

• sauvegarde locale prioritaire (localStorage)

• synchronisation différée (debounce 8 secondes)

• file d’attente de synchronisation

• retry automatique en cas d’échec

• détection offline avec navigator.onLine

• reprise automatique de la synchronisation quand la connexion revient

• ajout d'un timestamp dans les données :
updated: Date.now()

• éviter les synchronisations inutiles en comparant les données

• protéger toutes les opérations JSON.parse avec try/catch

• vérifier les données après synchronisation GitHub

6. Ajouter une fonction de synchronisation multi-appareils :

L'application doit vérifier périodiquement (ex: toutes les 60 secondes) si les données du GitHub Gist ont changé et proposer de mettre à jour l’application.

7. Ajouter une fonction Doublie-clique sur le titre Budget pour revenir à l'accueil sur le mois actuel.

7. Ajouter des commentaires dans le code pour expliquer les parties importantes.

8. À la fin de ta réponse :

* explique les améliorations apportées
* explique comment installer la PWA
* explique comment fonctionne la synchronisation.

Je vais maintenant te fournir le fichier complet de l'application.
