# Tableau du lexique de Developpeur web

---

<h2 align="center">ARCHITECTURE</h2>

---

### Design pattern

Élément essentiel en POO. Il s'agit d'une infrastructure faite d'une petite quantité de classes qui sert à régler un problème technique.

**Avantages** : Accélérer le processus de développement, gagner du temps, facilite la lisibilité du code.
= Se base sur des pratiques antérieures et sur les leçons apprises.

---

### MVC

Modèle-Vue-Contrôleur : nom d'une méthodologie visant à faire le lien entre l'interface utilisateur et les modèles de données.

**Avantages** : Très utile pour de la récupération de code objet, réduit le temps nécessaire au développement d'applications avec une interface utilisateur.

**Détail** :
*Modèle* => représente la structure logique des données dans l'application. Ne contient aucune information sur l'interface.
*Vue* => représente les éléments de l'interface utilisateur (partie visuelle).
*Contrôleur* => Représente les classes qui se connectent au Modèle et à la Vue, sert de communication entre les classes dans le modèle et la vue.

---

### Architecture

Élément clé de la conception d'un site efficace et fonctionnel.
Définit la manière (structure) dont un site est organisé et fonctionne.

Cela comprend : 
- La conception du site 
- L'organisation du site 
- La gestion de ses données
- La mise en place des interactions entre le site et ses utilisateurs.

**IMPORTANT** : Cela peut avoir un impact sur les performances, la sécurité, la maintenance et l'évolutivité...

L'architecture peut aussi faire référence à l'infrastructure technique (serveur, BDD, Langages, etc). |

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

