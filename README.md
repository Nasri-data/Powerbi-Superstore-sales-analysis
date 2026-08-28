# 📊 Analyse des Ventes et de la Rentabilité — Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-Analyse%20de%20données-yellow)
![DAX](https://img.shields.io/badge/DAX-Modélisation-blue)
![Power Query](https://img.shields.io/badge/Power%20Query-ETL-green)
![Business Intelligence](https://img.shields.io/badge/Business%20Intelligence-Analytics-orange)

---

## 📌 Présentation du projet

Ce projet consiste à développer une solution de Business Intelligence avec **Microsoft Power BI Desktop** afin d'analyser les performances commerciales d'une entreprise de distribution.

L'objectif est de transformer des données transactionnelles brutes en **indicateurs de performance, analyses interactives et recommandations métier** permettant d'améliorer la prise de décision.

Le projet couvre notamment :

- l'analyse du chiffre d'affaires ;
- l'analyse de la rentabilité ;
- l'analyse des clients ;
- l'analyse des produits ;
- l'analyse géographique ;
- l'analyse des remises ;
- l'analyse des commandes ;
- le suivi des indicateurs clés de performance (KPI).

---

# 🎯 Objectifs métier

L'objectif principal est de permettre aux décideurs de comprendre rapidement les performances commerciales et d'identifier les leviers d'amélioration.

### 📈 Analyse des ventes

- Quel est le chiffre d'affaires total ?
- Comment évoluent les ventes dans le temps ?
- Quelles catégories génèrent le plus de chiffre d'affaires ?
- Quels sont les produits les plus vendus ?
- Quelles régions génèrent le plus de ventes ?

### 💰 Analyse de la rentabilité

- Quel est le bénéfice total ?
- Quelle est la marge bénéficiaire ?
- Quelles catégories sont les plus rentables ?
- Quels produits génèrent des pertes ?
- Quelles régions sont les plus rentables ?

### 👥 Analyse des clients

- Quels sont les clients générant le plus de chiffre d'affaires ?
- Quels segments de clientèle sont les plus performants ?
- Quels clients contribuent le plus au bénéfice ?

### 🏷️ Analyse des remises

- Quel est l'impact des remises sur la rentabilité ?
- Les remises importantes réduisent-elles la marge ?
- Quels produits sont fortement remisés ?

### 🚚 Analyse opérationnelle

- Quels modes de livraison sont les plus utilisés ?
- Quels modes de livraison génèrent le plus de ventes ?
- Quels modes de livraison sont les plus rentables ?

---

# 🗂️ Données utilisées

Le projet utilise le jeu de données **Superstore**, contenant des informations transactionnelles relatives aux commandes, clients, produits, régions, ventes, quantités, remises et bénéfices.

## Principales variables

| Variable | Description |
|---|---|
| Row ID | Identifiant unique de la ligne |
| Order ID | Identifiant de la commande |
| Order Date | Date de commande |
| Ship Date | Date d'expédition |
| Ship Mode | Mode de livraison |
| Customer ID | Identifiant du client |
| Customer Name | Nom du client |
| Segment | Segment du client |
| Country | Pays |
| City | Ville |
| State | État |
| Region | Région |
| Category | Catégorie du produit |
| Sub-Category | Sous-catégorie |
| Product Name | Nom du produit |
| Sales | Chiffre d'affaires |
| Quantity | Quantité vendue |
| Discount | Remise appliquée |
| Profit | Bénéfice |

---

# 🧹 Préparation et nettoyage des données

La préparation des données a été réalisée avec **Power Query** dans Power BI Desktop.

L'objectif était d'obtenir des données propres, cohérentes et adaptées à l'analyse.

## Principales transformations

### Vérification des types de données

Les types de données ont été vérifiés et corrigés.

Exemples :

- Order Date → Date
- Ship Date → Date
- Sales → Nombre décimal
- Profit → Nombre décimal
- Quantity → Nombre entier
- Discount → Nombre décimal

### Contrôles de qualité

Plusieurs contrôles ont été réalisés :

- recherche des valeurs manquantes ;
- recherche des doublons ;
- vérification des types de données ;
- contrôle des valeurs incohérentes ;
- vérification de la qualité des données.

### Standardisation des colonnes

Les noms des colonnes ont été standardisés afin de faciliter la modélisation et la création des mesures DAX.

Exemples :

```text
Order ID       → Order_ID
Customer ID    → Customer_ID
Customer Name  → Customer_Name
Order Date     → Order_Date
Ship Date      → Ship_Date
Product Name   → Product_Name
Sub-Category   → Sub_Category
