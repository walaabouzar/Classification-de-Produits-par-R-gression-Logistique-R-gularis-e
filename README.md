# Classification-de-Produits-par-R-gression-Logistique-R-gularisé
# 📊  Régression Logistique avec Régularisation

## 🔍 Objectif

Mettre en œuvre une **régression logistique régularisée** afin de résoudre un problème de **classification binaire**. L’algorithme est entraîné pour prédire si un produit sera commercialisé ou non, à partir des résultats de deux tests de qualité.

## 🗂️ Contenu des données

Le fichier `data.csv` contient **118 exemples** avec les colonnes suivantes :

1. Test 1 : Résultat du premier test de qualité
2. Test 2 : Résultat du second test de qualité
3. Commercialisation : Valeur cible `y` (1 = commercialisé, 0 = non commercialisé)

---

## ⚙️ Étapes principales

### 1. 📥 Chargement et préparation des données
- Lecture du fichier CSV
- Construction de la matrice des caractéristiques `X` avec ajout du biais (x₀ = 1)
- Construction du vecteur `y`

### 2. 🔄 Mapping polynomial
- Transformation des caractéristiques en une forme polynomiale de degré 6
- Génération de 28 nouvelles features

### 3. 🧮 Implémentation de la régression logistique
- Fonction `Sigmoid(z)`
- Fonction de coût régularisée `computeCostReg`
- Implémentation de `gradientDescent` avec régularisation

### 4. 📉 Entraînement du modèle
- Initialisation de `theta`
- Entraînement avec descente du gradient
- Visualisation de la fonction de coût au fil des itérations

### 5. 🧪 Prédiction & Évaluation
- Prédiction à l’aide d’un seuil (sigmoid > 0.5)
- Calcul de la **précision du classifieur**
- Affichage de la frontière de décision

### 6. 🔍 Vérification
- Comparaison possible avec la régression logistique de **scikit-learn**

---

## 📈 Résultats attendus

- Une courbe de coût qui diminue progressivement.
- Une frontière de décision non linéaire bien ajustée aux données.
- Une précision élevée sur les données d’entraînement.

---

## 🧠 Pour aller plus loin

- Tester d'autres degrés de polynômes
- Essayer différentes valeurs de régularisation `λ`
- Implémenter la classification avec **Scikit-Learn** pour comparer
- Ajouter une métrique F1-score ou matrice de confusion

---

## 📎 Fichiers inclus

- `data.csv` : Données d’apprentissage
- `reg_log_reg.py` : Implémentation de la régression logistique
- `README.md` : Fichier de documentation

---


