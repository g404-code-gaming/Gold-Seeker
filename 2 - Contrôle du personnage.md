# Contrôle du personnage

Passons maintenant aux contrôles du personnage.

> Le personnage peut se déplacer dans quatre directions : haut, bas, gauche, droite. Lorsque le joueur choisit d'avancer, le personnage se déplace dans la direction souhaitée et ne s'arrête que s'il rencontre un obstacle, obligeant le joueur à être réactif : il faut éviter de tomber dans un piège.

### Déplacements

Pour commencer, ajoutez une [variable](https://github.com/g404-code-gaming/GDevelop_Cour/blob/main/Variables.md) **Direction** à votre personnage. Cette variable servira à savoir dans quelle direction il doit aller. 

Nous allons également créer une variable **Movable**, qui permet de savoir si notre personnage peut bouger ou non.

![variable](https://github.com/g404-code-gaming/Blop/blob/main/Image/deplacement_evenement_0.JPG)

Ensuite, allez dans la fenêtre des [événements](https://github.com/g404-code-gaming/GDevelop_Cour/blob/main/%C3%A9v%C3%A8nements.md).  
Commencez par ajouter des événements permettant de changer la variable **Direction** en fonction de la touche sur laquelle on appuie.

Une fois que c'est fait, ajoutez les événements qui déplacent le personnage en fonction de la valeur de sa variable **Direction** :

- **"Droit"** : Le personnage se déplace de **+100** sur l'axe X  
- **"Gauche"** : Le personnage se déplace de **-100** sur l'axe X  
- **"Haut"** : Le personnage se déplace de **-100** sur l'axe Y  
- **"Bas"** : Le personnage se déplace de **+100** sur l'axe Y

![variable](https://github.com/g404-code-gaming/Blop/blob/main/Image/deplacement_evenement_1.JPG)

Et maintenant, le personnage peut se déplacer grâce aux touches que nous avons choisies !  
Lancez l’aperçu pour voir ce que ça donne.

### Personnage et Collisions

Le personnage traverse le mur ? Pas de panique : nous allons gérer ce problème. 

Il existe un comportement **Physic2D** qui permet aux personnages de bloquer contre les murs et autres obstacles. 

![variable](/Image/deplacement_mur_0.JPG)

Ajoutez ce comportement à votre personnage, en mettant les paramètres suivants : 

![variable](/Image/deplacement_mur_1.JPG)

Ensuite, ajoutez-le à vos murs, en mettant cette fois-ci les paramètres suivantes : 

![variable](/Image/deplacement_mur_2.JPG)

Ajoutez le comportement ci-dessus à tout les objets de votre jeu que le personnage ne peut pas traverser. 

Avec tout ça, nous avons un personnage qui peut se déplacer et qui ne traverse pas les murs.  
Le labyrinthe prend vie petit à petit.

[étape 3 : Gestion des pièces et de la fin de partie](https://github.com/g404-code-gaming/Blop/blob/main/3%20-%20Argent.md)
