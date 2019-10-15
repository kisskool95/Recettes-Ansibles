Bonjour, Voici la mise à jour de la documentation.

# 1) récupérer le projet

git clone https://github.com/kisskool95/Recettes-Ansibles.git

# 2) insaller les requirements.yml

ansible-galaxy install -r requirements.yml

# 3) Jouer le playbook system.yml

ansible-playbook system.yml -i hosts

# 4) Jouer le playbook Mysql.yml

ansible-playbook mysql.yml -i hosts