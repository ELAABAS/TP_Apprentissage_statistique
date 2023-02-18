# ISIMA ZZ2F4 2022-2023 - Apprentissage statistique : TP noté
## Introduction

Ce projet a pour objectif de développer un modèle de classification pour détecter les comportements anormaux de vaches laitières dans une ferme de haute précision. Les données ont été collectées en hiver, lorsque les vaches sont à l'étable, à l'aide de capteurs positionnés sur les vaches qui ont enregistré le nombre de secondes passées dans chacune des trois salles de l'étable (logettes, salles des auges et allées). Le fichier xTrain.csv contient les caractéristiques nécessaires à la prédiction de comportements anormaux ou non, tandis que le fichier yTrain.csv contient l'état de la vache après 24 heures. Les valeurs de sortie sont égales à 0 si l'état est considéré comme normal et 1 sinon.
Données

Les données sont disponibles sous la forme de trois fichiers:

    xTrain.csv: caractéristiques nécessaires à la prédiction des comportements anormaux ou non des vaches.
    yTrain.csv: état de la vache après 24 heures.
    xEval.csv: caractéristiques nécessaires à la prédiction des comportements anormaux ou non des vaches pour le jeu de test.

Les attributs dans les fichiers xTrain.csv et xEval.csv sont:

    date hour: date et heure du premier enregistrement.
    idCow: identifiant de la vache.
    all+i: nombre de secondes passées dans les allées pour l'heure date hour + i (i compris entre 0 et 23).
    rest+i: nombre de secondes passées dans les logettes pour l'heure date hour + i (i compris entre 0 et 23).
    eat+i: nombre de secondes passées dans la salle des auges pour l'heure date hour + i (i compris entre 0 et 23).

Le fichier yTrain.csv contient une seule colonne indiquant l'état de la vache après 24 heures. Les valeurs sont 0 si l'état est considéré comme normal et 1 sinon. Il y a des valeurs manquantes sous la forme de NaN dans le fichier xTrain.csv, tandis que le fichier xEval.csv a déjà été nettoyé.
## Objectif

L'objectif est de trouver le meilleur modèle de classification pour prédire les comportements anormaux des vaches. Il est possible d'utiliser différents algorithmes d'apprentissage supervisé vus en cours et/ou de modifier ces algorithmes. Les réseaux de neurones ne sont pas autorisés. Les résultats seront évalués en utilisant la fonction sklearn.metrics.f1_score et la matrice de confusion. Les prédictions devront être envoyées au format CSV, au plus tard 5 jours avant la date de rendu.
## Rapport

Le rapport devra contenir une explication claire du pipeline utilisé pour la prédiction, ainsi que des détails permettant la reproduction de ce pipeline. Les justifications sur le choix de la pipeline devront être appuyées par des références bibliographiques. Il faudra également expliquer le choix des paramètres et le protocole expérimental mis en place, ainsi qu'une analyse détaillée des résultats obtenus et des performances du modèle de prédiction.

Le rapport devra commencer par une introduction claire et concise sur le contexte de la prédiction et les objectifs poursuivis. Il faudra également décrire les données utilisées pour entraîner et tester le modèle de prédiction.

Ensuite, le rapport devra détailler le pipeline utilisé pour la prédiction, en expliquant les différentes étapes du processus, telles que la préparation des données, l'extraction des caractéristiques, la sélection de modèle, l'optimisation des paramètres, etc. Les justifications pour chaque étape du pipeline devront être fournies, avec des références bibliographiques pour étayer les choix effectués.

Le rapport devra également décrire le protocole expérimental utilisé pour l'évaluation du modèle de prédiction, en expliquant les métriques utilisées pour évaluer les performances du modèle, ainsi que la méthode de validation croisée ou de test utilisée.

Enfin, le rapport devra fournir une analyse détaillée des résultats obtenus, en présentant les performances du modèle sur les données de test et en comparant ces performances avec celles d'autres modèles de référence. Les avantages et les limites du modèle de prédiction devront être discutés, ainsi que les perspectives d'amélioration pour des travaux futurs.

Le rapport devra être structuré de manière claire et précise, avec des titres et des sous-titres pour faciliter la lecture. Les références bibliographiques devront être citées dans le texte et listées en fin de rapport.