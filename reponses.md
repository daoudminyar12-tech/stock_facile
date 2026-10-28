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
