# Prédiction de la récidive du patient lors d’un cancer de la prostate

[Voir le rapport du projet](https://acrobat.adobe.com/id/urn:aaid:sc:EU:a59847e8-44e6-4008-b5ef-90eb5ac3f150)

## Le contexte du projet 

Au cours de la licence MIASHS (Mathématiques et Informatique Appliquées aux Sciences Humaines et Sociales) j'ai étudié de nombreuses méthodes statistiques et de programmation. Dans ce contexte, nous étions missionnés de réaliser un projet sur l'ensemble du dernier semestre de licence par groupe de quatre, qui regroupe un grand nombre de compétences à mettre en avant lors de ce projet. Chaque enseignant choisissait un sujet sur lequel il a travaillé dans le passé, et un groupe qui allait travailler dessus. 
Nous avons tout de suité été, avec mon équipe, enthousiasmés par l'idée de travailler sur un projet comme celui ci. Il contenait une grande part de statistique, mais également un aspect traitement d'images, qui nous semblait ambitieux suite à un formation (la licence) qui avait été jusqu'à lors plutôt théorique.

## Le traitement des données

Après un premier échange sur les attentes du projet, notre encadrante, Aurélie Fargeas, nous a transmis la base de données avec laquelle nous allions travailler. Elle contenait initialement 100 variables pour 565 individus. Voici un rapide résumé des tâches qui ont été réalisées dessus : 

- Nettoyage de la base (traitement des NA, valeurs aberrantes...)
- Statistiques Descriptives (Tendance centrale, dispersion, représentation graphique croisée...)

## Création de modèle pertinent

Une fois avoir pris le temps de nettoyer et mieux appréhender la base de données, nous avons cherché à créer un modèle qui était des plus pertinent pour chercher à expliquer les saignements des patients et leurs récidives.

- Séparation en échantillon apprentissage/test (Leave one cross out)
- Régression logistique
- Test de Wald

Ce modèle nous a permis de prédire la récidive avec une certaine probabilité.

## Traitement d'image

Cela n'est pas mentionné dans le rapport, mais nous avons à la suite du rendu du projet, continué à travailler dessus et notamment sur l'aspect traitement des images. Nous avons récupéré l'ensemble des IRM des patients et avons, utilisés différents packages avec R tels que "png" pour, avec la valeur des pixels, essayer de mettre en place des méthodes de deep learning qui détectent des groupes ayant des caractéristiques communes pour prévenir des chances de récidives.