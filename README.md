# RESTaurantAPI

# Application Node.js avec Express et MySQL

Ceci est une application Node.js simple qui utilise Express pour créer une API restaurant et utilise MySQL comme base de données. L'API gère les opérations CRUD (Create, Read, Update, Delete) pour les tables suivantes : "items", "catégories" et "formules".

## Configuration

1. Assurez-vous d'avoir Node.js et MySQLWorkBench installés sur votre ordinateur.
2. Clonez ce dépôt ou téléchargez le code source.

## Installation

$assurez-vous d'installer les dépendances nécessaires en exécutant la commande suivante à la racine du projet : ```npm install```
Cela installera les packages requis répertoriés dans le fichier package.json.

## Configuration de la base de données

1. Créez une base de données MySQL appelée "Restaurantsql".
2. Configurez les informations de connexion à la base de données dans votre fichier `fichier.js` :

```javascript
const connection = mysql.createConnection({
    host: 'localhost', 
    user: 'root',
    password: 'Ethan33380',
    database: 'Restaurantsql'
});
```
Démarrage de l'application

Exécutez node ```fichier.js``` dans le terminal pour démarrer le serveur Express.
L'application sera accessible à l'adresse http://localhost:3000.


## Utilisation de l'API

### Table "items"
GET :/items Récupère tous les éléments (peut être filtré avec des paramètres).
GET :/items/id_items Récupère un élément par son ID.
POST :/items Crée un nouvel élément.
PUT :/items/id Met à jour un élément.
DELETE :/items/id_items Supprime un élément.

### Table "categories"
GET :/categories Récupère toutes les catégories avec les éléments associés.
GET :/categories/id_cate Récupère une catégorie par son ID avec les éléments associés.
POST :/categories Crée une nouvelle catégorie.
PUT :/categories/cate_id Met à jour une catégorie.
DELETE :/categories/cate_id Supprime une catégorie.

### Table "formulas"
GET :/formulas Récupère toutes les formules (peut être filtré avec des paramètres).
GET :/formulas/id Récupère une formule par son ID.
POST :/formulas Crée une nouvelle formule.
PUT :/formulas/id Met à jour une formule.
DELETE :/formulas/id Supprime une formule.
Exemples de requêtes

Vous pouvez utiliser des outils comme Postman pour tester les différentes routes de l'API et les visualiser clairement.

