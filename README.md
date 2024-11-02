Tutoriel sur la Normalisation
Ce projet a été réalisé dans le cadre de mon cours universitaire pour aider à comprendre le concept de normalisation dans les bases de données. Il couvre les principes de normalisation, les différentes formes normales, et l'importance de structurer les données de manière efficace pour optimiser les performances et garantir l'intégrité des informations.


Normalisation des tables - Étapes
Pour atteindre la 1ère forme normale (1NF)
Vérification de la 1NF : Assurez-vous que chaque cellule de la table contient une valeur atomique (indivisible).
Énumération des attributs : Listez tous les attributs de la table de départ.
Définition de la table de départ : Identifiez la table de base sur laquelle la normalisation va être appliquée.
Identification des clés candidates : Trouvez les ensembles d'attributs uniques qui peuvent identifier les lignes de la table.
Détermination de la clé primaire : Choisissez la clé primaire parmi les clés candidates ; les autres clés candidates deviennent des clés alternatives.
De la 1NF à la 2ème forme normale (2NF)
Identification des dépendances partielles : Repérez les attributs qui dépendent uniquement d'une partie de la clé primaire (si celle-ci est composée).
Création de nouvelles relations : Supprimez les dépendances partielles en créant de nouvelles tables pour assurer que tous les attributs dépendent entièrement de la clé primaire.
De la 2NF à la 3ème forme normale (3NF)
Identification des dépendances fonctionnelles : Déterminez les dépendances fonctionnelles et les clés primaires de chaque table.
Élimination des dépendances transitives : Pour chaque table, identifiez les dépendances transitives par rapport à la clé primaire et supprimez-les en créant des tables supplémentaires.
Boyce-Codd Normal Form (BCNF)
Vérification de la 3NF : Assurez-vous que la table est en 3NF.
Identification des déterminants : Pour chaque table, identifiez les déterminants qui ne sont pas des clés candidates et qui risquent de créer des anomalies. Placez alors les attributs dépendants dans une nouvelle table avec le déterminant.
Pour atteindre la 4ème forme normale (4NF)
Vérification de la BCNF : La table doit être en BCNF avant de passer à la 4NF.
Élimination des dépendances multivaluées : Identifiez et supprimez les dépendances multivaluées en les plaçant dans des tables séparées pour éviter les redondances.
