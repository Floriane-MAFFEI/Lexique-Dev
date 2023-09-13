# Lexique lié aux connaissances de base dans le Developpement web

---

<h2 align="center">CONNAISSANCES DE BASE</h2>

---

### Front-end

Partie visible du site web, celle avec laquelle les utilisateurs interagissent.

**Languages** : HTML, CSS, JavaScript, etc...

---

### Back-end

Partie invisible du site web pour les utilisateurs.

Gère l'authentification des utilisateurs, les sessions, les mots de passes chiffrés et d'autres aspects liés à la sécurité.

**Languages** : C#, Java, Python, PHP, Ruby, JS(Node.js)

---

### Back-office

Il s'agit de la partie invisible d'un site Internet ou d'un système informatique.

Elle permet à l'entreprise ou utilisateurs d'administrer et de gérer son site.

Le back-office propose généralement :

- Ajout de produits et/ou services
- Modification
- Administration
- Gestion des utilisateurs

**Opposé** : [Front-office]([htt](https://github.com/Floriane-MAFFEI/Lexique-Dev/blob/master/Connaissance-de-base.md#Front-office)) => partie dédiée à l'interaction avec l'utilisateur.

**En image** : Correspond à l'entrepôt, l'administration, etc...

Source : [Techno-science](https://www.techno-science.net/definition/10892.html)

---

### Front-office

Partie qui prend en charge l'interface d'une application.

**Opposé** : [Back-office]([htt](https://github.com/Floriane-MAFFEI/Lexique-Dev/blob/master/Connaissance-de-base.md#Back-office)) => partie dédiée à la gestion.

**En image** : Correspond à un magasin fréquenté par les clients

Source : [Techno-science](https://www.techno-science.net/definition/11021.html)

---

---

### CMS

*Content Mangement System* ou *Système de gestion de contenu*

Logiciel en ligne donnant la possibilité de créer, gérer et/ou modifier un site web sans avoir besoin de connaissance technique et en seulement quelques clics.

Il existe des : 

- **CMS custom** => créer sur mesure (*Avantages* : Uniquement constitué des modules utiles, plus simple)
- **CMS Open Source** => Accessible gratuitement pour la plupart.

**CMS Populaire** : Wordpress, Joomla, Shopify, Drupal

Source : [pure-illusion](https://www.pure-illusion.com/lexique/definition-de-cms)

---

### Frameworks

*=> ils disent aux développeurs quoi faire*

*Frame* = cadre
*Work* = travail

Boite à outils pour développeur web.

Contient des composants autonomes qui permettent de faciliter le développement d’un site web ou d’une application.

Résout souvent les problèmes rencontrés par les développeur (CRUD, Arborescence, normes, sécurité...)

Plus utilisé pour de gros projets.

**Avantages** : 

- Rend le développement plus rapide
- Facilite le déboggage
- Augmente la réutilisabilité du code 
- Adapté pour le travail en équipe ;
- Vient avec un ensemble de fonctionnalités (sécurité, cache, authentification, ORM, etc.).

**Inconvénients** : 

- On a une dépendance vis à vis des développeurs du frameworks (bugs, problèmes de compatibilité, failles, etc.)
- Peu flexible comparé à une bibliothèque
- Effet “usine à gaz” pour les petits projets
- On doit bien le choisir, pas de retour en arrière facile
- On doit faire de la veille et mettre à jour son code pour rester dans les versions à jour.

**Exemple de frameworks** : Angular, Symfony, Laravel, Django, Vue.JS, Semantic UI, Flutter, Ruby on Rails

Source : [FreelanceRepublik](https://talks.freelancerepublik.com/framework-bibliotheque-differences/#:~:text=Une%20librairie%20est%20plus%20flexible,'un%20(gros)%20projet.)

---

### Librairies (bibliothèque) 

*=> le dévéloppeur lui dit quoi faire*

Collection de routine (méthodes) pouvant être appelés par le code d'un développeur pour éxécuter des actions spécifiques.

Utilisé pour des petits projets ou éléments (formulaire, data picker...)

**Différences avec Frameworks** : Un Framework est composé de plusieurs bibliothèque.

**Avantages** : 

- Rend le développement plus rapide
- Permet d’écrire moins de code 
- Flexible au niveau de l’utilisation – elle ne cadre pas le développement tout entier comme un framework 
- Il est facile de créer soi-même une librairie.

**Inconvénients** :

- Risques d’incompatibilité entre différentes librairies, ou entre une librairie et la version d’un framework, etc. 
- Certaines librairies peuvent avoir des failles de sécurité 
- Empiler bibliothèque sur bibliothèque peut complexifier un projet.

**Exemple de libraires** : React JS, jQuery, Bootstrap, Tailwind

Source : [FreelanceRepublik](https://talks.freelancerepublik.com/framework-bibliotheque-differences/#:~:text=Une%20librairie%20est%20plus%20flexible,'un%20(gros)%20projet.)


--- 

### Dépendance

Cela fait référence aux bibliothèques, aux frameworks ou aux modules de code tiers qu'un projet web utilise pour fonctionner.

Ces éléments externes sont "dépendants" car le projet ne peut pas fonctionner sans eux.

---

### Token

*token Access* ou *jetons individuels*

Mécanisme fréquemment intégré au procédures d'authentification.

Le token permet une connexion sécurisée.

![Token function](https://www.okta.com/sites/default/files/styles/tinypng/public/media/image/2020-12/TokenBasedAuthentication.png?itok=zXMogDjG)

Source : [CNIL](https://www.cnil.fr/fr/les-jetons-individuels-de-connexion-ou-token-access)

---

### Client

Ordinateur ou application qui envoie des requêtes à un serveur.

---

### Serveur

Attends les requêtes des clients et y réponds.

=> Offre un service au client

![Client-Serveur](https://upload.wikimedia.org/wikipedia/commons/thumb/d/db/Mod%C3%A8le-client-serveur.svg/1024px-Mod%C3%A8le-client-serveur.svg.png)

Source : [Wikipedia](https://fr.wikipedia.org/wiki/Client-serveur)


---

### Chemin Relatif

```dossier\page.html```

La cible (page.html) va être cherchée par le navigateur à partir de la page html ou de la feuille de style qu'il interprète, dans le sous-répertoire "dossier".

```./dossier/page.html```
./ => signifie que la page est cherchée à partir du répertoire courant.

````../dossier/page.html```

../ => signifie que la page est cherchée à partir du répertoire parent (on remonte d'un niveau).


**Important** : En PHP, si on utilise la fonction ```include()``` => le chemin relatif part du fichier dans lequel est placé son contenu (fichier éxécuté par le serveur). En PHP, pour obtenir la racine du serveur web il faut tuilisez => ```$_SERVER['DOCUMENT_ROOT']```

**Exemple** => ```include('/inc/menu.php');``` équivaudrait à ```C:>inc\menu.php``` et non pas à ```http://www.domaine.fr/inc/menu.php``` qui n'est au fond qu'une vue "virtuelle" du répertoire qui héberge le site, et qui peut être placée n'importe où dans l'arborescence du système de stockage.

Source : [Alsacreations](https://www.alsacreations.com/astuce/lire/78-quelle-est-la-diffrence-entre-les-chemins-relatifs-et-absolus.html)

---

### Chemin absolu

```\dossier\page.html```

Le slash intial précise que l'on ne se réfère plus à l'emplacement courant mais que l'on remonte à la racine puis on précise ensuite le chemin complet.

---

### Callback

*Fonction de rappel*

Fonction passée dans une autre fonction en tant qu'argument.
Peut alors être exécutée ultérieurement, souvent en réponse à un événement spécifique, comme le chargement d'une page web ou la fin d'une opération asynchrone.

**Utilisations** : gére des tâches telles que la manipulation de données après leur chargement depuis un serveur ou la réaction à des actions de l'utilisateur sur une page web.

**Avantages** :  permet un traitement non bloquant et réactif dans le développement web.

Source : [Mdn](https://developer.mozilla.org/fr/docs/Glossary/Callback_function)

---

### JSON

*JavaScript Object Notation*

**Extension** : .json

Format de donnée textuel utilisé pour stocker et échanger des informations.

Il est basé sur une structure d'objets et de tableaux, et il est couramment utilisé pour transmettre des données entre un serveur et un client web, ainsi que pour configurer des applications web.

**Avantages** : 
- Facile à lire et à écrire
- Facile à analyser
- et Facile à générer pour les machines
  
**Concurrent** : XML

---

### Fonction

Bloc de code réutilisable qui effectue une tâche spécifique.

Elles accomplissent des actions ou des calculs.

Une fonction prend entre 0 et plusieurs paramètres et renvoie (return) toujours un résultat.

Peuvent être appelées (exécutées) à partir d'autres parties du code chaque fois qu'elle doit être exécutée.

**Avantages** : 
- Code plus modulaire
- Plus facile à maintenir
- Plus facile à organiser
- Evite les répétitions de code similaire
- Favorise la réutilisation du code

---

### Méthode

Fonction qui est associée à un objet ou à une classe.

Définit :
- les actions
- les opérations spécifiques que l'objet ou la classe peut effectuer

Elles sont appellé sur l'objet ou la classe pour déclencher l'action ou l'opération.

Existe : 
- *méthode d'instance* => représente les fonctions fournissant une interface pour effectuer des actions dans le contexte de l'objet qu'elles composent => agit que sur un objet à la fois
- *méthode statique* => représente les focntions pouvant être exécutée sans nécessiter d'instanciation

**Exemple de méthode** : constructeur, destructeur, getter, setter

**Portée des méthodes** : private, protected, public

Source : [Wikipédia](https://fr.wikipedia.org/wiki/M%C3%A9thode_(informatique))

---

### Variable

Eléments qui associent un nom (l'identifiant) à une valeur, qui sera implantée dans la mémoire du système programmé.

La variable peut prendre différentes valeurs au cours de l'exécution du programme.

Doit obligatoirement être déclarée.

Possible de lui assigner une valeur au moment de la déclaration.

**En JS** : elle se déclare via *let nomVariable* => permet de changer la valeur, *const nomVariable* => la valeur de la variable ne peux pas changer.

**En PHP** : elle se déclare en faisant $nom_variable

---

### Propriété

Elément de description d'un objet.

**Usage courant** : Rajouter des instructions appliquée systématiquement au moment de la modification ou de la lecture d'une instance d'une classe sans modification de cette classe.

**Egalement** : Contrôler l'accès aux champs (public, private)

**Important** : la valeur d'une propriété private ne pourra être modifier que via un [*setter*](#setter) et ces valeurs pourront être lu via un [*getter*](#getter) 

---

### Constante

Element de donnée associé à une valeur fixe

Syntaxiquement, elle ressemble à une variable

**Important** : On ne peut jamais modifier sa valeur et celle-ci doit donc être précisée lors de la définition de l'objet.

---

### Setter

Méthode qui permet de modifier la valeur d'une propriété private d'une classe.

---

### Getter

Méthode qui permet de lire la valeur d'une propriété private d'une classe.

---

### Handler

Procédure permettant d'effectuer un traitement après un event.

---

### Hook

Représente une actioon que l'on vient intercaler dans un traitement déjà défini pour faire un traitement "custom".