# Composantes du référentiel

Le référentiel des métadonnées descriptives du spectacle contient trois composantes principales :

## 1. Classes et relations

**Les classes et les relations** sont la base de la modélisation, les grands traits. Les classes correspondent aux concepts généraux qui doivent être décrits. Les relations indiquent comment ces classes sont liées entre elles.

*Exemple : La classe Représentation est liée à la classe Spectacle, et ce lien est une relation qui indique qu’une représentation est toujours associée à un et un seul spectacle, alors qu’un spectacle peut avoir aucune, une ou plusieurs représentations.*

## 2. Propriétés

**Les propriétés** complètent les classes, pour permettre une description détaillée des concepts concernés. Chaque propriété a un nom, et des règles dictant la façon d’en préciser la valeur.

*Exemple : La classe Représentation a une propriété Date, qui sert à indiquer la date et l’heure de la représentation. Le référentiel indique qu’il faut utiliser le format ISO-8601 pour représenter la date de façon précise et interopérable.*

De façon générale, les règles mentionnées dans le référentiel sont associées au format et à la représentation des données, et pas à des règles d’affaires, conformément aux lignes directrices mentionnées précédemment.

Une propriété peut parfois correspondre à une relation.

*Exemple : La classe Représentation a une propriété Lieu, qui est une relation vers un objet de la classe Lieu, servant à indiquer à quel endroit se tient la représentation.*

## 3. Vocabulaires contrôlés

**Les vocabulaires contrôlés** servent à indiquer, pour certaines propriétés, des valeurs normalisées, compréhensibles par plusieurs systèmes. Il s’agit essentiellement de standardiser des façons de décrire des réalités. Par exemple, pour exprimer l’état d’une représentation annulée, différents systèmes pourraient choisir des valeurs différentes: «Annulé», «cancellé», «canceled», «x-event-cncl»… Le référentiel propose d’utiliser des vocabulaires contrôlés déjà en usage dans le milieu du web ou du spectacle lorsque c’est possible. Des explications supplémentaires sur les vocabulaires contrôlés seront présentées plus loin, dans la section qui leur est consacrée.
