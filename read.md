1/ creer un dossier de projet dans le dossier xampp
2/ copier ce dossier dans visualcode
3/ créer les fichiers (html, css, js) dans visualcode
4/ dans le terminal editer les commandes:
    git init => crée un nouveau depot git
créer un nouveau repertoire sur github en faisant un copier coller du dossier de xampp.
   dans le terminal editer :
   git add . (ajoute les fichiers)
   git commit -m "message" (enregistre les modifs dans l'historique de depot)
   prendre l'url sur git hub correspondante au projet
   dans le terminal editer:
   git remote add origin (url).git
5/ créer une branche "dev": (j'ai crée une branche "essai")
    git checkout -b dev
6/ git branch -a (liste les branches locales et distantes)
7/ git checkout dev (positionne sur la branche dev)
8/ modifier le CSS dans visualcode 
    on est positionné sur la branche dev
    dansle terminal editer:
    git add . (ajoute)
    git commit -m "modif css" (enregistre)
9/  git push origin dev (depose sur github)
10/ git checkout main (retour sur la branche main) la modif n'apparait pas.
11/  rester sur main et editer:
    git pull origin main (met a jour)
    git merge dev (fusionne la branche dev avec main)
    git commit -m (enregistre)
    git push origin main (depose sur github)
12/ le css apparait sur dev
13/ editer: git checkout dev (retour branche dev)
            creer un fichier readme.md
14/         git add.
            git commit -m "creation fichier readme"
            git push origin dev

15/ visualiser difference entre main et dev editer:
            git diff dev main
16/ creer deux nouvelles branche dev1 et dev2: editer:
            git checkout -b dev1
            git checkout -b dev2
            git push -u origin dev1
            git push -u origin dev2
17/ dans chaque fichier dev1 et dev 2 editer une modif "modif dev1" et "modif dev2"
18/ comparer les deux branches: 
     git diff dev1..dev2
19/ git merge dev1
20/ git merge dev2
21/ git comit -m dev1
    git comit -a
    git fetch
    git commit -m "resolution de conflit"



       