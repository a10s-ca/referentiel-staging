# Structure et relations

Le référentiel propose l'utilisation de [classes principales](./classes_principales.md) et de [classes utilitaires](./classes_utilitaires.md) pour structurer les données.

Les relations entre les classes principales sont illustrées dans le schéma suivant. Les classes utilitaires sont volontairement omises.

!!! note
    Ce n'est pas le bon diagramme, je voulais juste tester le plugin pour faire des graphiques...


``` mermaid
erDiagram
    CUSTOMER ||--o{ ORDER : places
    ORDER ||--|{ LINE-ITEM : contains
    CUSTOMER }|..|{ DELIVERY-ADDRESS : uses
```
