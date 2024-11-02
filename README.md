Tutoriel sur la Normalisation
Ce projet a été réalisé dans le cadre de mon cours universitaire pour aider à comprendre le concept de normalisation dans les bases de données. Il couvre les principes de normalisation, les différentes formes normales, et l'importance de structurer les données de manière efficace pour optimiser les performances et garantir l'intégrité des informations.

# Normalisation des Tables - Étapes

Ce document décrit les étapes de normalisation pour organiser les tables de données et minimiser les anomalies et redondances.

## Étapes de Normalisation

### 1ère forme normale (1NF)
1. **Vérification de la 1NF** : Chaque cellule de la table doit contenir une valeur atomique (indivisible).
2. **Énumération des attributs** : Listez tous les attributs de la table de départ.
3. **Définition de la table de départ** : Identifiez la table de base sur laquelle la normalisation va être appliquée.
4. **Identification des clés candidates** : Trouvez les ensembles d'attributs uniques pouvant identifier les lignes de la table.
5. **Détermination de la clé primaire** : Choisissez la clé primaire parmi les clés candidates ; les autres clés candidates deviennent des clés alternatives.

### De la 1NF à la 2ème forme normale (2NF)
1. **Identification des dépendances partielles** : Repérez les attributs qui dépendent uniquement d'une partie de la clé primaire (si celle-ci est composée).
2. **Création de nouvelles relations** : Supprimez les dépendances partielles en créant de nouvelles tables pour assurer que tous les attributs dépendent entièrement de la clé primaire.

### De la 2NF à la 3ème forme normale (3NF)
1. **Identification des dépendances fonctionnelles** : Déterminez les dépendances fonctionnelles et les clés primaires de chaque table.
2. **Élimination des dépendances transitives** : Pour chaque table, identifiez les dépendances transitives par rapport à la clé primaire et supprimez-les en créant des tables supplémentaires.

### Boyce-Codd Normal Form (BCNF)
1. **Vérification de la 3NF** : Assurez-vous que la table est en 3NF.
2. **Identification des déterminants** : Pour chaque table, identifiez les déterminants qui ne sont pas des clés candidates et qui risquent de créer des anomalies. Placez alors les attributs dépendants dans une nouvelle table avec le déterminant.

### 4ème forme normale (4NF)
1. **Vérification de la BCNF** : La table doit être en BCNF avant de passer à la 4NF.
2. **Élimination des dépendances multivaluées** : Identifiez et supprimez les dépendances multivaluées en les plaçant dans des tables séparées pour éviter les redondances.

Ces étapes permettent de structurer la base de données de manière optimale, en réduisant les anomalies et les redondances, et en facilitant la gestion des données.
