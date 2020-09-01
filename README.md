# Détection de fraudes en ligne

Ce projet vise à partir d'un jeu de données labelisées d'opérations en ligne frauduleuses, de prédire une future opération de fraude grâce à des algorythme de machine learning supervisés.

Il s'appuie sur deux jeux de données disponnibles dans le dossier data.

## Sommaire

  - [Dataset](#Dataset)
  - [Set up](#SetUp)


## Dataset

Ce dossier contient les deux fichiers utilisés pour le projet. 

### Fraud_Data.csv

Ce fichier csv contient les champs suivants : 

  - user_id : identifiant de l'utilisateur
  - signup_time : heure à laquelle l'utilisateur s'est connecté
  - purchase_time :heure à laquelle l'utilisateur à fait l'achat
  - purchase_value : montant de l'achat
  - device_id : identifiant du moyen par lequel l'utilisateur s'est connecté 
  - source : moyen parlequel l'utilisateur est arrivé sur le site
  - browser : navigateur utilisé 
  - sex : sexe
  - age : âge
  - ip_address : adresse IP
  - class : variable cible (0 : opération normale , 1 : opération frauduleuse)
  
### IpAddress_to_country.csv
Ce fichier csv permet d'associer un pays à une adresse IP via des intervalles (borne supérieure et inferieure des adresses IP).

Il contient les champs suivants : 

  - lower_bound_ip_address : borne inférieure de l'intervalle
  - upper_bound_ip_address : borne supérieur de l'intervalle
  - country : pays associé aux adresses IP se situant dans cet intervalle

## SetUp

Ce projet a été codé en python, et utilise différentes librairies :

  - Pandas : gestion des datasets
  - MatplotLib et Seaborn : librairies liées à la datavisualisation
  - Sklearn : librairie pour les algorythmes de ML

# Installation des librairies

Si vous voulez runner le code en local vous aurez donc besoin d'installer les librairies suivantes avec pip via l'invite de commande de votre machine  :

    pip install pandas
    
    pip install seaborn

    pip install matplotlib
    
    pip install sklearn
