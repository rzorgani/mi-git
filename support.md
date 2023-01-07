initialisation de Git
git config --global user.name  "toto"
git config --global user.email "example@gmail.com"
git config --global --list

Versionner en local 
git init :  permet de convertir un projet existant, sans version en un dépôt Git

Gérer les commits
git log : liste des commits
git log -n2 : afficher les 2 derniers commits
git show sh1 : voir commit spésificque 
git checkout sh1 : remttre la version du sh1
git checkout main : remttre sur la version "main"

créer une branche puis switcher à la branche
git branch <branch_name>
git checkout <branch_name>

créer et switcher à la branche en même temps
git checkout -b <branch_name>

supprimer une branche locale
git branch -d <branch_name>



Autre commande 
git status : état du fichier 
git diff :afficher les modifs avant commit
git branch : pour afficher la lisyte des branches
git merge autre_branche : merger autre_branche avec la branche actuel 


Versionner sur un dépôt distant
git clone lien-gitlab.com : récupérer le travail depuis dépôt distant
git push -u origin main : posse les modifications vers le serveurs et sur la branche main
git push -f origin main : posse de force les modifications vers le serveurs et sur la branche main (à utiliser avec précaution)
