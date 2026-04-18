# 🛒 Segmentation Client RFM - Online Retail

## 📌 Présentation du Projet
L'objectif de ce projet est de segmenter la base clients d'une entreprise de retail en utilisant la méthode **RFM (Récence, Fréquence, Montant)**. Cette analyse permet de comprendre le comportement d'achat et de définir des stratégies marketing ciblées pour augmenter la rétention et le chiffre d'affaires.

## 🛠️ Technologies Utilisées
* **Python 3.12**
* **Pandas** : Nettoyage et manipulation des données.
* **Matplotlib & Seaborn** : Visualisation des segments.
* **Datetime** : Gestion des périodes de récence.

## 📊 Méthodologie
1. **Nettoyage des données** : 
   - Suppression des `CustomerID` manquants.
   - Filtrage des transactions annulées (codes commençant par 'C').
   - Élimination des quantités et prix négatifs.
2. **Calcul des métriques RFM** :
   - **Récence** : Nombre de jours depuis le dernier achat.
   - **Fréquence** : Nombre total de transactions uniques.
   - **Montant** : Chiffre d'affaires total généré par client.
3. **Scoring** : Attribution d'une note de 1 à 5 pour chaque métrique en utilisant les quintiles.
4. **Segmentation** : Mapping des scores RF en 10 segments (Champions, Loyal Customers, At Risk, Hibernating, etc.).

## 📈 Résultats Clés
* **Segments Dominants** : [Indique ici le segment le plus nombreux, ex: Hibernating].
* **Impact Business** : Le segment des **Champions** représente [X]% du chiffre d'affaires total, soulignant l'importance de la fidélisation.
* **Alerte** : [X]% des clients sont classés "At Risk", nécessitant une campagne de réactivation immédiate.

## 🚀 Comment utiliser ce repo
1. Cloner le projet.
2. Installer les dépendances : `pip install pandas matplotlib seaborn`.
3. Lancer le notebook `segmentation_rfm.ipynb`.
