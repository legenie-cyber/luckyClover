les branches sur github sont un peu comme des version du livre. la branche main est la version finale et les autres branches que tu cree sont comme des brouillons ou tu peux faire tout ce que tu souhaite sans risque de casser ton projet.

Etapes
# Initialisation en ligne
> apres avoir cree le depot github recopier les commandes de la secondes section: celles ci

    git remote add origin https://github.com/legenie-cyber/luckyClover.git 

    git branch -M main
    
- git remote add origin https://github.com/legenie-cyber/luckyClover.git  donne un nom (origin) a ton depot en ligne

## Creer une nouvelle branche (nommee dev)
    git checkout -b dev
 exp de branche: dev/nouvelle-fonctionnalite

## Pour envoyer la branche vers le depot distant
    git push -u origin dev

## Faire des modifications, sauvegardes, et envoit
    git add .
    git commit -m 'Test de deploiement' //pour un nouveau commit
    git push origin dev 

## Pour les restaurations
    git revert //pour annuler les changements du dernier commit. 
    git checkout (ou restore) // pour revenir a l'etat precis d'un commit

## Commandes
    git checkout branche // pour se deplacer sur une branche
    git merge branche // pour fusionner un branche avec la branche principale (main)

## Etapes
    git checkout -b dev
    git add. / git commit
    // si tout est okay
    git checkout main
    git merge dev
    git push

### git remote -v permet de voir vers quelle URL pointe origin