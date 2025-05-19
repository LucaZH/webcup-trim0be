# 🖤 TheEnd.page

![TheEnd.page Logo](https://via.placeholder.com/150x50.png?text=☠️+TheEnd.page)  

## 🚀 **Description de notre Site web**

**TheEnd.page** est une expérience web unique qui transforme les fins en œuvres numériques. Notre plateforme propose :

1. **Un accueil visuel immersif** avec interface intuitive
2. **Deux modes d'entrée** :
   - Sélection directe d'émotion
   - Dialogue avec notre bot émotionnel (humour ou bienveillance au choix)
3. **Un studio créatif** pour personnaliser sa page de fin


## 🛠️ **Technologies utilisées**

- ### **Backend** 
Django Rest Framework

- ### **Frontend**  
React JS , Typescript, Tailwind CSS

- ### **Design**  
Figma

- ### **Database**  
MySQL


## 📋 **Prérequis**

- 🐍 **Python 3.10+**  
- ⚛️ **Node.js 18+**
- 🐬 **MySQL 8.0+**  
- 🧩 **Pipenv** (Gestion des dépendances Python)


## 🛠️ **Installation en local**

### 1. Clone le repo
```bash
git clone --recurse-submodules https://github.com/LucaZH/webcup-trim0be.git
cd ./webcup-trim0be
```

### 2. Configuration du Backend (Django)
**Installation les dépendances**
```bash
cd ./webcup2025-backend 
pipenv install
pip install -r requirements.txt
```

**Configuration :**
- Crée un fichier `.env` :
```ini
SECRET_KEY=votre_cle_secrete_django_ici

DEBUG=False

DB_NAME=nom_de_votre_base_de_donnees
DB_USER=utilisateur_mysql
DB_PASSWORD=theendpage
DB_HOST=localhost
DB_PORT=3306

EMAIL_HOST_USER=votre_email@gmail.com
EMAIL_HOST_PASSWORD=mot_de_passe_ou_mot_de_passe_application

HOST=http://localhost:3000/
BACKEND_HOST=http://localhost:8000/api/

GOOGLE_OAUTH_CLIENT_ID=identifiant_client_google
GOOGLE_OAUTH_CLIENT_SECRET=secret_client_google
GOOGLE_OAUTH_CALLBACK_URL=http://localhost:8000/auth/callback/

```

**Base de données :**
```sql
CREATE DATABASE theendpage;
```

```bash
pipenv run python manage.py migrate 
pipenv run python manage.py createsuperuser 
```

**Lancer l'application :**
```sql
pipenv run python manage.py runserver 
```

### 3. Frontend (React)
**Installation les dépendances**
```bash
cd ./webcup2025.front
npm install
```

**Lancer l'application :**
```bash
npm run dev
```
