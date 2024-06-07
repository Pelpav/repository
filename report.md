1. Initialisation et Configuration
    a. Clonage
        git clone https://github.com/Pelpav/repository
        Créer report.md
        git add report.md
        git commit -m "Initial Commit"
    b. Configurer user.email et user.name
        git config --global user.email "elpav2022@gmail.com"
        git config --global user.name "Pelpav"
2. Création de branches et développement
    a. Créer et basculer vers une nouvelle branche nommée "feature"
        git checkout -b feature
    b. Ajouter un fichier README.md avec une description du projet
        créer un fichier README.md et ajouter ### Projet de Christian
        git add README.md
    c. Committer les changements
        git commit -m "Ajout du fichier README.md"
3. Gestion des conflits
    a. Retourner sur la branche main et envoyer les dernières modifications vers le dépôt distant
        git checkout main
        git push origin main
    b. Créer un fichier nommé index.html et le remplir
        git add index.html
        git commit -m "Création du fichier index.html"
    c. Basculer vers la branche feature tout en veillant à ne pas perdre le contenu de index.html
        git stash
        git checkout feature
    d. Ajouter des commentaires dans README.md
        git add README.md
        git commit -m "Ajout de commentaires"
    e. Envoyer vers le dépôt
        git push origin feature
    f. Retourner sur la branche principale et compléter le fichier index.html
        git checkout main
        compléter le fichier index.html
        git add index.html
        git commit -m "Complétion du fichier index.html"
    g. Fusionner la branche feature dans main en résolvant les conflits avec rebase
        git checkout main
        git rebase feature
        (résoudre les conflits si nécessaire)
        git add .
        git rebase --continue
        git push origin main$
        git add .
        git commit -a -m "Final commit"