# sql-data-warehouse-project
Building a modern data warehouse with SQL server, including ETL and data modeling

On veut réliser un projet Data  Engineer(  Data Warehouse ) dans le but de permetre aux décideurs de l'entreprise  de prendre de meilleures décision sur base de l'analyse et le raport réalisé sur ces données.
La source de données est constituée de 2 dossiers : 
crm : qui cinteint 3 fichiers csv ( customers , product , sales)
erp : qui contient 3 fichiers csv ( category , localite , customer_inf).
Toutes les données sont à l'état  brut et necessitent  le netoyage  les transformations en vue  produire un star schema  fact_sales , dim_products , dim_customers.
L'architecture adoptée est celle de medals c'est à dire en 3 couches :
Bronze layer : Dans cette étape les données seront transfeérs vers sql server à l'état brut c'est à dire sans aucune transformation.
Durand cette étape jutilise SSis pour charger les données  dans sql server.
Silver lay :  Dans cette étape les données seront transfeérs vers sql server  après  le netouyage et les transformations necessairesJ'utilise l  le langage python et plus précisément  les librairies pandas, numpy 
Gold layer : La modélisation finales dans cette couche les datas sont prêt pour le reporting et l'analyse,  le schema utilisé est elui de star schema
