# Structure et relations

Le référentiel propose l'utilisation de [classes principales](./classes_principales.md) et de [classes utilitaires](./classes_utilitaires.md) pour structurer les données.

Les relations entre les classes principales sont illustrées dans le schéma suivant. Les classes utilitaires sont volontairement omises.

``` mermaid
flowchart TD
    Représentation -- inclut la contribution de --> Contributeur
    Représentation -- dans le cadre de --> Spectacle
    Représentation -- peut faire partie de  --> Série
    Représentation -- se tient dans --> Lieu
    Représentation -- se tient dans --> Salle
    Salle -- située dans --> Lieu
    Spectacle -- inclut la contribution de --> Contributeur
    Spectacle -- associé à --> Oeuvre
    Série -- inclut la contribution de --> Contributeur
```
