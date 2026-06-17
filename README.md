# Projet : Déploiement d’un serveur Nginx avec Terraform et Ansible

Ce projet a pour but de déployer une machine et d’installer automatiquement Nginx dessus. J’ai utilisé Terraform pour créer l’infrastructure et Ansible pour installer et configurer le serveur. L’objectif était surtout de comprendre comment automatiser une installation simple et organiser un petit projet proprement.

## Objectifs du projet

- Créer une machine avec Terraform  
- Installer Nginx automatiquement avec Ansible  
- Déployer une page web simple  
- Garder une structure claire dans le dépôt  

Ce projet m’a permis de revoir les bases d’Infra-as-Code et d’Ansible.

## Technologies utilisées

- Terraform  
- Ansible  
- Nginx  
- AWS (EC2)  
- Git / GitHub  

## Structure du dépôt

Nginx/
│── main.tf
│── inventory.ini
│── site.yml
│── site web.png
│── .gitignore

Code

### Description des fichiers

- **main.tf** : configuration Terraform pour créer l’infrastructure.  
- **inventory.ini** : inventaire Ansible.  
- **site.yml** : playbook qui installe Nginx et déploie une page HTML.  
- **site web.png** : capture d’écran du résultat.  
- **.gitignore** : pour éviter d’envoyer les fichiers Terraform inutiles.  

## Déploiement

### 1. Initialiser Terraform
terraform init

Code

### 2. Créer l’infrastructure
terraform apply -auto-approve

Code

### 3. Lancer Ansible
ansible-playbook -i inventory.ini site.yml

Code

Après l’exécution du playbook, Nginx est installé et la page web est accessible.

## Résultat

Une capture d’écran du site est disponible dans le fichier **site web.png**.

## Auteur

Projet réalisé par **RAVEENDRAKUMAR ARUSAN** dans le cadre d’un TP sur l’automatisation et le déploiment.