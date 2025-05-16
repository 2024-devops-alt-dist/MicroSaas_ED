# 🧾 TikTakFacture

> 🕒 TikTakFacture, c’est l’allié des indépendants pressés.  
> Créez et envoyez vos factures avant même que le café ne refroidisse ☕

---

![TikTakFacture banner](https://img.shields.io/badge/MicroSaaS-Devis%20%2F%20Factures-blue?style=for-the-badge)

---

## 🚀 Présentation du service

![🚀](https://img.shields.io/badge/Objectif-Autonomiser%20les%20ind%C3%A9pendants-informational?style=flat-square)

TikTakFacture est une application **Micro-SaaS** dédiée aux indépendants, freelances et TPE qui souhaitent créer rapidement des **devis** et **factures professionnelles**, sans complexité.

### 🧠 Objectif

Faciliter la gestion administrative des petites entreprises avec une interface intuitive, rapide et accessible depuis n'importe où.

---

## 🎨 Charte graphique

**Palette de couleurs** :

- 🔷 **Bleu pétrole** : `#007C91`
- ⚪ **Gris clair** : `#F5F5F5`
- ⚪ **Blanc** : `#FFFFFF`
- ⚫ **Noir doux** : `#333333`

✒️ **Typographies** :
- Titres : `Poppins`, `Montserrat`
- Texte : `Roboto`, `Open Sans`

🖼️ **Style** :
- Illustrations minimalistes, icônes vectorielles, ambiance moderne et épurée

---

## 📌 Expression des besoins

### 🎯 Problème identifié

Les indépendants et petites structures perdent un temps précieux à gérer manuellement leurs devis et factures avec des outils inadaptés (Word, Excel).

### 👤 Public cible

- Indépendants, freelances
- Artisans, graphistes, développeurs, consultants

### 🧩 Fonctionnalité principale

- Création rapide de **devis** et **factures** professionnelles, avec téléchargement PDF ou envoi par email

### 🧱 Fonctionnalités secondaires

- Gestion des **clients**
- Suivi des **paiements**
- Tableau de bord simplifié

---

## ✏️ Wireframes & Zoning

🗂️ Aperçu rapide des interfaces proposées :
- **Dashboard** avec sidebar, résumé des factures et derniers documents
- **Formulaire de création de devis** avec champs : client, date, description, montant
- **Liste des devis** sous forme de tableau filtrable

📎 Voir `/wireframes` ou dans la présentation Canva pour les visuels associés.

---

## 🛠️ Stack technique

| Layer               | Technologie | Logo                                                                                                     |
|---------------------|-------------|----------------------------------------------------------------------------------------------------------|
| **Frontend**        | Angular     | ![Angular](https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white) |
| **Backend**         | Symfony     | ![Symfony](https://img.shields.io/badge/Symfony-000000?style=for-the-badge&logo=symfony&logoColor=white) |
| **Base de données** | MySQL       | ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)       |


---

## 🔄 Diagramme de cas d'utilisation

Diagramme réalisé avec PlantUML :

![Diagramme de cas d'utilisation](./Diagramme/Diagramme_Cas_Utilisation.png)

- Gérer clients
- Gérer devis
- Gérer factures
- Se connecter

---

## 🗃️ MCD (Modèle Conceptuel de Données)

### Entités principales :

- **Client** : id, name, siret, adresse, code_postale, telephone, mail, isProfessionnel, createdAt, updatedAt
- **Devis** : id, numero_devis, date, client_id, montant_total, montant_ht, tva, montant_facture, montant_restant, active, service_id, createdAt, updatedAt
- **Facture** : id, numero_facture, date, devis_id, client_id, statut, montant, montant_ht, montant_paye, montant_restant, tva, createdAt, updatedAt
- **Service/Produits** : id, description, prix_unitaire, createdAt, updatedAt
- **User** : id, login, password
![MCD](./Merise/MLD.png)