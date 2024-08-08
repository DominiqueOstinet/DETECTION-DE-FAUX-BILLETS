DETECTION DE FAUX BILLETS AVEC PYTHON

Ce projet a été réalisé dans le cadre de ma formation Data Analyst chez OpenClassrooms.

Objectif : construire un algorithme qui, à partir des caractéristiques géométriques d’un billet, serait capable de définir si ce dernier est un vrai ou un faux billet.

Données : un fichier d’exemple contenant 1500 billets : 1 000 sont vrais et 500 sont faux avec six informations géométriques :
- length : la longueur du billet (en mm),

- height_left : la hauteur du billet (mesurée sur le côté gauche, en mm)
- height_right : la hauteur du billet (mesurée sur le côté droit, en mm)
- margin_up: la marge entre le bord supérieur du billet et l'image de celui-ci (en mm)
- margin_low: la marge entre le bord inférieur du billet et l'image de celui-ci (en mm)
- diagonal : la diagonale du billet (en mm)

Une colonne supplémentaire précise la nature du billet (« is genuine » : « False / True).



L'étude a été réalisée sur un Notebook GoogleColab , plusieurs méthodes d’analyses ont été menées :

- Régression linéaire multiple : Analyse de la relation des dimensions du billet entre elles pour compléter les valeurs manquantes
-	Régression logistique : Modélisation de la probabilité qu'un billet soit authentique en fonction de ses caractéristiques géométriques
- Clusterisation (K-means) : Regroupement des billets en clusters pour explorer les similarités géométriques
- Random Forest : Modélisation de la classification des billets en utilisant un ensemble d'arbres de décision pour déterminer s'ils sont authentiques ou non
