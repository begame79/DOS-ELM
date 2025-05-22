# DOS-ELM
Prédiction de la RUL avec DOS-ELM (C-MAPSS)

Ce dépôt contient l’implémentation du modèle DOS-ELM (Denoising Online Sequential Extreme Learning Machine) pour la prédiction de la Remaining Useful Life (RUL) des moteurs d’avion à partir des données C-MAPSS de la NASA.

Le modèle est appliqué aux quatre scénarios de panne du jeu de données :
FD001 : 1 condition de fonctionnement, 1 mode de panne
FD002 : plusieurs conditions, 1 mode de panne
FD003 : 1 condition, plusieurs modes de panne
FD004 : plusieurs conditions, plusieurs modes de panne

Objectif
Utiliser un autoencodeur débruiteur combiné à une ELM séquentielle pour :
traiter des données capteurs bruitées, apprendre en ligne, prédire efficacement la durée de vie restante (RUL).

Contenu
Chaque scénario a son propre notebook :
DOS_ELM_FD001.ipynb
DOS_ELM_FD002.ipynb
DOS_ELM_FD003.ipynb
DOS_ELM_FD004.ipynb

Données
Jeu de données : C-MAPSS 

Prétraitement : suppression des capteurs constants, normalisation, ajout de bruit contrôlé

Librairies utilisées
NumPy, Pandas, Matplotlib
scikit-learn
