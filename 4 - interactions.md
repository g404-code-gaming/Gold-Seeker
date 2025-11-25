# Interactions avec l'environnement

Maintenant que nous avons la base du jeu, nous allons ajouter des **éléments d'interaction** pour le rendre plus difficile et plus amusant.

## Lave et mort du joueur

Ajoutons un moyen de faire perdre le joueur : un **lac de lave** qui le force à recommencer le jeu en cas de contact.

![image](https://github.com/g404-code-gaming/Blop/blob/main/Image/inter_1.JPG)

Il faut d'abord ajouter un [objet](https://github.com/g404-code-gaming/GDevelop_Cour/blob/main/Objets.md) pour représenter notre lac de lave.

Ensuite, il faut créer un [événement](https://github.com/g404-code-gaming/GDevelop_Cour/blob/main/%C3%A9v%C3%A8nements.md) qui, lorsque le personnage du joueur touche la lave, le supprime et le fait recommencer la partie.

![image](https://github.com/g404-code-gaming/Blop/blob/main/Image/inter_2.JPG)

C'est tout ! Il ne reste plus qu'à jeter le personnage dans la lave pour vérifier si notre programme fonctionne.

## Porte et clé

Nous allons ajouter une **porte**. Elle bloque le passage du personnage et ne peut s'ouvrir qu'avec une **clé**.

![image](https://github.com/g404-code-gaming/Blop/blob/main/Image/inter_3.JPG)

Dans un premier temps, il faut ajouter la porte et la clé à la scène. La porte est un objet qu'il faut placer dans le groupe **Bloc**.

Commençons par créer une variable de scène **Key** qui compte le nombre de clés que possède le joueur :

![image](https://github.com/g404-code-gaming/Blop/blob/main/Image/inter_4.JPG)

Ensuite, ajoutons un texte **TextKey** qui va afficher à l'écran le nombre de clés possédées par le joueur.

Nous pouvons maintenant créer l'événement qui permet de ramasser une clé.

![image](https://github.com/g404-code-gaming/Blop/blob/main/Image/inter_5.JPG)

Maintenant que notre personnage peut ramasser des clés, il nous reste à créer l'événement permettant d'ouvrir la porte si le joueur possède une clé.

![image](https://github.com/g404-code-gaming/Blop/blob/main/Image/inter_6.JPG)

Il faut vérifier que tout fonctionne : on ne doit pas pouvoir traverser la porte sans clé !

## Bloc poussable

Ajoutons un **bloc**, un obstacle que le personnage peut pousser.

![image](https://github.com/g404-code-gaming/Blop/blob/main/Image/inter_7.JPG)

Ajoutez l'objet à la scène.

Pour que le personnage ne puisse pas traverser l'objet, mais puisse quand même le déplacer, il faut lui ajouter le comportement **Physic2D**, et mettre les mêmes paramètres que ceux du Player (voir fin du chapitre 2).

Utilisez le bloc pour condamner un passage, forçant le joueur à le pousser pour trouver son chemin.

Voilà ! Vous avez ajouté de la lave pour éliminer le personnage, ainsi que des portes et des blocs poussables pour augmenter le défi. Gold Seeker commence à devenir un vrai jeu !

[étape 5 - Finalisation](https://github.com/g404-code-gaming/Blop/blob/main/5%20-%20fin.md)
