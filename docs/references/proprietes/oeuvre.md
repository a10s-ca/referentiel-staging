---
iucd: true
---

{%- import '/utils.md' as utils -%}

# Oeuvre

{% include '/references/proprietes/info_classes_principales.md' %}

=== "Affichage condensé"

    | Propriété | Description | Priorité | Cardinalité | Type |
    | ------------ | ------------- | ------------ | ------------ |------------ |
    | Identifiants | Énumération des identifiants connus. | Obligatoire | 1..N | Objets de la classe utilitaire Identifiant |
    | Nom | Nom de l'oeuvre | Obligatoire | 1 | Texte court multilingue |

=== "Affichage étendu"

    | Propriété | Description | Priorité | Cardinalité | Type |
    | ------------ | ------------- | ------------ | ------------ |------------ |
    | Identifiants | Énumération des identifiants connus. | Obligatoire | 1..N | Objets de la classe utilitaire Identifiant |
    {% include '/references/proprietes/identifiant_inc.md' %}
    | Nom | Nom de l'oeuvre | Obligatoire | 1 | Texte court multilingue |
