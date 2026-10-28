Q1.3 : 
Stockage:
disponible est stocké en INTEGER un nombre, 1 = vrai, 0 = faux.
date_ajout est stocké en TEXT

Rôle:
AUTOINCREMENT : l’id se met à jour tout seul.
UNIQUE sur nom : pas deux noms identiques.
CHECK (prix >= 0) : le prix ne peut pas être négatif.

ON DELETE RESTRICT:
On ne peut pas supprimer une catégorie si elle contient encore des produits.


Q1.4 :
Huile d''olive : sert à ouvrir et fermer un texte


Q3.2:
1-Deux fois DatabaseHelper():
Un seul objet est créé. Le deuxième appel renvoie le même objet que le premier.
C’est le rôle du mot-clé factory : le constructeur ne crée pas forcément un nouvel objet, il peut renvoyer une instance déjà existante.

2-Il signifie « si la variable est null, lui donner cette valeur ». Sinon, il ne fait rien.

3-Dans SQLite, ce réglage n’est pas gardé dans le fichier : il faut le réactiver à chaque ouverture. Dans onCreate, il ne serait activé que la toute première fois.

4-Une seule fois dans toute la vie de l’application : à la création du fichier de base de données.
Ensuite, le fichier existe déjà, donc onCreate n’est plus appelé.


