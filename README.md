Description
SQL SRS est une application interactive développée avec Streamlit et DuckDB pour pratiquer et réviser les requêtes SQL de manière efficace.

L’application permet de :

sélectionner un thème SQL (e.g., GROUP BY, JOIN, WINDOW FUNCTIONS)

s’exercer sur des questions réelles

vérifier automatiquement les réponses des utilisateurs

suivre la progression avec un système de répétition espacée, pour revoir les exercices les moins récents

L’objectif est d’offrir un outil d’apprentissage pratique pour renforcer ses compétences en SQL et data manipulation.

Fonctionnalités principales
✅ Sélection automatique d’un exercice si aucun thème n’est choisi

✅ Vérification instantanée des réponses SQL avec affichage des différences

✅ Indication “Correct !” lorsque la réponse correspond à la solution

✅ Système de répétition espacée pour réviser les exercices moins récemment vus

✅ Reset du suivi des exercices via un bouton Reset

✅ Listing dynamique des thèmes disponibles à partir de la base de données

Tech Stack
Python 3.12

Streamlit pour l’interface utilisateur

DuckDB pour le stockage et l’exécution des requêtes SQL

Gestion des dépendances avec venv

Logging et gestion des erreurs pour une UX robuste

Comment utiliser
Cloner le projet :
git clone <URL_DU_PROJET> cd sql_srs

Installer les dépendances :
python -m venv venv source venv/bin/activate # sur Linux/Mac venv\Scripts\activate # sur Windows pip install -r requirements.txt

Lancer l’application :
streamlit run app.py

Sélectionner un thème dans la sidebar et commencer à réviser !

Cliquer sur Reset pour réinitialiser les dates des exercices et recommencer le suivi.

Organisation du projet
sql_srs/ ├─ app.py # Application principale Streamlit ├─ init_db.py # Script d'initialisation de la base de données ├─ data/ # Base de données DuckDB ├─ answers/ # Fichiers SQL des réponses ├─ requirements.txt └─ README.md

Extensions possibles
Ajouter de nouveaux exercices et thèmes SQL

Améliorer l’UI pour plus d’interactivité et de lisibilité

Implémenter un système multi-utilisateurs avec login

Formatter automatiquement les requêtes SQL pour plus de lisibilité

Ajouter un suivi graphique des progrès
