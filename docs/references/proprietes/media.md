# Média

| Propriété | Description | Priorité | Cardinalité | Type |
| ------------ | ------------- | ------------ | ------------ |------------ |
| Type | Identification du type de média. | Obligatoire | 1 | Mime type |
| Numéro de séquence | Priorité d'utilisation du média (les nombres plus petits représentant un niveau de priorité plus élevé). | Optionnel | 1 | Nombre |
| Notes d'usage | Texte libre permettant d'identifier les usages possibles du média (à l'intention des opérateurs des systèmes, pas du grand public, et donc pas pour publication). | Obligatoire | 1 | Texte court |
| URL | URL permettant d'obtenir le média. Il est suggéré de rendre disponibles les médias dans les formats standards du web, en haute résolution lorsque possible. | Obligatoire | 1 | URL |
| Licence | Licence d'utilisation du média. Une valeur vide ou non définie correspond à un média libre de droits. Si des conditions s'appliquent, elles doivent être définies dans cette propriété, ou sur le web à une URL intégrée dans cette propriété.<br><br>_Exemple 1: «Utilisation permise avec mention des crédits.»<br>Exemple 2: «https://creativecommons.org/licenses/by-nc-sa/4.0/»<br>Exemple 3: «Veuillez nous contacter à droits@domaine.com pour obtenir une licence d'utilisation.»_ | Obligatoire | 1 | Texte court |
| Crédits | Crédits associés au média. | Obligatoire | 0..1 | Texte court |
| Description | Description courte (pouvant par exemple servir de «alt description» sur le web). | Obligatoire | 0..1 | Texte court |
