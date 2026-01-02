# Smart Home Project

Ce projet est une application de gestion de maison intelligente (Smart Home) composée d'un backend Spring Boot et d'un frontend Angular, orchestrés via Docker Compose.

## 🚀 Fonctionnalités

L'application permet de gérer des appareils connectés et leurs catégories.
-   **Backend** : API REST pour la gestion des appareils et catégories.
-   **Frontend** : Interface utilisateur pour visualiser et contrôler les appareils.

## 🛠 Technologies Utilisées

-   **Backend** : Java, Spring Boot
-   **Frontend** : Angular, Tailwind CSS
-   **Base de données** : PostgreSQL
-   **Conteneurisation** : Docker, Docker Compose

## 📋 Prérequis

Avant de commencer, assurez-vous d'avoir installé :
-   [Docker Desktop](https://www.docker.com/products/docker-desktop) (incluant Docker Compose)

## ⚙️ Installation et Démarrage

Le projet est configuré pour être lancé facilement avec Docker Compose.

1.  **Cloner le projet** (si ce n'est pas déjà fait) :
    ```bash
    git clone <votre-repo-url>
    cd TP24
    ```

2.  **Lancer l'application** :
    À la racine du projet (là où se trouve le fichier `docker-compose.yml`), exécutez :
    ```bash
    docker-compose up --build
    ```
    *L'option `--build` force la reconstruction des images Docker pour s'assurer que vous avez la dernière version du code.*

3.  **Arrêter l'application** :
    ```bash
    docker-compose down
    ```

## 🔌 Accès aux Services

Une fois les conteneurs démarrés, vous pouvez accéder aux services aux adresses suivantes :

| Service | URL | Description |
| :--- | :--- | :--- |
| **Frontend** | `http://localhost:80` | Interface utilisateur Angular |
| **Backend API** | `http://localhost:8085` | API Spring Boot |
| **Base de données** | `localhost:5432` | PostgreSQL (User: `postgres`, Pass: `root`, DB: `smart-house`) |

## 📂 Structure du Projet

-   `Smart_Home_back/` : Code source du backend Spring Boot.
-   `smartHome-front/` : Code source du frontend Angular.
-   `docker-compose.yml` : Configuration des services Docker.
