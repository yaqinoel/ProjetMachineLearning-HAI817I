# Projet Machine Learning - TODO List

## 1. Refactorisation & Prétraitement
- [ ] **Refactorisation de la structure du code**
- [ ] **Éviter la répétition du prétraitement** : Centraliser le pipeline de nettoyage des données pour qu'il ne soit exécuté qu'une seule fois.

## 2. Modélisation & Optimisation
- [ ] **Optimisation des hyperparamètres** : Utiliser **Optuna** pour trouver les meilleurs paramètres des modèles. **@Sab**
- [ ] **Réduction de dimensionnalité** : Appliquer une **ACP** (Analyse en Composantes Principales). **@Léo**
- [ ] **Mise à jour des métriques d'évaluation** : Ne pas se limiter à l'accuracy. Intégrer le **Rappel (Recall)**, la **Précision**, le **F1-score**, etc.

## 3. Visualisation & Analyse
- [ ] **Visualisation générale** : Gérer les graphiques et l'esthétique globale du notebook. **@Yaqi**
- [ ] **Boxplots des modèles** : Créer un graphe en boîte (box plot) dédié pour chaque modèle. **@Lei**
- [ ] **Comparaison des tâches** : Créer un histogramme pour comparer les différentes tâches/classes. **@Yagmur**
- [ ] **Analyse de l'impact des Stop Words** : 
    - [ ] Tracer les courbes de performances pour chaque modèle avec **ET** sans stop words.
    - [ ] Analyser et rédiger une conclusion : quel modèle est le plus performant dans chaque cas et pourquoi.
- [ ] **Affichage des résultats finaux** : Dans la dernière partie, afficher le **rang (rank)** des modèles au lieu du pourcentage classique pour l'Accuracy et le F1-score.