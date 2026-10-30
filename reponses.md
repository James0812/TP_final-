
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

## Mission 11 - Correction isolée
- Commande utilisée : `git cherry-pick 80f2479`
- Identifiant du commit récupéré : `80f2479`
- Pourquoi pas une fusion classique : Une fusion  aurait récupéré l'intégralité des 3 commits de la branche de test . `git cherry-pick` permet d'appliquer uniquement le commit de correction orthographique .

## Mission 12 - Version stable
- Explication des trois nombres de `1.0.0` (Semantic Versioning) :
  - 1 (Majeur) : Modifications majeures .
  - 0 (Mineur) : Ajout de fonctionnalités .
  - 0 (Patch) : Corrections de bugs .
- Version suivante selon le cas :
  - Correction de bug mineur : `v1.0.1`
  - Nouvelle fonctionnalité compatible : `v1.1.0`
  - Refonte majeure incompatible : `v2.0.0`

## Mission 13 - Configuration des exclusions
- Éléments ignorés : `debug.log`, `cache/`, `.env`
- Le fichier `.gitignore` est bien enregistré .


## Questions finales

1. **Différence entre zone de travail, zone de staging et historique :**
   - **Zone de travail  :** Les fichiers modifiés directement sur le disque.
   - **Zone de staging  :** La zone intermédiaire où on prépare les fichiers sélectionnés avec `git add`.
   - **Historique :** L'ensemble des commits sauvegardés définitivement dans la base Git avec `git commit`.

2. **Intérêt d'une branche dédiée :**
   Travailler sur une nouvelle fonctionnalité dans son coin sans risquer de casser le code propre et stable de la branche principale.

3. **Différence `git reset` (mission 8) vs `git revert` (mission 9) :**
   `git reset` efface le commit de l'historique . `git revert` crée un nouveau commit qui annule les modifications passées sans supprimer l'historique (indispensable pour du code déjà partagé).

4. **Utilité de `git stash` :**
   Mettre ses modifications non terminées de côté pour changer de branche ou traiter une urgence rapidement, sans devoir faire un commit incomplet.

5. **`git cherry-pick` vs `git merge` :**
   `git cherry-pick` permet d'importer un seul commit précis   sans être obligé de fusionner toute la branche et ses autres modifications non voulues.

6. **Rôle de HEAD :**
   C'est le pointeur qui indique sur quel commit ou sur quelle b ranche on se    trouve actuellement.

7. **Signification de HEAD~2 :**
   Le commit situé 2 niveaux avant le commit actuel (`HEAD`).

8. **Rôle d'un tag Git :**
   Poser un repère fixe et facile à lire sur un commit précis, principalement pour m arquer une version officielle .

9. **Intérêt des commits petits et précis :**
   Rendre l'historique clair faciliter la recherche de bugs et pouvoir corriger ou annuler une modification précise sans impacter le reste.

10. **Raison de ne pas versionner certains fichiers :**
    Sécurité  et éviter d'alourdir le dépôt avec des fichiers inutiles .
