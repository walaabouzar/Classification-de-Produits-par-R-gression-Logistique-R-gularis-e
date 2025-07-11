# 📊 Régression Logistique avec Régularisation

## 🎯 Objectif

Ce projet implémente un modèle de **régression logistique régularisée** pour résoudre un problème de **classification binaire**. L’objectif est de prédire la **commercialisation d’un produit** en fonction de deux tests de qualité (`Test 1` et `Test 2`).

---

## 📁 Contenu

- `data.csv` : Jeu de données contenant 118 échantillons :
  - Colonne 1 : Score du Test 1
  - Colonne 2 : Score du Test 2
  - Colonne 3 : Commercialisation (1 = Oui, 0 = Non)
- `regularisation.ipynb` : Notebook Python contenant l’implémentation complète.

---

## 🧱 Étapes principales

### 1. 🔄 Prétraitement
- Chargement des données
- Ajout d’une colonne de biais
- Séparation des variables explicatives `X` et de la cible `y`

### 2. 🧮 Transformation polynomiale
- Expansion des variables `X1` et `X2` jusqu’au **degré 6**
- Génération de **28 caractéristiques** à partir des combinaisons polynomiales

### 3. 📉 Régression logistique
- Fonction `Sigmoid`
- Fonction de coût avec **régularisation L2**
- Implémentation de la **descente du gradient**

### 4. 📈 Visualisation
- Courbe de convergence du coût
- Visualisation de la **frontière de décision**
- Tracé 3D de la surface du coût

### 5. 🔍 Prédiction
- Fonction de prédiction binaire
- Calcul de la **précision**
- Comparaison des performances avec **Scikit-Learn**

---

## ✅ Résultats

- Précision du modèle implémenté manuellement : **~83%**
- Précision du modèle `LogisticRegression` de `scikit-learn` : **~83%**
- Meilleur coût atteint ≈ **0.38** après 20 000 itérations avec `lambda=0.01` et `alpha=0.01`

---

## 📚 Renforcement de l’apprentissage

Le projet comprend :
- Un découpage en **train / validation / test**
- Une **courbe d’apprentissage**
- Des visualisations supplémentaires pour mieux comprendre le comportement du modèle

---

## 🔧 Librairies utilisées

- `NumPy`
- `Matplotlib`
- `Scikit-learn`
- `SciPy`
- `Pandas`

---

## 📌 Remarques

- La régularisation permet d’éviter le **surapprentissage** dû à l’augmentation du nombre de caractéristiques.
- L’évaluation a été réalisée à l’aide de **précision** et de la **fonction de coût régularisée**.

---

