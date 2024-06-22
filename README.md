# TimelineNumerique
Fichiers nécessaires pour faire fonction ce petit jeu à visées éducatives.  
Téléchargez tous les fichiers et placez les dans un même dossier et décompressez l'archive img **OU** téléchargez et décompressez l'archive TimelineNumerique, puis lancez le jeu en ouvrant sur index.html avec un navigateur Internet (ne nécessite cependant pas de connexion internet)

Consulter le fichier readme.html pour plus d'informations


## Bugs connus

- Quand une date à deviner se trouve déjà sur le plateau en plusieurs exemplaires, alors la détection du bon interval peut être fausse.  
  Explication possible : Quand la date Y est présente sur le plateau en un seul exemplaire alors on valide les réponses tombant dans l'intervalle [X;Y] et [Y;Z]. Quand la date Y est présente en plusieurs exemplaires alors il y a des intervalles du style [X;Y] [Y;Y] [Y;Y] [Y;Z]. Si l'intervalle donné est [Y;Z] il se peut que la réponse ne soit pas validée car de mémoire une recherche séquentielle est réalisée et il se peut que seul les deux premiers intervales (indices) soient sélectionnés pour tester la validation.
- Certaines images se chevauchent légèrement dans la frise.
