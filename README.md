# 🏄 Taghazout — Plateforme Touristique Intégrée

> Plateforme web complète de gestion touristique dédiée à la destination **Taghazout**, Maroc — développée dans le cadre du projet de fin d'études (Soutenance 103).

---

## 📌 Description du Projet

**Taghazout** est une application web full-stack qui centralise l'ensemble des services touristiques de la ville de Taghazout en une seule plateforme. Elle permet aux visiteurs de réserver des hôtels, restaurants et activités, de suivre des cours de surf, de payer en ligne et de communiquer en temps réel.

---

## ✨ Fonctionnalités Principales

### 👤 Côté Utilisateur
- 🔐 Authentification sécurisée (JWT + bcryptjs)
- 🏨 Réservation d'hôtels, restaurants et activités
- 🏄 Inscription aux cours de surf
- 💳 Paiement en ligne via **Stripe**
- 💬 Chat en temps réel
- 🗺️ Carte interactive (Leaflet.js)
- ⭐ Système d'avis et de reviews
- 🌍 Support multilingue (dossier `lang/`)
- 🎖️ Programme de fidélité (Loyalty)

### 🛠️ Côté Administrateur
- Dashboard complet (admin panel)
- Gestion des hôtels, restaurants, activités et cours de surf
- Gestion des réservations et paiements
- Gestion des utilisateurs et messages
- Génération de rapports PDF (fpdf)
- Statistiques avec Chart.js

---

## 🧰 Technologies Utilisées

### Backend
| Technologie | Usage |
|---|---|
| **PHP** | Logique serveur principale |
| **Node.js / Express** | API REST & serveur temps réel |
| **MongoDB / Mongoose** | Base de données NoSQL |
| **JWT** | Authentification sécurisée |
| **bcryptjs** | Hachage des mots de passe |
| **Multer** | Upload de fichiers |
| **dotenv** | Gestion des variables d'environnement |

### Frontend
| Technologie | Usage |
|---|---|
| **HTML / CSS / JavaScript** | Interface utilisateur |
| **GSAP** | Animations avancées |
| **AOS** | Animations au scroll |
| **Leaflet.js** | Carte interactive |
| **Chart.js** | Tableaux de bord statistiques |

### Paiement & Stockage
| Technologie | Usage |
|---|---|
| **Stripe** | Paiement en ligne sécurisé |
| **FPDF** | Génération de factures PDF |

---

## 📁 Structure du Projet

```
soutenance-103/
├── admin/              # Panel d'administration
│   ├── hotels/
│   ├── restaurants/
│   ├── activities/
│   ├── bookings/
│   ├── payments/
│   ├── surf-courses/
│   ├── loyalty/
│   ├── users/
│   └── reviews/
├── api/                # API REST (Node.js/Express)
├── auth/               # Authentification (login, register, JWT)
├── booking/            # Module de réservation
├── chat/               # Chat en temps réel
├── map/                # Carte interactive (Leaflet)
├── payment/            # Intégration Stripe
├── profile/            # Gestion du profil utilisateur
├── database/           # Configuration & connexion DB
├── lang/               # Fichiers de traduction
├── includes/           # Composants PHP partagés
├── assets/
│   ├── css/
│   ├── js/
│   ├── images/         # (hotels, surf, restaurants, gallery...)
│   ├── videos/
│   └── libraries/      # AOS, GSAP, Chart.js, Leaflet, Stripe
├── uploads/            # Fichiers uploadés par les utilisateurs
└── vendor/             # Dépendances PHP (Stripe SDK)
```

---

## ⚙️ Installation & Configuration

### Prérequis
- PHP >= 7.4
- Node.js >= 16
- MongoDB
- Compte Stripe (pour les paiements)

### Étapes d'installation

```bash
# 1. Cloner le dépôt
git clone https://github.com/zakariyaaaaaa/soutenance-103-.git
cd soutenance-103-

# 2. Installer les dépendances Node.js
npm install

# 3. Configurer les variables d'environnement
cp .env.example .env
# Éditer .env avec vos clés (MongoDB URI, Stripe keys, JWT secret)

# 4. Lancer le serveur Node.js
node server.js

# 5. Lancer le serveur PHP (XAMPP / WAMP ou PHP built-in)
php -S localhost:8000
```

### Variables d'environnement (.env)
```env
MONGODB_URI=mongodb://localhost:27017/taghazout
JWT_SECRET=your_jwt_secret_key
STRIPE_SECRET_KEY=sk_test_...
STRIPE_PUBLIC_KEY=pk_test_...
PORT=3000
```

---

## 🖼️ Aperçu des Pages

| Page | Description |
|---|---|
| `/` | Page d'accueil avec animations |
| `/booking/` | Réservation d'hôtels et activités |
| `/map/` | Carte interactive de Taghazout |
| `/chat/` | Messagerie en temps réel |
| `/profile/` | Espace utilisateur |
| `/admin/` | Tableau de bord administrateur |

---

## 👨‍💻 Auteur

**Zakaria Boutlane**  
Projet de Fin d'Études — Soutenance 103

---

## 📄 Licence

Ce projet est réalisé dans un cadre académique. Tous droits réservés © 2024 Zakaria Boutlane.
