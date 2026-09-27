

# Roadmap Data Analyst — De la prépa MPI au métier de la Data

> Feuille de route personnelle et progressive pour un étudiant en classe préparatoire MPI souhaitant devenir Data Analyst, avec une trajectoire ouverte vers Data Scientist, Data Engineer ou BI Analyst.


## Sommaire

1. [Introduction](#1-introduction)
2. [Les métiers de la Data](#2-les-m%C3%A9tiers-de-la-data)
3. [Objectif : devenir Data Analyst](#3-objectif--devenir-data-analyst)
4. [Roadmap des compétences](#4-roadmap-des-comp%C3%A9tences)
5. [Ressources d'apprentissage](#5-ressources-dapprentissage)
6. [Exercices](#6-exercices)
7. [Projets](#7-projets)
8. [GitHub et portfolio](#8-github-et-portfolio)
9. [Roadmap temporelle](#9-roadmap-temporelle)
10. [Préparation aux études après la MPI](#10-pr%C3%A9paration-aux-%C3%A9tudes-apr%C3%A8s-la-mpi)
11. [Préparation au stage](#11-pr%C3%A9paration-au-stage)
12. [Checklist finale](#12-checklist-finale)
13. [Par où commencer aujourd'hui ?](#13-par-o%C3%B9-commencer-aujourdhui-)

---

## 1. Introduction

### Qu'est-ce que la Data ?

La Data désigne l'ensemble des données produites par une activité (ventes, logs applicatifs, capteurs, comportements utilisateurs, transactions financières, etc.) et exploitées pour comprendre une situation, détecter des tendances, ou orienter une décision. Le travail avec la donnée repose sur trois piliers : la **collecte** (aller chercher la donnée là où elle se trouve), la **transformation** (la nettoyer, la structurer) et l'**exploitation** (l'analyser, la visualiser, en tirer une conclusion actionnable).

### Qu'est-ce qu'un Data Analyst ?

Un Data Analyst transforme des données brutes en informations exploitables pour la prise de décision. Concrètement, il :

- interroge des bases de données (SQL) pour extraire l'information pertinente ;
- nettoie et structure des jeux de données souvent imparfaits ;
- applique des méthodes statistiques simples pour caractériser un phénomène (moyenne, dispersion, corrélation, test d'hypothèse) ;
- construit des visualisations et des tableaux de bord (dashboards) ;
- communique les résultats à des interlocuteurs non techniques (managers, équipes métier).

Contrairement au Data Scientist, le Data Analyst se concentre sur la compréhension du passé et du présent (« que s'est-il passé ? pourquoi ? ») plutôt que sur la prédiction du futur.

### Pourquoi un profil MPI est pertinent

La prépa MPI développe des compétences directement réutilisables dans la Data :

- **rigueur mathématique** : probabilités, algèbre linéaire, statistiques — le socle théorique de toute l'analyse de données ;
- **capacité d'abstraction et de modélisation** : essentielle pour formuler un problème métier en problème de données ;
- **logique algorithmique et bases de programmation** (Python, structures de données, complexité) héritées de l'informatique MPI ;
- **méthode de travail et rigueur de raisonnement**, utile pour ne pas tirer de conclusions hâtives d'un jeu de données.

### Ce qui manque et doit être acquis

La prépa ne couvre pas, ou très peu :

- les outils du métier (SQL, Pandas, Power BI, Git) ;
- la statistique appliquée et interprétative (au-delà du formalisme mathématique : p-value, intervalle de confiance, choix de test) ;
- la manipulation de données réelles, sales, incomplètes ;
- la communication de résultats à un public non technique ;
- la culture du monde de l'entreprise et de la donnée (dashboard, reporting, KPI).

Cette roadmap comble précisément cet écart.

### Note de contexte : étudier en MPI au Sénégal

Cette feuille de route est pensée pour un étudiant en MPI au Sénégal, et intègre à ce titre trois réalités locales :

- Les CPGE scientifiques sénégalaises (notamment celles hébergées à l'École Polytechnique de Thiès, EPT) suivent le programme français et préparent aux mêmes concours que les CPGE de France (Mines-Ponts, Mines-Télécom, CCINP, etc.), en plus de donner accès aux écoles d'ingénieurs sénégalaises. Le parcours décrit dans ce document reste donc valable qu'on prépare ces concours depuis le Sénégal, depuis une CPGE en France via une bourse d'excellence, ou dans le cadre d'un double objectif Sénégal/France.
- Le Sénégal dispose d'un écosystème data en plein développement (banques, télécoms, fintechs/scaleups à Dakar), avec des besoins réels en Data Analysts localement, en plus des opportunités à distance pour des entreprises étrangères.
- Les ressources listées ci-dessous sont toutes gratuites ou proposent une alternative gratuite crédible (aide financière, contenu en libre accès), et privilégient des formats légers en bande passante (cours interactifs textuels, documentation) en complément des vidéos, pour tenir compte de contraintes de connexion possibles.

---

## 2. Les métiers de la Data

Il n'existe pas de « meilleur » métier de la Data : chacun correspond à un type d'appétence et de mission différent. Le tableau ci-dessous présente les repères principaux, sans hiérarchie.

### Data Analyst

- **Rôle** : répondre à des questions métier à partir de données existantes.
- **Missions** : extraction SQL, nettoyage, analyse descriptive, création de dashboards, présentation de résultats.
- **Compétences clés** : SQL, statistiques descriptives, Excel, Power BI/Tableau, communication.
- **Outils** : SQL, Excel, Power BI, Python (Pandas), parfois Looker/Tableau.
- **Niveau de mathématiques** : statistiques descriptives, notions de probabilités. Pas besoin de mathématiques avancées.
- **Niveau de programmation** : modéré (SQL indispensable, Python utile).
- **Exemple de problème traité** : « Pourquoi le taux de conversion a-t-il baissé de 8 % le mois dernier sur le segment mobile ? »
- **Profil correspondant** : personnes aimant l'investigation, la clarté, la communication, et un usage concret et immédiat des données.

### Data Scientist

- **Rôle** : construire des modèles prédictifs et exploiter des données pour anticiper des comportements futurs.
- **Missions** : feature engineering, modélisation (régression, classification, clustering), évaluation de modèles, mise en production avec les Data Engineers.
- **Compétences clés** : statistiques avancées, machine learning, Python, parfois deep learning.
- **Outils** : Python (scikit-learn, PyTorch/TensorFlow), SQL, notebooks Jupyter, MLflow.
- **Niveau de mathématiques** : élevé (algèbre linéaire, probabilités, optimisation, statistiques inférentielles).
- **Niveau de programmation** : élevé.
- **Exemple de problème traité** : « Peut-on prédire, à partir de l'historique client, la probabilité de résiliation d'un abonnement dans les 3 prochains mois ? »
- **Profil correspondant** : personnes attirées par la modélisation mathématique, la recherche, l'expérimentation.

### Data Engineer

- **Rôle** : construire et maintenir l'infrastructure qui permet de collecter, stocker et acheminer la donnée.
- **Missions** : conception de pipelines ETL/ELT, architecture de bases de données, industrialisation des flux de données, cloud.
- **Compétences clés** : ingénierie logicielle, bases de données, systèmes distribués, cloud (AWS/Azure/GCP).
- **Outils** : SQL, Python/Scala, Airflow, Spark, Kafka, Docker, solutions cloud.
- **Niveau de mathématiques** : faible à modéré.
- **Niveau de programmation** : élevé, proche du génie logiciel.
- **Exemple de problème traité** : « Comment ingérer 50 millions d'événements par jour en garantissant une latence inférieure à 5 minutes ? »
- **Profil correspondant** : personnes attirées par l'architecture logicielle, la performance, les systèmes.

### BI Analyst (Business Intelligence Analyst)

- **Rôle** : concevoir des outils de reporting récurrents pour le pilotage de l'activité.
- **Missions** : modélisation de données décisionnelles, création et maintenance de dashboards, définition de KPI.
- **Compétences clés** : SQL, modélisation dimensionnelle, Power BI/Tableau, sens métier.
- **Outils** : Power BI, Tableau, SQL, parfois DAX.
- **Niveau de mathématiques** : faible.
- **Niveau de programmation** : modéré (SQL principalement).
- **Exemple de problème traité** : « Construire un dashboard de suivi mensuel du chiffre d'affaires par région pour le comité de direction. »
- **Profil correspondant** : personnes orientées outil, structuration de l'information, relation avec le métier.

### Business Analyst

- **Rôle** : faire le lien entre les besoins métier et les solutions techniques ou data.
- **Missions** : recueil de besoins, analyse de processus, rédaction de spécifications, suivi de projets.
- **Compétences clés** : compréhension métier, gestion de projet, analyse de processus, Excel.
- **Outils** : Excel, PowerPoint, parfois SQL, outils de gestion de projet.
- **Niveau de mathématiques** : faible.
- **Niveau de programmation** : faible à modéré.
- **Exemple de problème traité** : « Formaliser les règles de gestion d'un nouveau processus de facturation pour l'équipe technique. »
- **Profil correspondant** : personnes à l'aise avec le métier et la communication plus qu'avec la technique pure.

### Statisticien

- **Rôle** : concevoir des méthodes d'analyse rigoureuses et garantir la validité statistique des conclusions.
- **Missions** : plans d'expérience, modèles statistiques, tests d'hypothèses, inférence.
- **Compétences clés** : statistique mathématique, probabilités, R ou Python, rigueur méthodologique.
- **Outils** : R, Python, SAS, logiciels statistiques spécialisés.
- **Niveau de mathématiques** : très élevé.
- **Niveau de programmation** : modéré à élevé.
- **Exemple de problème traité** : « Concevoir un test A/B statistiquement valide pour mesurer l'effet d'une nouvelle interface. »
- **Profil correspondant** : personnes attirées par la théorie statistique et la rigueur mathématique, proches de la recherche.

---

## 3. Objectif : devenir Data Analyst

### Ce qu'un Data Analyst doit savoir faire, concrètement

- Comprendre un problème métier et le traduire en question analysable.
- Aller chercher la donnée (fichiers, bases SQL, API, exports).
- Évaluer la qualité de la donnée (valeurs manquantes, doublons, incohérences).
- Nettoyer et structurer les données.
- Écrire des requêtes SQL pour extraire, filtrer, agréger.
- Appliquer une analyse statistique simple et pertinente.
- Manipuler les données avec Python (Pandas) pour les cas que SQL ne couvre pas bien.
- Construire des visualisations claires et non trompeuses.
- Construire un dashboard interactif.
- Interpréter les résultats avec prudence (corrélation ≠ causalité, biais d'échantillonnage).
- Présenter des conclusions à un public non technique, avec une recommandation actionnable.

### Le workflow professionnel du Data Analyst

```text
Problème métier
↓
Collecte des données
↓
Compréhension des données
↓
Nettoyage
↓
SQL
↓
Analyse statistique
↓
Python
↓
Visualisation
↓
Dashboard
↓
Interprétation
↓
Présentation des résultats
```

**Exemple filé : baisse du taux de conversion e-commerce**

1. **Problème métier** : le service marketing constate une baisse des ventes en ligne et veut en comprendre la cause.
2. **Collecte des données** : extraction des logs de connexion, des commandes, des données de trafic publicitaire depuis la base SQL de production.
3. **Compréhension des données** : identifier les tables disponibles (utilisateurs, sessions, commandes), leurs relations (clés primaires/étrangères), leur fraîcheur.
4. **Nettoyage** : retirer les sessions de robots, corriger les doublons de commandes, traiter les valeurs de montant négatives (remboursements).
5. **SQL** : requêtes agrégées pour calculer le taux de conversion par jour, par canal d'acquisition, par device.
6. **Analyse statistique** : comparer les taux de conversion mobile vs desktop, tester si l'écart est significatif ou dû au hasard.
7. **Python** : croiser plusieurs sources (SQL + fichier CSV de campagnes publicitaires) que SQL seul gère mal.
8. **Visualisation** : graphique en courbes de l'évolution du taux de conversion sur 3 mois, segmenté par canal.
9. **Dashboard** : intégration dans un dashboard Power BI suivi par l'équipe marketing chaque semaine.
10. **Interprétation** : la baisse est concentrée sur le mobile depuis une mise à jour du site — hypothèse de bug d'ergonomie plutôt que de baisse de la demande.
11. **Présentation** : synthèse en 3 diapositives avec recommandation (auditer le parcours mobile) pour le comité marketing.

---

## 4. Roadmap des compétences

L'ordre proposé est pensé pour donner rapidement des résultats concrets tout en construisant les fondations correctement.

### 4.1 Python

**Pourquoi** : langage central de la Data, utilisé pour l'automatisation, le nettoyage, l'analyse et le machine learning.

**Ce qu'il faut réellement apprendre** : syntaxe de base, structures de contrôle, fonctions, listes/dictionnaires/tuples, compréhensions de liste, manipulation de fichiers, gestion des exceptions, notions d'orienté objet (classes simples), environnements virtuels, gestion de paquets (pip).

**Ce qui est secondaire au démarrage** : programmation asynchrone, métaclasses, développement web (Flask/Django), packaging avancé.

- **Débutant** : variables, boucles, fonctions, listes, dictionnaires.
- **Intermédiaire** : compréhensions de liste, gestion de fichiers, modules, POO simple.
- **Avancé** : décorateurs, generators, bonnes pratiques de structuration de projet.

**Erreurs à éviter** : apprendre Python de manière isolée sans jamais l'appliquer à un jeu de données réel ; vouloir tout apprendre du langage avant de passer à Pandas.

**Exercices** : implémenter des fonctions de traitement de listes, parser un fichier texte, écrire un petit script d'automatisation (renommage de fichiers, calcul de statistiques simples).

**Projet de validation** : un script qui lit un fichier CSV, calcule des statistiques simples (moyenne, min, max par catégorie) sans utiliser Pandas, pour bien comprendre les fondations avant d'utiliser la bibliothèque.

### 4.2 SQL

**Pourquoi** : langage universel d'interrogation des bases de données relationnelles, compétence numéro un exigée en entretien Data Analyst.

**Ce qu'il faut réellement apprendre** : SELECT/WHERE/ORDER BY, GROUP BY/HAVING, toutes les jointures (INNER, LEFT, RIGHT, FULL), sous-requêtes, CTE (WITH), fonctions d'agrégation, window functions (ROW_NUMBER, RANK, LAG/LEAD).

**Ce qui est secondaire au démarrage** : administration de base de données, tuning avancé d'index, procédures stockées complexes.

- **Débutant** : SELECT, WHERE, ORDER BY, LIMIT.
- **Intermédiaire** : GROUP BY, HAVING, jointures, sous-requêtes simples.
- **Avancé** : CTE, window functions, requêtes de type entretien technique.

**Erreurs à éviter** : apprendre uniquement la théorie sans écrire de requêtes ; ignorer les window functions, très demandées en entretien.

**Exercices** : SQLBolt, SQLZoo, exercices sur une base de données publique (ex. Chinook, Northwind).

**Projet de validation** : analyse complète d'une base de données relationnelle avec des requêtes multi-tables et un rapport de synthèse (voir Projet 2).

### 4.3 Statistiques et probabilités

**Pourquoi** : fondement théorique de toute interprétation de données ; permet d'éviter les conclusions erronées.

**Ce qu'il faut réellement apprendre** (au-delà du programme de prépa, orienté application) : statistiques descriptives (moyenne, médiane, variance, écart-type, quantiles), distributions usuelles (normale, binomiale), échantillonnage, théorème central limite, intervalles de confiance, tests d'hypothèses (test t, test du chi², ANOVA), p-value et son interprétation correcte, corrélation vs causalité, détection de valeurs aberrantes.

**Ce qui est secondaire au démarrage** : statistique bayésienne avancée, séries temporelles complexes, théorie de la mesure.

- **Débutant** : statistiques descriptives, notion de distribution.
- **Intermédiaire** : tests d'hypothèses, intervalles de confiance, corrélation.
- **Avancé** : régression linéaire/logistique, ANOVA, interprétation critique des résultats.

**Erreurs à éviter** : confondre significativité statistique et significativité pratique ; interpréter une p-value comme une probabilité que l'hypothèse soit vraie ; conclure à une causalité à partir d'une simple corrélation.

**Exercices** : calculer et interpréter des p-values sur des jeux de données réels, comparer deux groupes avec un test statistique adapté.

**Projet de validation** : étude statistique complète avec interprétation (voir Projet 4).

### 4.4 Pandas / NumPy

**Pourquoi** : bibliothèques incontournables de manipulation de données en Python.

**Ce qu'il faut réellement apprendre** : création/lecture de DataFrames, sélection et filtrage (loc/iloc), groupby et agrégations, gestion des valeurs manquantes, fusion de tables (merge/join/concat), séries temporelles simples, opérations vectorisées NumPy.

**Ce qui est secondaire au démarrage** : optimisation mémoire avancée, écriture de fonctions vectorisées personnalisées en NumPy pur pour la performance extrême.

- **Débutant** : lecture de fichiers, sélection de colonnes/lignes, filtres simples.
- **Intermédiaire** : groupby, merge, gestion des NaN, apply.
- **Avancé** : opérations vectorisées, manipulation de dates, pivot tables.

**Erreurs à éviter** : utiliser des boucles `for` explicites sur un DataFrame plutôt que les opérations vectorisées ; ignorer les avertissements de copie (`SettingWithCopyWarning`).

**Exercices** : micro-défis Kaggle Learn Pandas ; reproduire une analyse Excel avec Pandas.

**Projet de validation** : nettoyage et exploration d'un dataset réel (voir Projet 3).

### 4.5 Data Cleaning

**Pourquoi** : dans la réalité, la majorité du temps d'un Data Analyst est consacrée au nettoyage plutôt qu'à l'analyse elle-même.

**Ce qu'il faut réellement apprendre** : détection et traitement des valeurs manquantes (suppression, imputation), détection des doublons, normalisation des formats (dates, texte, unités), détection de valeurs aberrantes, validation de la cohérence des types de données.

**Ce qui est secondaire au démarrage** : imputation multiple avancée, détection d'anomalies par machine learning.

**Erreurs à éviter** : supprimer des lignes sans comprendre pourquoi elles sont manquantes ; remplacer systématiquement par la moyenne sans réflexion sur le contexte.

**Exercices** : Kaggle Learn « Data Cleaning ».

**Projet de validation** : intégré au Projet 3 (Pandas).

### 4.6 Data Visualization

**Pourquoi** : une analyse juste mal communiquée n'a aucun impact ; savoir choisir le bon graphique est une compétence à part entière.

**Ce qu'il faut réellement apprendre** : choix du graphique selon le message (évolution → courbe, comparaison → barres, répartition → parts, relation → nuage de points), bibliothèques Matplotlib et Seaborn, principes de lisibilité (éviter la surcharge, choisir les couleurs à bon escient, ne pas tronquer un axe pour exagérer une tendance).

**Ce qui est secondaire au démarrage** : visualisations 3D, bibliothèques de visualisation web avancées (D3.js).

**Erreurs à éviter** : utiliser un camembert pour plus de 5 catégories ; tronquer l'axe des ordonnées pour exagérer une différence ; surcharger un graphique d'informations.

**Exercices** : Kaggle Learn « Data Visualization ».

**Projet de validation** : intégré aux Projets 3, 4 et 6.

### 4.7 Excel

**Pourquoi** : encore omniprésent en entreprise ; souvent le premier outil utilisé avant même Python ou SQL.

**Ce qu'il faut réellement apprendre** : formules courantes (RECHERCHEV/XLOOKUP, SI, SOMME.SI, INDEX/EQUIV), tableaux croisés dynamiques, mise en forme conditionnelle, graphiques simples.

**Ce qui est secondaire au démarrage** : VBA avancé, macros complexes (utile mais non indispensable pour démarrer).

**Erreurs à éviter** : négliger Excel en pensant que « Python remplace tout » — de nombreuses entreprises l'utilisent encore comme interface principale.

**Exercices** : reconstruire avec Excel une analyse déjà faite en Pandas pour comparer les deux approches.

### 4.8 Power BI

**Pourquoi** : outil de référence en entreprise (notamment en France) pour la restitution de données sous forme de dashboards.

**Ce qu'il faut réellement apprendre** : connexion à des sources de données, Power Query (transformation), modélisation de données (relations entre tables), notions de base du langage DAX, création de visuels interactifs, publication de rapports.

**Ce qui est secondaire au démarrage** : administration de workspace en entreprise, DAX très avancé (time intelligence complexe).

**Erreurs à éviter** : construire un dashboard uniquement esthétique sans réflexion sur le message à transmettre ; multiplier les visuels sans hiérarchie de lecture.

**Exercices** : parcours Microsoft Learn officiel « Get started with Microsoft data analytics ».

**Projet de validation** : dashboard professionnel (voir Projet 5).

### 4.9 Git / GitHub

**Pourquoi** : indispensable pour versionner son travail, collaborer, et constituer un portfolio visible.

**Ce qu'il faut réellement apprendre** : init/clone, add/commit/push/pull, branches, merge, résolution de conflits simples, rédaction de README, structure de repository.

**Ce qui est secondaire au démarrage** : rebase interactif avancé, workflows Git complexes (Git flow) — utiles plus tard en environnement d'équipe.

**Erreurs à éviter** : committer des fichiers de données volumineux ou des identifiants/API keys ; ne pas écrire de messages de commit clairs.

**Projet de validation** : chaque projet de la roadmap doit être versionné et documenté sur GitHub.

### 4.10 Machine Learning (notions)

**Pourquoi** : non indispensable pour un poste de Data Analyst pur, mais très utile pour évoluer vers Data Scientist et pour comprendre les modèles utilisés en aval.

**Ce qu'il faut réellement apprendre** : différence apprentissage supervisé/non supervisé, régression linéaire et logistique, arbres de décision, notion de sur-apprentissage (overfitting), métriques d'évaluation simples (précision, rappel, RMSE).

**Ce qui est secondaire au démarrage** : deep learning, NLP avancé, MLOps — à explorer seulement après une bonne maîtrise des bases.

**Projet de validation** : Kaggle Learn « Intro to Machine Learning », puis une première compétition Kaggle simple (Titanic).

### 4.11 Notions de Data Engineering / Cloud

**Pourquoi** : utile pour comprendre l'environnement technique dans lequel évoluent les données, et pour évoluer vers un poste de Data Engineer.

**Ce qu'il faut réellement apprendre** : notions de pipeline de données (ETL/ELT), différence entre base de données relationnelle et non relationnelle, notions de base sur le cloud (stockage, calcul), notion de format de données (CSV, JSON, Parquet).

**Ce qui est secondaire au démarrage** : orchestration avancée (Airflow), architecture Big Data (Spark, Kafka) — à explorer après une base solide en Data Analyst.

---

## 5. Ressources d'apprentissage

Chaque ressource ci-dessous est directement rattachée à une étape de la roadmap de la section 4. Les ressources ont été vérifiées ; seules celles dont l'existence a pu être confirmée sont incluses.

### 5.1 Python

**Vidéos**

|Titre|Chaîne|Durée approx.|Niveau|Contenu|Lien|
|---|---|---|---|---|---|
|Learn Python – Full Course for Beginners|freeCodeCamp.org|~4h30|Débutant|Bases complètes du langage avec mini-projets|Voir l'article freeCodeCamp qui héberge le lien direct : https://www.freecodecamp.org/news/learn-python-free-python-courses-for-beginners/|
|Python for Everybody (Programming for Everybody)|freeCodeCamp.org / Dr Chuck (Univ. of Michigan)|~13h40|Débutant à intermédiaire|Programmation, structures de données, bases de données avec Python|https://www.freecodecamp.org/news/python-for-everybody/|
|Formation Python – Machine Learning (série)|MachineLearnia (Guillaume Saint-Cirgue)|Série de vidéos courtes (10–20 min chacune)|Débutant à intermédiaire|Python, NumPy, structures de données, en français|Chaîne à rechercher sur YouTube : « MachineLearnia »|

**Cours interactifs**

- **Kaggle Learn – Python** : https://www.kaggle.com/learn — niveau débutant, quelques heures, bases du langage orientées data (variables, fonctions, listes, bibliothèques externes).

**Documentation officielle**

- Documentation Python : https://docs.python.org/3/

### 5.2 SQL

**Vidéos**

|Titre|Chaîne|Durée approx.|Niveau|Contenu|Lien|
|---|---|---|---|---|---|
|SQL for Beginners / Data Analyst Bootcamp|Alex The Analyst|Série (plusieurs heures au total)|Débutant à avancé|SELECT, WHERE, GROUP BY, jointures, sous-requêtes, procédures stockées|https://www.youtube.com/playlist?list=PLUaB-1hjhk8FE_XZ87vPPSfHqb6OcM0cF|
|SQL Tutorial – Full Database Course for Beginners|freeCodeCamp.org|~4h20|Débutant|Introduction complète au SQL et aux bases de données relationnelles|Rechercher sur la chaîne YouTube freeCodeCamp.org (titre exact ci-dessus)|

**Cours interactifs**

- **SQLBolt** : https://sqlbolt.com — interactif, gratuit, sans compte requis ; couvre SELECT, filtres, jointures, sous-requêtes, jusqu'à des notions de DDL.
- **Kaggle Learn – Intro to SQL / Advanced SQL** : https://www.kaggle.com/learn — requêtes de base puis JOIN, sous-requêtes analytiques, fonctions de fenêtrage.
- **SQLZoo** : plateforme interactive complémentaire, notamment pour les jointures et les requêtes imbriquées.

**Documentation officielle** : selon le SGBD utilisé (PostgreSQL, MySQL) ; privilégier la documentation officielle du moteur choisi pour l'entraînement (PostgreSQL est recommandé pour son respect du standard SQL).

### 5.3 Statistiques et probabilités

**Vidéos**

|Titre|Chaîne|Durée approx.|Niveau|Contenu|Lien|
|---|---|---|---|---|---|
|StatQuest: Statistics Fundamentals|StatQuest with Josh Starmer|Série d'environ 8h au total|Débutant à intermédiaire|Distributions, échantillonnage, tests d'hypothèses, p-value, corrélation, régression|Syllabus complet et accès aux vidéos : https://classcentral.com/course/youtube-statistics-fundamentals-45654|
|StatQuest (série Machine Learning et stats appliquées)|StatQuest with Josh Starmer|Série (nombreuses vidéos courtes)|Intermédiaire à avancé|PCA, régression logistique, arbres de décision, ROC/AUC|Syllabus complet : https://classcentral.com/classroom/youtube-statquest-90294|

**Complément mathématique** : pour l'intuition sur l'algèbre linéaire et les probabilités (utile pour comprendre le fond des méthodes statistiques), la chaîne 3Blue1Brown propose des séries reconnues (« Essence of Linear Algebra », « Essence of Calculus ») — rechercher directement sur YouTube, la chaîne étant très largement documentée et citée par la communauté scientifique.

### 5.4 Pandas / NumPy

**Vidéos**

|Titre|Chaîne|Durée approx.|Niveau|Contenu|Lien|
|---|---|---|---|---|---|
|Python Pandas Tutorial (série complète)|Corey Schafer|Série de ~11 vidéos, 15–35 min chacune|Débutant à avancé|DataFrames, indexation, filtrage, groupby, nettoyage, dates, import/export|https://www.youtube.com/playlist?list=PL-osiE80TeTsWmV9i9c58mdDCSskIFdDS|
|Data Analysis with Python Course – NumPy, Pandas, Data Visualization|freeCodeCamp.org|~9h56|Débutant à intermédiaire|NumPy, Pandas, visualisation, projet fil rouge|Rechercher sur la chaîne YouTube freeCodeCamp.org|

Le code associé à la série de Corey Schafer est disponible ici : https://github.com/CoreyMSchafer/code_snippets/tree/master/Python/Pandas

**Cours interactifs**

- **Kaggle Learn – Pandas** : https://www.kaggle.com/learn/pandas — création/lecture, indexation, group by, types de données et valeurs manquantes, renommage/combinaison.
- **Mini-cours Pandas (TU Delft)** : série de vidéos courtes et dépôt d'exercices, orientée bonnes pratiques d'écriture Pandas : https://github.com/junzis/course-pandas

**Documentation officielle**

- Pandas : https://pandas.pydata.org/docs/
- NumPy : https://numpy.org/doc/stable/

### 5.5 Data Cleaning

- **Kaggle Learn – Data Cleaning** : https://www.kaggle.com/learn — valeurs manquantes, mise à l'échelle, parsing de dates, encodages de caractères, détection d'incohérences.

### 5.6 Data Visualization

- **Kaggle Learn – Data Visualization** : https://www.kaggle.com/learn — Seaborn, choix du graphique adapté, personnalisation.
- Documentation Matplotlib et Seaborn : à consulter directement sur leurs sites officiels respectifs pour la syntaxe exacte des fonctions utilisées dans les projets.

### 5.7 Excel

- Pas de ressource vidéo spécifique vérifiée à ce stade au-delà des chaînes généralistes ; privilégier le support officiel Microsoft (documentation Excel) et la pratique directe sur des tableaux de données réels (voir section Exercices).

### 5.8 Power BI

**Cours interactifs (officiel)**

- **Microsoft Learn – Get started with Microsoft data analytics** : https://learn.microsoft.com/training/paths/get-started-power-bi — gratuit, officiel, prépare à la certification Microsoft Certified: Data Analyst Associate (PL-300).
- **Microsoft Learn – Data Analytics with Microsoft** (parcours plus large) : https://learn.microsoft.com/training/paths/data-analytics-microsoft

**Documentation officielle**

- Power BI : https://learn.microsoft.com/power-bi/

### 5.9 Git / GitHub

**Vidéos**

|Titre|Chaîne|Durée approx.|Niveau|Contenu|Lien|
|---|---|---|---|---|---|
|Git and GitHub for Beginners – Crash Course|freeCodeCamp.org|~1h08|Débutant|Concepts de base, commandes essentielles, workflow GitHub|Article avec lien direct : https://www.freecodecamp.org/news/git-and-github-crash-course-for-beginners/|
|Learn Git – Full Course for Beginners|freeCodeCamp.org|~4h|Débutant à intermédiaire|Approfondissement : branches, merge, rebase, contribution open source|Article avec lien direct : https://www.freecodecamp.org/news/learn-git-in-detail-to-manage-your-code/|

**Documentation officielle**

- Git : https://git-scm.com/doc

### 5.10 Machine Learning (notions)

- **Kaggle Learn – Intro to Machine Learning / Intermediate Machine Learning** : https://www.kaggle.com/learn — arbres de décision, forêts aléatoires, validation croisée, gestion des valeurs manquantes et variables catégorielles.

**Documentation officielle**

- Scikit-learn : https://scikit-learn.org/stable/

### 5.11 Sources de données officielles (France et Sénégal)

- **data.gouv.fr** (plateforme officielle de l'État français) : https://www.data.gouv.fr
- **INSEE** (Institut national de la statistique et des études économiques, France) : https://www.insee.fr
- **ANSD** (Agence Nationale de la Statistique et de la Démographie, Sénégal) : https://www.ansd.sn — publie ses données en open data (formats CSV, JSON, API), avec un score d'ouverture des données classé premier en Afrique par l'Open Data Inventory (ODIN) 2024. Source à privilégier pour des projets ancrés sur des problématiques sénégalaises (démographie, emploi, commerce extérieur, prix).

### 5.12 Certification complémentaire (optionnelle)

- **Google Data Analytics Professional Certificate** (sur Coursera) : programme de 8 cours couvrant les fondamentaux du Data Analyst (nettoyage, analyse, visualisation, SQL, R, Tableau), avec projet de synthèse (capstone). Payant par abonnement mensuel, mais une **aide financière** est proposée par Coursera pour les personnes ne pouvant pas payer, ce qui rend le parcours accessible gratuitement sous conditions. À considérer une fois les bases de cette roadmap acquises : le programme enseigne R plutôt que Python, il est donc complémentaire à cette roadmap plutôt qu'un point de départ. Cette certification peut avoir une valeur de crédibilité auprès de recruteurs qui ne connaissent pas encore un portfolio GitHub.

---

## 6. Exercices

### SQL

**Niveau 1** — SELECT, WHERE, ORDER BY **Niveau 2** — GROUP BY, HAVING, agrégations **Niveau 3** — JOIN (INNER/LEFT/RIGHT/FULL), sous-requêtes, CTE **Niveau 4** — Window Functions (ROW_NUMBER, RANK, LAG/LEAD), problèmes de type entretien (top N par groupe, croissance mois par mois)

Pratiquer sur : SQLBolt (https://sqlbolt.com) pour les niveaux 1 et 2, puis Kaggle Learn Advanced SQL pour les niveaux 3 et 4, en complément d'une base de données publique de type Chinook ou Northwind importée localement.

### Python

**Niveau 1** — variables, conditions, boucles **Niveau 2** — fonctions, listes, dictionnaires, compréhensions de liste **Niveau 3** — manipulation de fichiers, gestion des exceptions, modules **Niveau 4** — mini-scripts d'automatisation appliqués à des fichiers de données réels

Pratiquer sur : Kaggle Learn – Python (https://www.kaggle.com/learn).

### Pandas

**Niveau 1** — lecture de fichiers, sélection de colonnes/lignes **Niveau 2** — filtres, tri, création de colonnes calculées **Niveau 3** — groupby, agrégations multiples, gestion des valeurs manquantes **Niveau 4** — merge/join de plusieurs tables, séries temporelles, pivot tables

Pratiquer sur : Kaggle Learn – Pandas (https://www.kaggle.com/learn/pandas), puis sur un dataset Kaggle réel (voir section Projets).

### Statistiques

**Niveau 1** — moyenne, médiane, écart-type, quantiles **Niveau 2** — distributions usuelles, échantillonnage **Niveau 3** — intervalles de confiance, tests d'hypothèses (test t, chi²) **Niveau 4** — régression linéaire/logistique, interprétation critique (p-hacking, biais de sélection)

Pratiquer sur : la série StatQuest Statistics Fundamentals (lien section 5.3), en appliquant chaque notion sur un jeu de données réel plutôt qu'en restant sur l'exemple théorique de la vidéo.

### Power BI

**Niveau 1** — connexion à une source de données, création d'un premier visuel **Niveau 2** — Power Query : nettoyage et transformation des données importées **Niveau 3** — modélisation de données (relations entre tables, modèle en étoile) **Niveau 4** — DAX (mesures calculées), dashboard multi-pages avec filtres croisés

Pratiquer sur : le parcours Microsoft Learn officiel (lien section 5.8), en reconstruisant chaque exercice avec un jeu de données personnel plutôt qu'avec le jeu de données fourni par défaut.

### Machine Learning

**Niveau 1** — régression linéaire simple **Niveau 2** — régression logistique, arbres de décision **Niveau 3** — validation croisée, gestion du sur-apprentissage **Niveau 4** — première compétition Kaggle (ex. Titanic — Machine Learning from Disaster)

Pratiquer sur : Kaggle Learn – Intro to Machine Learning (https://www.kaggle.com/learn), puis la compétition Kaggle « Titanic ».

---

## 7. Projets

Chaque projet doit être versionné sur GitHub avec un README dédié (voir section 8).

### Projet 1 — Python : analyse simple

- **Objectif** : manipuler un fichier de données sans bibliothèque spécialisée, pour consolider les bases du langage.
- **Dataset** : un fichier CSV simple (ex. relevés météo, notes d'élèves, ventes d'un petit magasin — disponible sur Kaggle Datasets).
- **Questions à résoudre** : quelles sont les valeurs moyennes/extrêmes par catégorie ? Quelle est la tendance sur la période ?
- **Compétences utilisées** : Python de base, lecture de fichiers, structures de données.
- **Livrables** : un script Python commenté + un court résumé des résultats.
- **Difficulté** : débutant.
- **Idées d'amélioration** : ajouter une gestion d'erreurs robuste, comparer les résultats avec une implémentation Pandas.

### Projet 2 — SQL : analyse d'une base de données relationnelle

- **Objectif** : interroger une base de données réaliste à plusieurs tables liées.
- **Dataset** : base Chinook (magasin de musique) ou Northwind (commerce), disponibles publiquement sous forme de fichiers SQL à importer dans une base locale (SQLite/PostgreSQL).
- **Questions à résoudre** : quels sont les produits/clients les plus rentables ? Quelle est l'évolution des ventes par période et par catégorie ?
- **Compétences utilisées** : SQL (jointures, agrégations, sous-requêtes, window functions).
- **Livrables** : un fichier `.sql` documenté avec les requêtes et un résumé des insights.
- **Difficulté** : intermédiaire.
- **Idées d'amélioration** : ajouter des window functions pour un classement (top clients par mois), optimiser les requêtes lentes.

### Projet 3 — Pandas : nettoyage et exploration d'un dataset réel

- **Objectif** : nettoyer un dataset réellement imparfait et en extraire des enseignements.
- **Dataset** : un dataset Kaggle avec valeurs manquantes et incohérences (ex. données immobilières, données de santé publique, données de trajets).
- **Questions à résoudre** : quelles variables sont corrélées ? Quels sous-groupes se distinguent ?
- **Compétences utilisées** : Pandas, NumPy, visualisation (Matplotlib/Seaborn).
- **Livrables** : un notebook Jupyter structuré (nettoyage → exploration → visualisations → conclusions).
- **Difficulté** : intermédiaire.
- **Idées d'amélioration** : automatiser le nettoyage sous forme de fonctions réutilisables, ajouter des tests de cohérence.

### Projet 4 — Statistiques : étude statistique avec interprétation

- **Objectif** : appliquer une démarche statistique rigoureuse sur un jeu de données réel.
- **Dataset** : un dataset permettant de comparer deux groupes (ex. résultats d'un test A/B, données de santé, performances scolaires selon un facteur).
- **Questions à résoudre** : la différence observée entre les groupes est-elle statistiquement significative ? Quelle est l'ampleur de l'effet ?
- **Compétences utilisées** : statistiques descriptives et inférentielles, tests d'hypothèses.
- **Livrables** : un rapport présentant la méthodologie, les résultats des tests, et une interprétation prudente (limites incluses).
- **Difficulté** : intermédiaire à avancé.
- **Idées d'amélioration** : ajouter une visualisation de la distribution avec intervalle de confiance, discuter la puissance statistique du test.

### Projet 5 — Power BI : dashboard professionnel

- **Objectif** : construire un dashboard interactif destiné à un public non technique.
- **Dataset** : données de ventes, données ouvertes de type data.gouv.fr, ou données personnelles (finances personnelles, suivi sportif).
- **Questions à résoudre** : quels indicateurs clés (KPI) suivre ? Comment les présenter de façon lisible et actionnable ?
- **Compétences utilisées** : Power Query, modélisation de données, DAX, mise en forme visuelle.
- **Livrables** : un fichier `.pbix` et des captures d'écran commentées dans le README du projet.
- **Difficulté** : intermédiaire.
- **Idées d'amélioration** : ajouter des filtres croisés, une page mobile, des mesures DAX de comparaison temporelle (mois précédent, année précédente).

### Projet 6 — Projet complet (portfolio)

```text
SQL
+
Python
+
Pandas
+
Statistiques
+
Visualisation
+
Power BI
```

- **Objectif** : mener une analyse de bout en bout, du problème métier au dashboard, comme en conditions professionnelles.
- **Dataset** : un dataset conséquent et réaliste (ex. données de vols aériens, données de santé publique de l'INSEE ou de data.gouv.fr, données Kaggle de e-commerce).
- **Questions à résoudre** : à définir soi-même à partir d'une problématique métier plausible (ex. « comment optimiser les tarifs selon la saisonnalité ? »).
- **Compétences utilisées** : l'ensemble de la roadmap.
- **Livrables** : extraction SQL documentée, notebook Pandas de nettoyage/analyse, étude statistique, dashboard Power BI, README de synthèse.
- **Difficulté** : avancé — c'est le projet phare du portfolio.
- **Idées d'amélioration** : ajouter une composante prédictive simple (régression), automatiser la mise à jour des données.

### Sources de datasets publics

- **Kaggle Datasets** : catalogue très large de jeux de données de tous domaines, avec descriptions et niveaux de qualité variables.
- **ANSD** : https://www.ansd.sn — données statistiques officielles du Sénégal (démographie, emploi, commerce extérieur, prix, recensement), en formats CSV/JSON/API. Base idéale pour un projet ancré localement (ex. Projet 6).
- **data.gouv.fr** : https://www.data.gouv.fr — données publiques françaises (transports, santé, environnement, économie).
- **INSEE** : https://www.insee.fr — données statistiques officielles françaises (démographie, économie, emploi).

---

## 8. GitHub et portfolio

### Structure de repository recommandée

```text
project/
├── data/
├── notebooks/
├── src/
├── reports/
├── images/
├── README.md
└── requirements.txt
```

- `data/` : données brutes et/ou nettoyées (éviter de committer des fichiers volumineux ; utiliser `.gitignore` si nécessaire).
- `notebooks/` : notebooks Jupyter d'exploration et d'analyse.
- `src/` : scripts Python réutilisables (fonctions de nettoyage, de chargement, etc.).
- `reports/` : rapports finaux (PDF, Markdown).
- `images/` : visualisations exportées, captures de dashboard.
- `README.md` : présentation du projet.
- `requirements.txt` : dépendances Python du projet.

### Contenu attendu dans le README de chaque projet

- **Problème** : quelle question métier le projet cherche-t-il à résoudre ?
- **Dataset** : source, taille, période couverte, licence si pertinente.
- **Méthodologie** : étapes suivies (collecte, nettoyage, analyse).
- **Analyse** : principales étapes d'exploration et choix effectués.
- **Résultats** : ce qui a été trouvé, avec chiffres et visualisations clés.
- **Limites** : biais connus, données manquantes, hypothèses simplificatrices.
- **Visualisations** : graphiques ou captures d'écran illustrant les résultats.
- **Conclusion** : synthèse actionnable, ce qu'on ferait différemment avec plus de temps/données.

Un portfolio de 3 à 6 projets bien documentés, couvrant SQL, Python/Pandas, statistiques et Power BI, est largement suffisant pour candidater à un stage de Data Analyst.

---

## 9. Roadmap temporelle

Cette roadmap est pensée pour un étudiant en MPI poursuivant sa prépa en parallèle : elle privilégie la régularité à l'intensité.

### 3 mois — Fondamentaux

- Python (bases) + SQL (niveaux 1 à 3) + statistiques descriptives.
- Premiers exercices Kaggle Learn (Python, Pandas, Intro to SQL).
- Mise en place de l'environnement de travail (Python, Git, éditeur de code).

### 6 mois — Niveau junior / premiers projets sérieux

- Pandas maîtrisé, Data Cleaning, Data Visualization.
- SQL niveau 4 (window functions).
- Statistiques inférentielles (tests d'hypothèses).
- Réalisation des Projets 1 à 4.
- Premier dashboard Power BI simple.

### 12 mois — Portfolio solide et préparation aux stages

- Power BI approfondi (Projet 5).
- Projet complet de portfolio (Projet 6).
- Notions de Machine Learning et premiers pas en Data Engineering/Cloud.
- Portfolio GitHub complet et documenté, CV à jour, préparation aux entretiens techniques.

### Adaptation selon le temps disponible

|Rythme|3 mois|6 mois|12 mois|
|---|---|---|---|
|3 h/semaine|Python + SQL niveaux 1-2|+ Pandas, stats descriptives|Portfolio partiel (2-3 projets), bases Power BI|
|5 h/semaine|Python + SQL complet + stats descriptives|+ Pandas, Data Cleaning/Viz, Projets 1-3|Portfolio complet (4-5 projets), Power BI, notions ML|
|10 h/semaine|Fondamentaux complets + Projets 1-2|Projets 1-5, stats inférentielles, Power BI|Portfolio complet + Projet 6 + ML + préparation entretiens|

Le rythme 3–5 h/semaine est réaliste en parallèle d'une prépa MPI ; le rythme 10 h/semaine est plutôt adapté aux vacances scolaires ou à une période post-prépa.

---

## 10. Préparation aux études après la MPI

Il n'existe pas de voie unique ni de « meilleure école » : le choix dépend du niveau de spécialisation souhaité, du type de mathématiques/informatique que l'on veut approfondir, et de contraintes concrètes (coût, bourses, mobilité). Pour un étudiant en MPI au Sénégal, deux grandes directions coexistent et ne s'excluent pas : rester dans le système des concours français, ou rejoindre une école régionale spécialisée.

### Voie 1 — Concours français post-prépa

Les CPGE scientifiques suivant le programme français (y compris celles hébergées au Sénégal, à l'École Polytechnique de Thiès) donnent accès aux mêmes concours communs qu'en France :

- **Concours communs** : CCINP, Mines-Ponts, Centrale-Supélec, X-ENS, Concours Avenir Prépas, Ingeni'Up, selon la filière et le niveau visé, avec ensuite une spécialisation possible en 3ᵉ année vers la data, la statistique ou l'informatique.
- **Écoles spécialisées en statistique et data** en France (ENSAE Paris, ENSAI, etc.), accessibles selon les concours et banques d'épreuves concernées.
- **Parcours universitaires français** (L3 informatique ou mathématiques appliquées, puis master orienté data science, statistique ou intelligence artificielle).

Les élèves des CPGE sénégalaises passent déjà ces concours français directement depuis le Sénégal ; les bourses d'excellence du gouvernement sénégalais permettent aussi, pour certains profils, une prépa directement en France (accords avec des lycées comme Louis-le-Grand, Henri IV ou le Lycée du Parc).

### Voie 2 — Écoles régionales spécialisées (Sénégal et Afrique de l'Ouest)

- **ENSAE Pierre Ndiaye (Dakar)** : école nationale de la statistique et de l'analyse économique, rattachée à l'ANSD, à vocation régionale (élèves venant de plusieurs pays africains). Recrute sur concours (cycle Ingénieur Statisticien Économiste en 5 ans, ou Analyste Statisticien en 3 ans) ; formation très mathématique, débouchant sur des postes en statistique publique, banques centrales, institutions internationales et secteur privé — un parcours pertinent pour qui vise plutôt Data Analyst/Statisticien qu'ingénieur logiciel.
- **École Supérieure Polytechnique (ESP), Université Cheikh Anta Diop de Dakar** : grande école d'ingénieurs publique sénégalaise, avec des filières informatique/télécoms pouvant mener vers la data.
- **École Polytechnique de Thiès (EPT)** : école d'ingénieurs qui héberge également les CPGE sénégalaises, avec des filières informatique et génie logiciel.
- **Parcours universitaires sénégalais** : UCAD (Université Cheikh Anta Diop) et Université Virtuelle du Sénégal (UVS) proposent des filières informatique et mathématiques appliquées, y compris à distance pour l'UVS.

Ces écoles régionales ne s'opposent pas à la voie française : elles constituent une option de repli solide, moins coûteuse et sans contrainte de mobilité, en cas de non-admission aux concours français ou de choix délibéré de rester dans la sous-région.

### Critères à examiner pour choisir une formation (plutôt qu'un classement)

- **Niveau de mathématiques enseigné** : statistique théorique, optimisation, probabilités avancées.
- **Niveau d'informatique enseigné** : algorithmique, bases de données, génie logiciel, cloud.
- **Possibilités de spécialisation** en 2ᵉ/3ᵉ année (data science, IA, ingénierie des données, statistique).
- **Stages et alternance** : durée, obligation, réseau d'entreprises partenaires (au Sénégal comme à l'international).
- **Projets concrets** proposés pendant la formation (projets data, hackathons, partenariats entreprises).
- **Débouchés** observés (types de postes, secteurs, mobilité géographique) pour les promotions précédentes.
- **Coût réel et bourses disponibles** : frais de scolarité, bourses d'excellence, possibilités de bourses de mobilité pour les établissements à l'étranger.

### Où vérifier ces critères avec des sources actuelles

- **Onisep** (information officielle sur l'orientation en France) : https://www.onisep.fr
- **L'Étudiant** (informations sur les concours et écoles post-prépa, mises à jour chaque année) : https://www.letudiant.fr
- Les **sites officiels** de chaque établissement envisagé (y compris ENSAE Pierre Ndiaye, ESP, EPT, UCAD, UVS), pour les programmes, les débouchés, les modalités d'admission et les frais à jour.

Ces informations évoluant chaque année (places disponibles, épreuves, spécialisations, frais), il est recommandé de vérifier systématiquement sur les sites officiels au moment de candidater plutôt que de se fier à des informations datées.

### Le marché de l'emploi Data au Sénégal et à l'international

Le secteur data se développe fortement à Dakar, porté notamment par les banques (reporting réglementaire), les télécoms et les scaleups technologiques (fintech, e-commerce), ce qui crée une demande locale réelle pour des profils Data Analyst. En parallèle, les compétences de cette roadmap (SQL, Python, Power BI) sont directement valorisables sur des missions à distance pour des entreprises étrangères, via des plateformes de freelancing internationales. Les chiffres précis de salaires évoluant vite et variant fortement selon les sources, il est préférable de les vérifier directement lors des entretiens ou auprès de plateformes d'emploi reconnues plutôt que de se fier à des grilles trouvées en ligne.

---

## 11. Préparation au stage

### Checklist technique

```markdown
- [ ] Python (bases solides + Pandas)
- [ ] SQL (jusqu'aux window functions)
- [ ] Pandas (nettoyage, groupby, merge)
- [ ] Statistiques (descriptives + tests d'hypothèses)
- [ ] Excel (formules courantes, TCD)
- [ ] Power BI (Power Query, DAX de base, dashboard)
- [ ] Git / GitHub (workflow de base)
```

### Checklist portfolio

```markdown
- [ ] 3 à 5 projets documentés
- [ ] GitHub propre et organisé
- [ ] README complet pour chaque projet
- [ ] Au moins un dashboard Power BI
- [ ] Analyses documentées avec conclusions claires
```

### Exemples de questions d'entretien technique

```text
Quelle différence entre INNER JOIN et LEFT JOIN ?
Comment traiter les valeurs manquantes dans un dataset ?
Quelle différence entre moyenne et médiane, et quand privilégier l'une ou l'autre ?
Comment détecter une valeur aberrante ?
Qu'est-ce qu'une p-value, et quelle est l'erreur d'interprétation la plus fréquente ?
Comment optimiser une requête SQL lente ?
Comment choisir le bon type de graphique pour un message donné ?
```

### Ressources pour s'entraîner aux entretiens

- **Kaggle Learn – Advanced SQL** (https://www.kaggle.com/learn) pour retravailler les requêtes de type entretien (top N par groupe, window functions).
- Reprendre la série **StatQuest** (section 5.3) pour être capable d'expliquer p-value, corrélation, et tests d'hypothèses avec ses propres mots, sans réciter une formule.
- Préparer 2 à 3 projets de son portfolio pour pouvoir les présenter oralement en 2 minutes chacun (problème → méthode → résultat → limite).

---

## 12. Checklist finale

```markdown
- [ ] Python
- [ ] NumPy
- [ ] Pandas
- [ ] SQL
- [ ] Statistiques
- [ ] Data Cleaning
- [ ] Data Visualization
- [ ] Excel
- [ ] Power BI
- [ ] Git
- [ ] GitHub
- [ ] Projet SQL
- [ ] Projet Python
- [ ] Projet statistiques
- [ ] Dashboard Power BI
- [ ] Projet complet
- [ ] Portfolio
- [ ] CV
```

---

## 13. Par où commencer aujourd'hui ?

1. **Installer son environnement de travail** : Python (via Anaconda ou installation classique + VS Code), Git, et créer un compte GitHub.
2. **Créer le repository GitHub de sa roadmap** : un dépôt personnel dans lequel ce README sera versionné, et qui accueillera progressivement les projets.
3. **Commencer le cours Kaggle Learn – Python** (https://www.kaggle.com/learn) pour consolider les bases dans un contexte orienté données.
4. **Commencer les premières leçons de SQLBolt** (https://sqlbolt.com) : 20 à 30 minutes suffisent pour poser les premiers concepts (SELECT, WHERE).
5. **Regarder les 2 ou 3 premières vidéos de la playlist SQL d'Alex The Analyst** (https://www.youtube.com/playlist?list=PLUaB-1hjhk8FE_XZ87vPPSfHqb6OcM0cF) pour ancrer les notions vues sur SQLBolt dans un contexte pratique et professionnel.

_Idée bonus pour ancrer l'apprentissage dans un contexte local : une fois les bases SQL/Pandas posées, explorer une donnée réelle et gratuite sur https://www.ansd.sn pour le premier vrai projet (voir Projet 6)._