<<<<<<< HEAD
# Système de Suivi de Colis

Ce projet est une application de suivi de colis complète avec un frontend Angular, un backend FastAPI et une base de données PostgreSQL.

## Structure du Projet

```
project/
├── frontend/          # Application Angular
│   └── src/
│       ├── app/
│       │   ├── pages/
│       │   │   ├── profile/
│       │   │   ├── help/
│       │   │   ├── home/
│       │   │   ├── advanced-shipment-tracking/
│       │   │   └── tracking-page/
│       │   ├── services/
│       │   └── components/
│       └── styles/
└── backend/          # API FastAPI (à implémenter)
    ├── app/
    │   ├── models/      # Modèles SQLAlchemy
    │   ├── schemas/     # Schémas Pydantic
    │   ├── routes/      # Points d'API
    │   └── services/    # Logique métier
    ├── alembic/         # Migrations de base de données
    └── tests/           # Tests unitaires et d'intégration
```

## Fonctionnalités Principales

### Frontend (Existant)
- Page d'accueil avec recherche de colis
- Suivi avancé des expéditions
- Profil utilisateur
- Section d'aide avec FAQ
- Système de notifications

### Backend (À Implémenter)
- API RESTful avec FastAPI
- Base de données PostgreSQL
- Authentification JWT
- Gestion des utilisateurs
- Suivi des colis en temps réel
- Notifications en temps réel

## Configuration Technique

### Frontend
- Angular 17+
- SCSS pour les styles
- Composants standalone
- Services d'état

### Backend
- Python 3.9+
- FastAPI
- SQLAlchemy
- Alembic
- PostgreSQL
- JWT pour l'authentification

### Base de Données
- PostgreSQL 14+
- Migrations avec Alembic

## Installation

### Prérequis
- Node.js 18+
- Python 3.9+
- PostgreSQL 14+
- Poetry (gestionnaire de paquets Python)

### Frontend
```bash
cd frontend
npm install
ng serve
```

### Backend (À implémenter)
```bash
cd backend
poetry install
poetry run uvicorn app.main:app --reload
```

### Base de données
```bash
# Créer la base de données
createdb shipment_tracking

# Appliquer les migrations
poetry run alembic upgrade head
```

## Variables d'Environnement

### Backend
```env
DATABASE_URL=postgresql://user:password@localhost:5432/shipment_tracking
SECRET_KEY=your_secret_key
ALGORITHM=HS256
ACCESS_TOKEN_EXPIRE_MINUTES=30
```

## Tests

### Backend
```bash
poetry run pytest
```

### Frontend
```bash
ng test
```

## Déploiement

- Frontend : Nginx
- Backend : Gunicorn + Uvicorn
- Base de données : PostgreSQL sur serveur dédié
- Cache : Redis (optionnel) 
=======
# nouveauDossier
>>>>>>> c09eb21a91da72cf01007b1f6bdadde5fb4382e7
