les branches sur github sont un peu comme des version du livre. la branche main est la version finale et les autres branches que tu cree sont comme des brouillons ou tu peux faire tout ce que tu souhaite sans risque de casser ton projet.

Etapes
## Creer une nouvelle branche (nommee dev)
    git checkout -b dev
### exp de branche: dev/nouvelle-fonctionnalite

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