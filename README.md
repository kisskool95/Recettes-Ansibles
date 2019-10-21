Ci-dessous la description complète du projet et des différentes étapes à jouer.
Repo en public


# 1) Récupérer le projet via:

git clone https://github.com/kisskool95/Recettes-Ansibles.git

# 2) Installer les requirements.yml

ansible-galaxy install -r requirements.yml

# 3) Jouer les playbooks system.yml
     #Le fichier system.yml contient l'ensemble des tâches obligatoires pour les serveurs (fichier hosts, création des users pour les         databases, Dépot des clés SSH...)
ansible-playbook system.yml -i hosts
ansible-playbook mysql.yml -i hosts
ansible-playbook mysql_backup.yml -i hosts
