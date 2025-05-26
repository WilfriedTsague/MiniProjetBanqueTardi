# 💳 MiniProjetBankTardi

**MiniProjetBankTardi** est une application de gestion bancaire développée dans un but pédagogique avec une architecture moderne en **.NET Core (API)** et **Angular (Front-end)**. Elle permet de simuler la gestion de clients, de comptes bancaires (chèque, épargne), les opérations financières, ainsi que le traitement des découverts et des intérêts.

---

## 🚀 Fonctionnalités

- 🔐 Gestion des clients (ajout, modification, suppression)
- 🏦 Création de comptes bancaires avec :
  - Numérotation automatique (type + incrément)
  - Affectation à un client
- 💳 Types de comptes : Chèque, Épargne (avec taux d'intérêt et découvert)
- 💸 Opérations bancaires : dépôts, retraits, découverts
- 📈 Calcul automatique des intérêts
- ⚠ Gestion des découverts avec pénalité (opération « Découvert »)
- 📂 Affichage des comptes et opérations par client

---

## 🛠️ Technologies utilisées

### Back-end : .NET Core
- ASP.NET Core Web API
- Entity Framework Core
- Architecture en couches : Controller / Service / Repository
- SQL Server

### Front-end : Angular
- Angular CLI
- HttpClient pour consommation d'API
- Bootstrap pour le design
- Reactive Forms

---

## ⚙️ Installation et exécution

### Prérequis
- [.NET SDK](https://dotnet.microsoft.com/download)
- [Node.js + Angular CLI](https://angular.io/cli)
- [SQL Server](https://www.microsoft.com/en-us/sql-server/)

### Étapes

#### 1. Base de données
- Créez la base dans SQL Server
- Modifiez la chaîne de connexion dans `appsettings.json`
- Exécutez les migrations :
```bash
dotnet ef database update
