# cars-pipeline-databricks
Reconstruction d’un pipeline de reporting métier dans Databricks – basé sur mon expérience HSolutions


 1. Ingestion des données
Webscraping ou lecture d’un fichier CSV public (simulé comme une source brute)

Ingestion dans un DataFrame Spark

2. Nettoyage / transformation
Traitement des valeurs nulles / types / doublons

Normalisation de colonnes

3. Stockage
Sauvegarde en Delta Lake (format .delta) ou Parquet

Utilisation du “bronze → silver” pattern

4. Visualisation
Création de KPIs simples avec display() ou avec SQL dans Databricks

Graphique via notebook intégré

5. Bonus : Orchestration
Ajout d’un dbutils.notebook.run() pour simuler une pipeline orchestrée
