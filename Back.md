# Lexique lié au Back dans le Developpement web

---

<h2 align="center">BACK</h2>

---

### API 

 *Application Programming Interface* ou *Interface de Programmation d'Application*
 
 C'est une interface logicielle qui permet à deux applications distinctes de communiquer entre elles et d'échanger des données. Peuvent être gratuites ou payantes. 
 
 **Les types** : 
 
 *API publique* => ouvert et disponible pour tous.
 
 *API Partenaires* => uniquement disponible pour des développeurs externes ou consommateurs d'API spécifiquement triés et autorisés. Dispose de droits et licences pour accéder à ces interfaces avec une sécurité plus robuste.
 
 *API Interne* => uniquement au sein de l'entreprise pour connecter les systèmes et des données. Aucune exposition publique.
 
 *API Composite* =>  combinaison de deux ou plusieurs Interface. Sert à établir des séquences d'opérations connexes ou interdépendantes. Utile pour traiter des comportements complexes ou liés et peut améliorer la vitesse et les performances par rapport aux API individuelles.

 ---

### REST 

Ensemble de contraintes architecturales. Approche la plus populaire pour construire une API. L'information est généralement transmise en JSON (lisible par l'homme et la machine).

 **Critère d'une API RESTful** : 
 -  S'appuie sur une architecture client-serveur (séparation front-back de l'API) avec requête via HTTP.
 
 - Communications *stateless* => information client jamais stockée entre les requêtes GET, traitées séparément et indépendamment.

 - Possibilité de mettre en cache des données = rationaliser les interactions client-serveur.

 - Interface uniforme entre les composants permettant un transfert standardisé des informations, c'est-à-dire : 
   - Ressources demandées identifiables et séparées des représentations envoyées au client. 
   - Ressources peuvent être manipulées par le client via la représentation reçue (contient suffisamment d'informations). 
   - Message autodescriptif renvoyé au client avec assez de détails pour décrire comment traiter les informations. 
   - API possède un hypertexte/hypermédia pour permettre au client d'utiliser des hyperliens afin de connaître toutes les autres actions disponibles.
  
 - Système à couches (invisible au client) mais permet de hiérarchiser les différents types de serveurs impliqués dans la récupération des informations demandées. 

 - Possible d'envoyer du code exécutable du serveur vers le client (si demande) afin d'étendre les fonctionnalités.

**Avantages** : rapide, légère et évolutive. 

**Différence** : SOAP

Source : [RedHat](https://www.redhat.com/fr/topics/api/what-is-a-rest-api)

---

### CRUD

*Create, Read, Update, Delete*

Moyen mnémotechnique pour les quatre fonctions de base de la gestion sur des données stockées.

Parfois appelé SCRUD => S pour Search

**SQL** => INSERT (create), SELECT(read), UPDATE (update), DELETE (delete)

**HTTP** => GET et POST (create), GET (read), PUT et PATCH (update), DELETE (delete)

Source : [Wikipedia](https://fr.wikipedia.org/wiki/CRUD)

---

### ORM

*Object-relational mapping* ou *mapping objet-relationnel*

Ensemble de classes permettant de manipuler les tables d'une base de donnéees relationnelle comme s'il s'agissait d'objet.

Donne l'illusion de ne plus travailler avec des requêtes mais avec des manipulations d'objets.

<div style="background-color : white;">

  ![ORM Schéma](https://res.cloudinary.com/practicaldev/image/fetch/s--QPH4sf2X--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/divzbwhf4hgov8ho911v.png)

</div>

Sources : [Linkedin](https://www.linkedin.com/posts/honorablecon_sundayword-activity-6878386656462823424-5jGs/?utm_source=linkedin_share&utm_medium=member_desktop_web)

---

### Doctrine

Il s'agit d'un ORM. 

Par défaut il est l'ORM du framework Symfony.

Permet de représenter les données de leur base de données relationnelle (comme MySQL, PostgreSQL, etc.) sous forme d'objets PHP.

Doctrine se charge de la conversion entre ces objets et les données stockées dans la base de données.

Se compose en deux parties :

- Doctrine [ORM](https://github.com/Floriane-MAFFEI/Lexique-Dev/blob/master/Back.md#ORM)
- Doctrine [DBAL](https://github.com/Floriane-MAFFEI/Lexique-Dev/blob/master/Back.md#DBAL)
  - s'appuie sur  [PDO](https://github.com/Floriane-MAFFEI/Lexique-Dev/blob/master/Back.md#PDO)

**Avantages** : 

- Facilite le developpement
- Code plus lisible
- Code plus maintenable
- Code plus portable

--- 

### PDO

*PHP Data Object*

Interface objet permettant d'accéder à une base de donnée en PHP. 
Elève le niveau de sécurité (requête préparée par exemple).

Agit comme une couche d'abstraction de base de données pour les applications web PHP. Elle fournit une interface uniforme pour interagir avec différentes bases de données (comme MySQL, PostgreSQL, SQLite, etc.) sans avoir à écrire du code spécifique à chaque système de gestion de base de données.

**Avantages** :

- Exécution des opérations sur la BDD, Récupération des données et Gestion des erreurs => plus efficace et plus sécurisé
- Code plus portable
- Amélioration de la sécurité (requêtes préparées => evite les injections SQL)

---

### DBAL

*Database Abstraction Layer*

Se positionne au-dessus de PDO.

Intermédiaire entre l'application web et la base de données sous-jacente, facilitant ainsi la communication et la manipulation des données.

Permet de travailler avec différentes bases de données (comme MySQL, PostgreSQL, SQLite, etc.) sans avoir à se soucier des détails spécifiques de chaque système.

Peut être utilisé indépendamment du Doctrine ORM.

**Avantages** : 
- Code plus portable
- réduit les dépendances à une BDD 
  - Projet plus flexible
  - Plus facile à maintenir