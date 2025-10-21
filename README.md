# 🌿 EcoRide – Application de covoiturage écoresponsable

**EcoRide** est une application web de covoiturage qui vise à réduire l’impact environnemental des déplacements en favorisant les trajets partagés entre particuliers.  
Ce projet a été réalisé dans le cadre du **Titre Professionnel Développeur Web et Web Mobile (DWWM)**.

---

##  Objectifs du projet

- Concevoir une application web **complète, moderne et sécurisée**.  
- Gérer deux types de bases de données : **relationnelle (MySQL)** et **non relationnelle (MongoDB)**.  
- Appliquer une démarche **Security by Design**, intégrant la sécurité tout au long du développement.  
- Démontrer la maîtrise du **back-end Node.js / Express.js** et du **front-end Angular**.  

---

##  Stack technique

- **Front-end :** Angular 17 (SPA responsive)  
- **Back-end :** Node.js + Express.js  
- **Base SQL :** MySQL 8.0 (tables utilisateurs, trajets, réservations, paiements)  
- **Base NoSQL :** MongoDB 8.2.1 (statistiques journalières et logs)  
- **Outils :** MySQL Workbench, MongoDB Compass, Figma, Trello  
- **Sécurité :** bcrypt, JWT, dotenv, CORS, validation front/back, mini-SIEM  
- **Environnement :** Visual Studio Code, Git, GitHub  

---

##  Installation du projet

### 1️⃣ Cloner le dépôt
```bash
git clone https://github.com/peaky013/EcoRide.git
cd EcoRide

2️⃣ Installer les dépendances
bash
npm install


3️⃣ Créer le fichier .env
Crée un fichier .env à la racine du dossier backend :
env
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=
DB_NAME=ecoride
MONGO_URI=mongodb://localhost:27017/ecoride_nosql
JWT_SECRET=secret_key
PORT=3000

4️⃣ Importer la base SQL
Dans MySQL Workbench :
SOURCE ./sql/ecoride_schema.sql;


5️⃣ Importer la base NoSQL
Dans MongoDB Compass :
Importer le fichier nosql/ecoride_nosql.stats.json dans la collection stats.


6️⃣ Lancer le serveur
npm start
Le serveur démarre sur http://localhost:3000


🔐 Sécurité intégrée
Mots de passe hachés avec bcrypt

Authentification via JWT

Requêtes SQL paramétrées (anti-injection)

Validation front-end et back-end

Journalisation des actions utilisateurs (logs MongoDB)

Mini SIEM pour la détection d’anomalies

Approche Security by Design (sécurité intégrée dès le développement)

📁 Structure du projet
DWWM_EcoRide/
│
├── backend/
│   ├── server.js
│   ├── routes/
│   ├── models/
│   └── config/
│
├── sql/
│   ├── ecoride_schema.sql
│   └── ecoride_schema.model.mwb
│
├── nosql/
│   ├── ecoride_nosql.stats.json
│   ├── mongodb_ecoride_stats.png
│   └── siem_monitor.js
│
├── maquettes_figma/
│   ├── maquette_accueil.png
│   ├── maquette_recherche.png
│   └── maquette_profil.png
│
└── README.md
👨‍💻 Auteur
Medjadi Mohamed
Étudiant DWWM – Studi / Ministère du Travail
Passionné par le développement web et la cybersécurité
🔗 Portfolio | LinkedIn

🧠 Licence
Projet réalisé à des fins pédagogiques dans le cadre du Titre Professionnel DWWM.
