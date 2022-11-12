### Users Clients table


Je vois que tu as le field `is_admin`. Est ce que le user ne peut avoir que deux roles: admin ou pas admin?
Je pense que dans le cadre d'une boutique e-commerce un utilisateur peut avoir les roles suivant : `administrateur`, `editeur`, `lecteur`.
Donc je te suggere, aulieu de `is_admin` tu aura `role` qui sear un `enum` de  `administrateur`, `editeur` et `lecteur`


### Articles table
La table Articles a une association `n` to `n` avec  la table Categorie mais la l'association doit se materialisrer avec leur cles respectives. Dans la table Articles, je pense que l'on devrait avroir `Category_id`, on devrait donc avoir `foreignId`au lieu de string



