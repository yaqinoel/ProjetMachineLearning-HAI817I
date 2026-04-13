# ProjetMachineLearning-HAI817I

# Guide de Démarrage Rapide

Ce document explique comment configurer l'environnement et exécuter ce projet sur différents systèmes d'exploitation.

## 1. Créer un environnement virtuel

Ouvrez un terminal à la racine du projet et exécutez la commande correspondante à votre système d'exploitation :

**Windows :**
```bash
python -m venv ml_venv
.\ml_venv\Scripts\activate
```

**macOS / Linux :**
```bash
python3 -m venv ml_venv
source ml_venv/bin/activate
```

## 2. Installer les dépendances

Une fois l'environnement activé (vous devriez voir `(ml_venv)` au début de votre ligne de commande), exécutez les commandes suivantes pour installer les bibliothèques requises :

```bash
# Installer les dépendances du projet
pip install -r requirements.txt

# Note : En cas d'erreur lors de l'installation, essayez de mettre à jour pip d'abord, puis réessayez :
# python -m pip install --upgrade pip

# Installer l'outil de noyau pour exécuter les Jupyter Notebooks
pip install ipykernel
```

## 3. Utiliser Jupyter (.ipynb) dans VS Code

1. **Installer les extensions** : Assurez-vous que les extensions **Python** et **Jupyter** sont installées dans VS Code.
2. **Ouvrir le fichier** : Ouvrez votre fichier `.ipynb` dans le projet.
3. **Sélectionner le noyau (Kernel)** :
   - Cliquez sur **Select Kernel** dans le coin supérieur droit de l'éditeur.
   - Choisissez **Python Environments...**.
   - Sélectionnez l'interpréteur Python situé dans votre projet actuel : `./ml_venv/bin/python` (ou `Scripts\python.exe`).

## 4. Gestion des dépendances

Si vous installez de nouveaux paquets pendant le développement, n'oubliez pas de mettre à jour la liste des dépendances :
```bash
pip freeze > requirements.txt
```

---

> **Remarque** : Ne commitez jamais le dossier `ml_venv/` sur Git.
