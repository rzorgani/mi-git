git init
créer le fichier1.txt
ajouter le texte dans le fichier1
git add .
git commit -m "ajout de fichier1"
git push --set-upstream origin master


créer le fichier2.txt
ajouter le texte dans le fichier12.txt
git status
git add fichier2.txt
git push


git log
git log
commit 3ef71345860c7fca9ccd8086f5d98712faa89370 (HEAD -> master, origin/master)
Author: rzorgani <contact@zr-consulting.fr>
Date:   Sat Jan 7 17:39:11 2023 +0100

    ajout du fichier2

commit 6f1c007abd0cd1ee7341347c3f0fb7c82b5bc71c
Author: rzorgani <contact@zr-consulting.fr>
Date:   Sat Jan 7 17:35:16 2023 +0100

    ajout du fichier1


git checkout 6f1c007abd0cd1ee7341347c3f0fb7c82b5bc71c
Note: switching to '6f1c007abd0cd1ee7341347c3f0fb7c82b5bc71c'.

nous sommes switcher sur le commit numéro 1

on remarque que le fichier2 n'existe plus 

pour retourner à l'état actuel il faut switcher sur la branche master

git checkout master


on va créer et switcher sur la branche test1
git checkout -b test1

on va supprimer la branche test1 en local 
git branch -d test1

git checkout -b test2
git push --set-upstream origin test2

git checkout master

git branch
* master
  test2
on va supprimer la branche test2 du en local et de serveur
git branch -D test2

git branch
* master

on va créer et switcher sur la branche test3
git checkout -b test3

modifier le fichier2.txt
commiter et pusher les modifications
git status
git add fichier2.txt
git commit -m "modifier fichier 2"
git push --set-upstream origin test3


git checkout master

les modifications de fichier2 qui se trouve sur la branche test3 ne sont présent, donc on va merger la branche test3 dans master

git merge test3
Updating 3ef7134..03be562
Fast-forward
 fichier2.txt | 8 +++++++-
 1 file changed, 7 insertions(+), 1 deletion(-)

 