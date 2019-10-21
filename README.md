Bonjour, Voici la mise à jour de la documentation.

# 1) récupérer le projet

git clone https://github.com/kisskool95/Recettes-Ansibles.git

# 2) installer les requirements.yml

ansible-galaxy install -r requirements.yml

# 3) Jouer le playbook system.yml

ansible-playbook system.yml -i hosts

# 4) Jouer le playbook Mysql.yml
ce playbook lancera les autres playbooks:
ansible-playbook mysql.yml -i hosts
installation :
- base de donnée mysql
- creer utilisateur mysql
- backup
- replication maitre esclave

# 5) Jouer le playbook apache.yml
ce playbook install apache 2 et php et met en place un vhost par defaut 
