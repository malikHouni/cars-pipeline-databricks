#  Car Data Pipeline – Spark + Delta Lake (Databricks Community Edition)

Projet complet de pipeline Big Data inspiré d'une expérience professionnelle.

##  Architecture Medallion

- **Bronze** : ingestion brute de fichiers JSON (multi-fichiers)
- **Silver** : nettoyage, typage, enrichissement
- **Gold** : KPI agrégés et création de vues analytiques

##  Stack technique

- Apache Spark
- Delta Lake
- Databricks (Community Edition)
- GitHub Actions (CI notebook)
- dbutils.notebook.run() (simulation d’orchestration)

##  Étapes

1. Ingestion multi-JSON (notebooks/01_bronze_ingestion.ipynb)
2. Transformation Silver (notebooks/02_silver_transformation.ipynb)
3. Agrégation & vue SQL (notebooks/03_gold_analysis.ipynb)

##  Pour aller plus loin

- Orchestration complète dans un environnement pro (Airflow, Databricks Jobs)
- Monitoring / Logging Spark
- Stockage sur S3 + gestion de partition

