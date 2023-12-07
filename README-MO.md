# Meeting optimizer
![](https://media4.giphy.com/media/vS2CaLlDWLky9McAFu/giphy.gif?cid=ecf05e476qwikq8dk8j5fpxd9fwsyodbv6wcvvuwz2vj5486&ep=v1_gifs_search&rid=giphy.gif&ct=g)

Une logique simple pour maximiser les rencontres entre les personnes lors d'un évènement.

Cet évènement contient plusieurs tours de rencontres (au choix). A chaque tour, les personnes doivent se rendre dans une salle qui correspond à une couleur. 

La logique dans le code (voir [[LOGIC ENGINE]]) fait en sorte qu'à la fin de tous les tours, le brassage ait été optimisé et donc que chaque personne ait rencontré un maximum d'autres personnes lors de l'évènements. 

## Modélisation de la réalité


* **une salle** = une couleur (🔴🔵🟠🟢)
* **une personne** = une combinaison de couleur dont la longueur (length) correspond au nombre de tour
* **nombre de tours de rencontre** = longueur de la combinaison de couleurs (_si la combinaison contient 3 couleurs, c'est qu'il y a 3 tours_)


## Logique 

Je demande à la machine de suivre la logique suivante : 
1. garde en mémoire toutes les salles dans lesquelles les personnes peuvent aller lors de l'évènement
2. génère toutes les combinaisons possibles de 3 salles parmi les 4 possibles
3. créé un jeu de données dans lequel chaque ligne correspond à une combinaison unique de 3 salles
4. répète l'étape 3 autant de fois qu'il faut pour couvrir le nombre de participants attendus (sachant qu'il y 24 combinaisons uniques de 3 couleurs parmi une liste de 4) et nomme bien les colonnes de manière à ce qu'on comprenne que chacune d'entre elle correspond à un tour dans l'évènement. 


## Schéma de la logique 

