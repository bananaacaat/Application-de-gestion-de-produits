# TP Hibernate 

Dans ce repo vous allez trouver les solutions des exercices suivants:

- `H1`: l'exercice 1.
- `gestion_de_stock`: l'exercice 2.
- `gestion_de_projet`: l'exercice 3.
- `gestion_de_etat_civil`: le travail a faire 

## H1
Le projet H1 vise à créer une application de gestion de produits. Il comprend les fonctionnalités suivantes :

Création d'une entité Produit avec des annotations Hibernate.
Configuration de Hibernate via un fichier hibernate.cfg.xml.
Mise en place d'une classe HibernateUtil pour gérer la SessionFactory.
Création d'une interface IDao et d'une classe de service ProduitService.
Tests complets pour la création, la modification, la suppression et la recherche de produits.
Structure du Projet

### Structure du Projet
src/main/java/ma.projet.entity : Entité Produit.
src/main/java/ma.projet.config : Fichier de configuration Hibernate.
src/main/java/ma.projet.util : Classe HibernateUtil.
src/main/java/ma.projet.dao : Interface IDao.
src/main/java/ma.projet.service : Classe ProduitService.
src/test/java : Tests unitaires.

## Gestion de stock

### Objectif
Le projet Gestion de stock vise à mettre en place une application de gestion de projets. Il comprend les fonctionnalités suivantes :

Création de classes entités pour les projets, les tâches et les employés avec des annotations Hibernate.
Configuration de Hibernate via un fichier hibernate.cfg.xml.
Mise en place d'une classe HibernateUtil pour gérer la SessionFactory.
Création d'une interface générique IDao et de classes de service (ProjetService, TacheService, EmployeService, EmployeTacheService).
Implémentation de diverses méthodes pour gérer les projets, les tâches et les employés.
Tests complets pour vérifier le bon fonctionnement des fonctionnalités.

### Conception
![gestion_de_stock](https://github.com/bananaacaat/tp-hibernate/assets/147453939/28730a9d-11e6-464d-a695-cbec0ca57ced)


### Structure de Projet
src/main/java/ma.projet.classes : Entités pour les projets, les tâches et les employés.
src/main/java/ma.projet.config : Fichier de configuration Hibernate.
src/main/java/ma.projet.util : Classe HibernateUtil.
src/main/java/ma.projet.dao : Interface IDao.
src/main/java/ma.projet.service : Classes de service (ProjetService, TacheService, EmployeService, EmployeTacheService).
src/test/java : Tests unitaires.

## Gestion de projet

### Objectif
Le projet Gestion de projet vise à mettre en place une application de gestion de projets. Il comprend les fonctionnalités suivantes :

Création de classes entités pour les projets, les tâches et les employés avec des annotations Hibernate.
Configuration de Hibernate via un fichier hibernate.cfg.xml.
Mise en place d'une classe HibernateUtil pour gérer la SessionFactory.
Création d'une interface générique IDao et de classes de service (ProjetService, TacheService, EmployeService, EmployeTacheService).
Implémentation de diverses méthodes pour gérer les projets, les tâches et les employés.
Tests complets pour vérifier le bon fonctionnement des fonctionnalités.

### Conception
![gestion_de_projet](https://github.com/bananaacaat/tp-hibernate/assets/147453939/b4b53f44-026d-4c73-9582-cc468b0b7fdb)


### Structure du Projet
src/main/java/ma.projet.classes : Entités pour les projets, les tâches et les employés.
src/main/java/ma.projet.config : Fichier de configuration Hibernate.
src/main/java/ma.projet.util : Classe HibernateUtil.
src/main/java/ma.projet.dao : Interface IDao.
src/main/java/ma.projet.service : Classes de service (ProjetService, TacheService, EmployeService, EmployeTacheService).
src/test/java : Tests unitaires.


## Gestion d'etat civil

### Objectif
Le projet Tar vise à développer une application de gestion de l'état civil des citoyens d'une province. Il inclut les entités Personne, Femme, Homme, et Mariage, ainsi que des fonctionnalités pour la gestion des données relatives à l'état civil.

### Conception
![gestion_de_etat_civil](https://github.com/bananaacaat/tp-hibernate/assets/147453939/f3269430-ad14-4ec5-8c60-9b438572414b)

### Structure de Projet
#### Couche de Persistance
Classes Entités : Dans le package ma.projet.beans, les classes entités (Personne, Femme, Homme, Mariage) sont développées avec les annotations Hibernate appropriées. Les annotations Hibernate, telles que @Entity, @Id, @GeneratedValue, @Table, et autres, sont utilisées pour définir la structure des entités.

Configuration Hibernate : Un fichier de configuration hibernate.cfg.xml est créé dans le package ma.projet.config pour configurer Hibernate et définir les paramètres de connexion à la base de données MySQL.

Classe HibernateUtil : Une classe HibernateUtil est mise en place dans le package ma.projet.util pour gérer la SessionFactory de Hibernate.

Base de Données MySQL : La base de données est générée en utilisant les entités et les annotations définies dans le projet.

#### Couche Service
Une interface générique IDao<T> est créée dans le package ma.projet.dao.
Classes de Service : Trois classes de service sont mises en place : HommeService, FemmeService, et MariageService. Ces classes implémentent l'interface IDao et sont responsables de la gestion des données relatives aux hommes, femmes, et mariages.

Affichage des Épouses : Dans la classe HommeService, une méthode est créée pour afficher les épouses d'un homme passé en paramètre entre deux dates spécifiées.

Requête Native : Une requête native nommée est créée pour renvoyer le nombre d'enfants d'une femme donnée entre deux dates.

Utilisation de la Requête : Une méthode est ajoutée dans la classe FemmeService pour utiliser la requête native créée précédemment.

Requête Nommée pour les Mariages Multiples : Une requête nommée est créée pour renvoyer les femmes mariées deux fois ou plus.

## Comment Exécuter les Projets
Clonez ce référentiel sur votre ordinateur.
Configurez une base de données MySQL en conséquence (assurez-vous que les paramètres de base de données correspondent à ceux définis dans les fichiers de configuration Hibernate).
Importez les projets dans votre environnement de développement (par exemple, NetBeans).
Exécutez les projets individuellement en suivant les instructions spécifiques à chaque projet dans leurs répertoires respectifs.
Utilisez les tests unitaires pour vérifier le bon fonctionnement des fonctionnalités.

## Avertissement
Assurez-vous de respecter les dépendances et les prérequis nécessaires pour exécuter ces projets, notamment les bibliothèques Hibernate-JPA et le pilote MySQL.


