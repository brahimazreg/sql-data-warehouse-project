# sql-data-warehouse-project
Building a modern data warehouse with SQL server, including ETL and data modeling

On veut réaliser un projet Data  Engineer(  Data Warehouse ) dans le but de permetre aux décideurs de l'entreprise  de prendre de meilleures décisions sur base de l'analyse et du  raport réalisés sur ces données.
L'objectve de cette étude :
- Comportement dees customers  et top des 10 meilleurs customers.
- Performance des produits .
- Tendence des ventes.
La source de données est constituée de 2 dossiers : 
crm : qui contient 3 fichiers csv ( customers , products , sales)
erp : qui contient 3 fichiers csv ( category , localite , customer_inf).
Toutes les données sont à l'état  brut et necessitent  le netoyage  les transformations en vue de produire un star schema  fact_sales , dim_products , dim_customers.
L'architecture adoptée est celle de medals c'est à dire en 3 couches :
Bronze layer : Dans cette étape les données seront transférées vers  sql server à l'état brut c'est à dire sans aucune transformation.
Durand cette étape jutilise SSIS pour charger les données  dans sql server.
Silver layer :  Dans cette étape les données seront transfeérs vers sql server  après  le netouyage et les transformations necessaires. J'utilise  le langage python et plus précisément  les librairies pandas, numpy 
Gold layer : La modélisation finale dans cette couche les datas sont prêts pour le reporting et l'analyse,  le schema utilisé est celui de star schema.

