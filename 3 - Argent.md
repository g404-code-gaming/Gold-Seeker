# L'argent, le nerf de la guerre ! 

Dans Gold Seeker, il faut ramasser toutes les pièces du niveau pour gagner la partie.

Si ce n'est pas déjà fait, il faut ajouter des pièces dans le jeu.

![image](https://github.com/g404-code-gaming/Blop/blob/main/Image/piece_1.JPG)

## Variables pour compter les pièces

Avant de s'occuper des événements, nous allons devoir créer une [variable de scène](https://github.com/g404-code-gaming/GDevelop_Cour/blob/main/Variables.md) **ArgentMax**. Il s'agit du nombre de pièces présentes dans la scène.

![image](https://github.com/g404-code-gaming/Blop/blob/main/Image/piece_2.JPG)

Dans les événements, on va initialiser cette variable : au lancement de la zone, on la remplit avec le nombre de pièces de la scène grâce à la commande *count()*.

![image](https://github.com/g404-code-gaming/Blop/blob/main/Image/piece_3.JPG)

Lorsque le nombre de pièces sur la scène est égal à 0, cela signifie que le joueur a remporté la partie. Pour l'instant, cela fait simplement recommencer le jeu, mais on verra plus tard comment changer de niveaux.

![image](https://github.com/g404-code-gaming/Blop/blob/main/Image/piece_4.JPG)

## Ramasser et afficher les pièces

Pour ramasser les pièces, il nous faut un [événement](https://github.com/g404-code-gaming/GDevelop_Cour/blob/main/%C3%A9v%C3%A8nements.md). Cet événement se décompose en plusieurs étapes : 

  - **Condition** : l'événement se déclenche lorsque notre personnage entre en collision avec une pièce.
  - **Action 1** : on supprime la pièce.
  - **Action 2** : on met à jour la variable **ArgentMax**.

![image](https://github.com/g404-code-gaming/Blop/blob/main/Image/piece_5.JPG)

Il faut tester le jeu pour voir si la partie se relance lorsqu'on ramasse toutes les pièces. Si oui, alors bravo !

Désormais, il nous reste à afficher le nombre de pièces qu'il faut ramasser pour gagner.

Nous allons d'abord créer un nouveau calque, que nous allons appeler **UI**.

![image](https://github.com/g404-code-gaming/Blop/blob/main/Image/piece_6.JPG)

Dans ce calque, nous allons ajouter un objet de type **Texte**, nommé **TextGold**.

![image](https://github.com/g404-code-gaming/Blop/blob/main/Image/piece_7.JPG)

Une fois que le texte est mis sur la scène, il faut lancer l'aperçu pour vérifier qu'il apparaît bien où il faut et qu'il suit le personnage correctement. Sinon, il y a une erreur qu'il faut corriger.

Il ne reste plus qu'à ajouter les actions propres au texte dans les événements. 

![image](https://github.com/g404-code-gaming/Blop/blob/main/Image/piece_8.JPG)

  Et voilà, désormais, on peut rammasser des pièces pour remporter la partie ! 

  [Partie 4 - Interactions](https://github.com/g404-code-gaming/Blop/blob/main/4%20-%20interactions.md)
