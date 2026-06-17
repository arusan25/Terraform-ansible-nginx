# Projet : Déploiement d’un serveur Nginx avec Terraform et Ansible

Ce dépôt contient mon travail pour mettre en place un petit environnement avec Terraform et installer automatiquement Nginx grâce à Ansible.  
L’idée était surtout de comprendre comment automatiser une installation simple et organiser un projet proprement.

---

## Objectif du projet

L’objectif était de :
- créer une machine (ou un environnement) avec Terraform,
- installer Nginx automatiquement,
- déployer une page web basique,
- garder une structure claire dans le dépôt.

Ce n’est pas un gros projet, mais ça m’a permis de revoir les bases d’Infra-as-Code et d’Ansible.

---

## Technologies utilisées

- Terraform  
- Ansible  
- Nginx  
- AWS (EC2)  
- Git / GitHub  

---

## Structure du dépôt

Nginx/
│── main.tf
│── inventory.ini
│── site.yml
│── site web.png
│── .gitignore

Code

### Description rapide des fichiers

- **main.tf** : configuration Terraform (création de l’infra).
- **inventory.ini** : inventaire Ansible (ici en local pour les tests).
- **site.yml** : playbook qui installe Nginx et déploie une page HTML.
- **site web.png** : capture du résultat final.
- **.gitignore** : pour éviter d’envoyer les fichiers Terraform inutiles.

---

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

Après ça, Nginx est installé et la page web est en place.

---

## Résultat

Une fois le playbook exécuté, on peut accéder à la page web.  
J’ai ajouté une capture d’écran dans le dépôt : **site web.png**.

---

## Auteur

Projet réalisé par **RAVEENDRAKUMAR ARUSAN** dans le cadre d’un TP sur l’automatisation et le déploiement.

Si tu veux, je peux aussi te faire une version :

plus courte

plus technique

avec un schéma d’architecture

Tu me dis ce que tu préfères.

en 1 seul fichier stp tu separe la
Compris Arusan — tu veux un seul fichier, sans séparation, sans style IA, juste un README simple, humain, naturel.

Voici TON README.md, en un seul bloc, prêt à copier-coller.

markdown
# Projet : Déploiement d’un serveur Nginx avec Terraform et Ansible

Ce projet a pour but de déployer une machine et d’installer automatiquement Nginx dessus. J’ai utilisé Terraform pour la partie infrastructure et Ansible pour la configuration. L’objectif était surtout de comprendre comment automatiser une installation simple et organiser un projet proprement.

## Objectifs du projet

- Créer une machine avec Terraform  
- Installer Nginx automatiquement avec Ansible  
- Déployer une petite page web  
- Garder une structure claire dans le dépôt  

Ce n’est pas un gros projet, mais il m’a permis de revoir les bases d’Infra-as-Code et d’Ansible.

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
- **inventory.ini** : inventaire Ansible (ici en local pour les tests).  
- **site.yml** : playbook qui installe Nginx et déploie une page HTML.  
- **site web.png** : capture du résultat final.  
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

Après ça, Nginx est installé et la page web est en place.

## Résultat

Une fois le playbook exécuté, on peut accéder à la page web.  
J’ai ajouté une capture d’écran dans le dépôt : **site web.png**.

## Auteur

Projet réalisé par **RAVEENDRAKUMAR ARUSAN** dans le cadre d’un TP sur l’automatisation et le déploiement.