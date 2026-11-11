# Tableaux de bord (accès protégé)

Ce dépôt publie un site statique sur GitHub Pages. La page est **chiffrée** (AES-256, clé dérivée du mot de passe par
PBKDF2-SHA256, 600 000 itérations) : sans le mot de passe, le contenu est illisible, même en téléchargeant les fichiers.
Le navigateur du visiteur déchiffre la page sur place ; le mot de passe n'est envoyé à aucun serveur.

Ne modifiez pas ces fichiers à la main. Le site a été mis en ligne depuis le tableau de bord lui-même (onglet « Mettre à jour »,
carte « Publier cette version sur le site ») et se met à jour de la même façon, avec le même mot de passe : les visiteurs gardent
leur accès. Pour changer le mot de passe : script `publier.py` (dossier `05_Application_en_ligne/tableaux_de_bord_proteges` des
livrables, site v4), qui ne garde alors qu'une seule version dans l'historique.

Réglage GitHub (une seule fois) : Settings > Pages > Build and deployment > Source : Deploy from a branch ;
branche par défaut du dépôt (main), dossier `/ (root)` ; Save.
