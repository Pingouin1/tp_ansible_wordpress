Installer ansible sur la machine hôte, [ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html).

Dans `host_vars`, éditer le fichier `devopswebserv.yml` :

- Remplacer `mySQLuser` par votre nom d'utilisateur et `IP` par l'adresse IP de votre serveur mySQL

Éditer `ansible.cfg` :

- Indiquer l’utilisateur de la machine pour la variable `remote_user`.

Dans `roles\mysql\default\main.yml`, indiquer les identifiants à utiliser.

A la racine de votre projet, lancer la commande `ansible-playbook -i invent ory playbook.yml`
