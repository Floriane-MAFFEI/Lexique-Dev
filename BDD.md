# Lexique lié au Base de donnée (BDD) dans le Developpement web

---

<h2 align="center">BASE DE DONNEE (BDD)</h2>

---

### Clé primaire

Contrainte d'unicité, composée d'une ou plusieurs colonnes, et qui permet d'identifier de manière unique chaque ligne de la table.

 --- 

 ### Clé étrangère

Permet de gérer des relations entre plusieurs tables, et garantit la cohérence des données.

Permet d'accéder au parent d'une relation.

Doit correspondre à la structure de la clé primaire de la table parent ou cible.


--- 

### Clé secondaire

Permet d'accéder à un ou plusieurs éléments de la table. 

C'est un index qui n'est ni unique ni obligatoire.

---

### SGBD

*Système de Gestion de Base de Données*

Logiciel permettant aux utilisateurs et programmeurs de créer et de gérer des bases de Données.

Par exemple : MariaDB (relationnel), MySQL (relationnel), MongoDB (orienté Document), PostgreSQL (Relationnel et objet (mélange des approche relationnel et objet)), etc

Sans SGBD impossible d'administrer, commander ou controler une base de données.

---

### Types de données


*Donnée numérique*
| Nature    | Type      | UNSIGNED              | SIGNED                               | Taille (octet) |
| --------- | --------- | --------------------- | ------------------------------------ | -------------- |
| Entiers   | TINYINT   | [0 à 255]             | [-128 à 127]                         | 1              |
| Entiers   | SMALLINT  | [0 à 65,535]          | [-32,768 à 32,767]                   | 2              |
| Entiers   | MEDIUMINT | [0 à 16,777,215]      | [-8,388,608 à 8,388,607]             | 3              |
| Entiers   | INT       | [0 à 4,294,967,295]   | [-2,147,483,648 à 2,147,483,647]     | 4              |
| Entiers   | BIGINT    | [0 à (2^64 - 1)]      | [-2^63 à (2^63 - 1)]                 | 8              |
| Flottants | FLOAT     | [0 à 3.402823466E+38] | [-1.175494351E-38 à 3.402823466E+38] | 4              |

*Type caractère*

| Nature de la donnée      | Type SQL | Note                                                                                                                 | Taille (octet)                   |
| ------------------------ | -------- | -------------------------------------------------------------------------------------------------------------------- | -------------------------------- |
| Chaîne de caractères     | VARCHAR  | Peut contenir jusqu’à 65,535 caractères (ou moins si encodage des caractères sur plusieurs octets : 21,844 en UTF-8) | Longeur de la chaîne maximum + 1 |
| Chaîne de caractères     | CHAR     | Maximum de 255 caractères                                                                                            | Longueur de la chaîne            |
| Chaîne de caractères     | TEXT     | Chaînes de 65,535 caractères, sensible à la casse                                                                    | Longueur + 2                     |
| Chaîne binaire (séquence | BLOB     | 65,535 caractères, insensible à la casse                                                                             | Longueur + 1 d’octets)           |

*Type date*

| Nature            | Type      | Note                                         | Taille (octet)                     |
| ----------------- | --------- | -------------------------------------------- | ---------------------------------- |
| Date au format AAAA-MM-JJ     | DATE      | De 1000-01-01 à 9999-12-31       | 3                                  |
| Date et heure au format AAAA-MM-JJ HH:MM:SS  | DATETIME  | De 1000-01-01 00:00:00 à 9999-12-31 23:59:59 | 8                                 |
| Heure au format HH:MM:SS   | TIME      | De -838:59:59 à 838:59:59                    | 3                                  |
| Année à 2 ou 4 chiffres   | YEAR      | De 1901 à 2155 ou 0000 (4 chiffres)          | 1                                  |
| Date sous forme numérique  | TIMESTAMP | Commence le 1970-01-01 00:00:00              | 4 (peut varier selon la précision) |

*Autres types*


| Nom            | Taille de stockage      | Descritpion                                         | Etendue              |
| ----------------- | --------- | -------------------------------------------- | ---------------------------------- |
| money     | 8 octets      | Montant monétaire       | -92233720368547758.08 à +92233720368547758.07                                  |
| boolean     | 1 octet      | Booléen (Vrai/Faux)       | Sont considéré comme "vrai" : TRUE, 't', 'true', 'y', 'yes', 'on', '1'                                  |
| json     |      | Données texte JSON        |                   |

Source : [Doc PostgreSQL](https://webusers.i3s.unice.fr/~rueher/Cours/BD/DocPostgresSQL9-5_HTML/datatype.html#datatype-numeric)




