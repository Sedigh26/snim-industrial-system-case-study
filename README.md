# snim-industrial-system-case-study
A technical case study of a software solution developed for SNIM to optimize industrial operations.
# SNIM - Portail de Formation & Recrutement

Ce projet est une plateforme professionnelle dédiée à la gestion des formations et du recrutement pour la **SNIM (Société Nationale Industrielle et Minière)**.

## 🚀 Fonctionnalités Clés

### 1. Administration Multi-Pages (Totalement Centralisée)

Le portail RH est désormais divisé en modules professionnels via une architecture de données centralisée :

- **Tableau de Bord** : Vue d'ensemble des statistiques et tendances.
- **Gestion des Candidatures** : Suivi complet du pipeline de recrutement.
- **Processus de Sélection** : Gestion des entretiens et évaluations.
- **Suivi des Formations** : Gestion des cohortes et de l'assiduité.
- **Paramètres Système** : Contrôle global et gestion du personnel RH.

### 2. Architecture Prête pour le Backend (100%)

Le projet utilise un "Service Layer" qui permet de basculer instantanément entre des données simulées (Mock) et un backend réel.

- **`js/config.js`** : Point de contrôle unique pour l'URL de l'API et le mode (Mock/Real).
- **`js/admin-data.js`** : Service API centralisé gérant toutes les requêtes (Candidats, Stats, Inscriptions, Suivi).
- **`js/store.js`** : Gestion centralisée de l'état (Single Source of Truth).

## 🛠️ Stack Technique

- **Core** : Vanilla JavaScript (ES Modules), HTML5, CSS3.
- **UI Framework** : Bootstrap 5 + Bootstrap Icons + Chart.js.
- **Qualité & Tests** : Intégration de **Vitest** pour les tests unitaires du service API.
- **Dev Tooling** : Vite (HMR) pour un développement fluide.

## 🏁 Configuration du Backend

Pour connecter votre propre backend :

1. Ouvrez `js/config.js`.
2. Modifiez `API_BASE_URL` avec votre adresse serveur.
3. Réglez `USE_MOCK_DATA: false`.

## 📂 Organisation du Code

- `js/admin-data.js` : Moteur de données (API Hub) centralisé.
- `js/config.js` : Configuration globale et endpoints.
- `js/store.js` : Magasin de données global.
- `js/admin-ui.js` : Bibliothèques de rendu UI (Tables, Stats, Modals).
- `js/components/` : Composants dynamiques (AdminSidebar, etc.).

## 🧪 Tests

Exécutez la commande suivante pour vérifier l'intégrité du service API :

```bash
npm test
```

---

_Projet développé pour la SNIM - Excellence en Formation & Recrutement Minier._
