# Mon portfolio

# 1. Projets Data

## 1.1 Projets Big Data

### [Projet Big Data: Netflix Analytics](https://github.com/gbangout/projet-big-data-netflix-analytics.git)
Besoin métier : Aider l’équipe produit à identifier les genres et zones géographiques à fort potentiel en analysant le catalogue existant pour orienter les décisions de contenu.

Approche : Cadrage des indicateurs utiles, ingestion et nettoyage des données à l’échelle (PySpark), enrichissement et structuration en base analytique (PostgreSQL), calculs distribués (Spark SQL) puis restitution visuelle des tendances (genres, pays, ratings, évolution temporelle) orientée décision.

Stack : PySpark, Pandas, Spark SQL, PostgreSQL, visualisations type BI.

Résultat : Identification des segments sous-exploités mais en croissance, catalogue prêt à être branché sur un dashboard ou pipeline produit.

### [Projet Big Data: Investissement dans Airbnb à Paris](https://github.com/gbangout/projet-big-data-investissement-airbnb.git)

Besoin métier simulé : Identifier les zones à fort rendement locatif pour guider une stratégie d’investissement immobilier sur Airbnb.

Approche : Ingestion et nettoyage des listings et avis utilisateurs, structuration des données (PostgreSQL) et automatisation des flux (NiFi), calculs distribués (Spark) et analyse des KPI (prix, taux d’occupation, attractivité zone).

Stack : Python, NiFi, Spark, PostgreSQL, visualisation BI.

Résultat : Mise en place d’une base analytique exploitable permettant de prioriser les quartiers à fort potentiel ROI.

### [Projet Big Data: Conception d’une solution Big Data pour optimiser la logistique](https://github.com/gbangout/gestion-de-projet-big-data-logistics.git)
Besoin métier : Améliorer la performance logistique en réduisant les retards de livraison, détectant des pannes et améliorant satisfaction client.

Approche : Conception d’une architecture Big Data temps réel : ingestion IoT + transactions (Kafka/NiFi), stockage distribué (Hadoop), traitement streaming (Spark Streaming), stockage NoSQL et dashboards opérationnels.

Stack : Kafka, NiFi, Hadoop, Spark, MongoDB/Cassandra, PowerBI/Tableau/Kibana.

Résultat : Détection anticipée des anomalies et optimisation de la chaîne logistique — base prête à connecter à des alertes temps réel et dashboards métier.

## 1.2 Projets Machine Learning (ML, NLP, Computer Vision, Time Series Forecasting)

### [Projet NLP Text Mining: Analyse et prédiction des sentiments de tweets](https://github.com/gbangout/text-mining-sentiment.git)
Besoin métier : Comprendre la perception des utilisateurs vis-à-vis d’une marque à partir des tweets.

Approche : Préparation et vectorisation des textes, entraînement d’un modèle de classification binaire des sentiments (positif / négatif).

Stack : Python, scikit-learn, pandas, nltk, TF-IDF, régression logistique.

Résultat : Modèle de classification des sentiments opérationnel pour analyser en continu la tonalité des retours utilisateurs.


### [Projet ML clustering rapport sientifique: Analyse de la tendance de la pollution en Europe](https://www.eionet.europa.eu/etcs/etc-he/products/etc-he-products/etc-he-reports/etc-he-report-2023-8-long-term-trends-of-air-pollutants-at-european-and-national-level-2005-2021)
Besoin métier : Identifier des profils d’évolution de pollution pour orienter les politiques environnementales en France et en Europe.

Approche : Analyse temporelle longue durée des polluants, clustering des trajectoires d’évolution pour regrouper les tendances par zone géographique.

Stack : Python, scikit-learn, visualisation scientifique.

Résultat : Typologie claire des dynamiques de pollution, facilitant des décisions ciblées par zone prioritaire.

### [Projet ML : Prédiction de souscription bancaire](https://github.com/gbangout-apziva/term-deposit.git)
Besoin métier : Prioriser les clients à fort potentiel de conversion pour une campagne de dépôt à terme.

Approche : Feature engineering, modèle supervisé avec validation croisée à 5 plis et optimisation.

Stack : Python, scikit-learn.

Résultat : Score de performance > 81%, modèle prêt à être intégré dans une campagne marketing ciblée.


### [Projet time series forecasting: Prédiction de prix boursiers & recommandation d’investissement](https://github.com/gbangout-apziva/term-deposit.git)
Besoin métier simulé : Aider une équipe finance à décider quand investir en automatisant l’analyse des tendances boursières et la prise de décision (Buy / Sell / Hold).

Approche : Construction d’un modèle de prévision des prix (time series / deep learning), puis développement d’un système de recommandation intelligent basé sur les signaux de marché générés.

Stack : Python, LSTM / modèles de séries temporelles, scikit-learn.

Résultat : 90% de précision sur la prédiction de prix et 69% de recommandations d’achat/vente correctes, base exploitable pour un assistant d’aide à la décision financière.


### [Projet Computer Vision: MonReader (Vision par Ordinateur pour la numérisation automatique de documents)](https://github.com/gbangout-apziva/MonReader.git)
Besoin utilisateur : Permettre à des personnes malvoyantes, chercheurs ou archivistes de numériser rapidement de gros volumes de documents sans intervention manuelle, en détectant automatiquement les changements de page.

Approche : Constitution d’un dataset vidéo labellisé ("page tournée" / "fixe"), extraction des frames, entraînement d’un modèle CNN pour détecter le moment optimal de capture. Intégration dans un pipeline de traitement automatisé (détection → capture HD → recadrage → redressement → OCR).

Stack : Python, CNN (Computer Vision), traitement d’images, pipeline ML embarqué.

Résultat : Détection fiable des moments de capture, base technologique exploitable pour une solution mobile de scan intelligent, orientée accessibilité et productivité.

### [Projet NLP: Potential Talents (Matching automatique candidats)](https://github.com/gbangout-apziva/potential-talents.git)
Besoin métier : Aider les RH ou équipes Talent Acquisition à identifier rapidement les candidats les plus adaptés à un poste, sans lire manuellement chaque CV/profil.

Approche : Extraction et vectorisation des informations candidats (textes de CV / profils), calcul de similarité NLP avec les exigences du poste, scoring automatique d’adéquation, avec possibilité d’utiliser le modèle en recommandation interne.

Stack : NLP (TF-IDF / embeddings), Python, scikit-learn, pipeline de classification / ranking.

Résultat : Priorisation automatique des profils les plus pertinents, base exploitable pour un outil de présélection RH assisté par IA.


### [Projet ML: Prédiction de satisfaction client](https://github.com/gbangout-apziva/customer-happiness.git)
Besoin métier : Identifier automatiquement si un client est satisfait ou non en fonction de ses réponses à un questionnaire, pour anticiper actions correctives ou fidélisation.

Approche : Exploration des données → feature selection et tuning d’hyperparamètres pour éviter le surapprentissage → entraînement de modèles de classification (Random Forest et XGBoost) → sélection du modèle optimal.

Stack : Python, scikit-learn, Random Forest, XGBoost, feature engineering.

Résultat : Modèle Random Forest retenu avec F1-score 79% et accuracy test 69%, exploitable pour monitorer la satisfaction client et guider les actions commerciales.

## 1.3 Mon positionnement pour créer de la valeur métier par la Data scientist dans la Finance
Mission : Traduire des besoins métiers (marketing, risque, fraude) en solutions data opérationnelles, explicables et responsables.

Approche : Industrialisation de modèles prédictifs (ML, IA générative), documentation Git, explication aux équipes métiers, animation de la communauté Data et respect de la gouvernance IA.

Stack / Outils : Python, SQL, ML/Deep Learning, LLM et RAG, prompt engineering, outils BI.

Résultat / Impact : Capacité à produire modèles industrialisables, éthiques et actionnables pour soutenir les décisions métiers et favoriser l’innovation collaborative.

# 2. [Travaux de recherche scientifique](https://scholar.google.com/citations?hl=en&user=t3vUxwgAAAAJ)
