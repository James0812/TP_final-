
## Mission 5 - Analyse du projet
1. Identifiant court du premier commit : <b01ba2c>
2. Commit correspondant à la page Contact : <0e746f9>
3. Nombre actuel de commits : <6>
4. Commande utilisée pour l'historique graphique : git show 0e746f9 


## Mission 8 - Commit local incorrect
- Commande utilisée : `git reset HEAD~1`
- Explication : `git reset`  supprime le commit de l'historique mais garde les modifications apportés.
- Méthode pour tout supprimer : La commande `git reset --hard HEAD~1` aurait également supprimé les modifications .

## Mission 9 - Commit partagé à annuler
- Explication : `git revert` crée un nouveau commit qui annule les modifications du commit dont on parle. quand  a `git reset`, il ne réécrit pas l'historique.