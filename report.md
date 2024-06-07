1. Initialisation et Configuration
    a. Clonage
        git clone https://github.com/Pelpav/repository
        Créer report.md
        git add report.md
        git commit -m "Initial Commit"
        git push origin main
    b. Config user.email et user.name
        git config --global user.email "elpav2022@gmail.com"
        git config --global user.name "Pelpav"
2. Création de branches et de développement
    a. Créer et basculer vers une nouvelle branche nommée "feature"
        git checkout -b feature
    b. Ajouter  un fichier Readme.md avec une description du projet
        créer un fichier README.md et ajouter ### Projet de Christian
        git add README.md
    c. Committer les changements
        git commit -m "Ajout du fichier README.md"
3. Gestion des conflits
    a. Retourner sur la branche main et envoyer les dernières modifications vers le dépot distant
        git checkout main
        git push origin main
    b. Basculer sur la branche feature et récupérer les dernières modifications de la branche main
        git checkout feature
        git pull origin main
    c. Resoudre le conflit et commiter les changements
        git add .
        git commit -m "Résolution du conflit"
    d. Pousser les changements sur la branche "feature"
        git push origin feature
4. 