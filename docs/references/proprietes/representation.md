---
iucd: true
---

{%- import '/utils.md' as utils -%}

# Représentation

{% include '/references/proprietes/info_classes_principales.md' %}

=== "Affichage condensé"

    | Propriété | Description | Priorité | Cardinalité | Type |
    | ------------ | ------------- | ------------ | ------------ |------------ |
    | Identifiants | Énumération des identifiants connus. | Obligatoire | 1..N | Objets de la classe utilitaire [Identifiant](./identifiant.md) |
    | Spectacle | Identification du spectacle dont fait partie la représentation. | Obligatoire | 1 | Objet de la classe [Spectacle](./spectacle.md) |
    | Série | Identification des séries desquelles fait partie le spectacle | Optionnel | 0..N | Objets de la classe [Série](./serie.md) |
    | Début | Date et heure de début de la représentation | Obligatoire | 1 | Date et heure |
    | Fin | Date et heure de fin de la représentation | Optionnel | 0..1 | Date et heure |
    | Durée | Durée de la représentation. | Optionnel | 0..1 | Durée |
    | Devait précédemment débuter | Date et heure de début initialement prévus pour la représentation, dans le cas où il s'agit d'une représentation reportée. | Optionnel | 0..1 | Date et heure |
    | Entracte | Indique la présence d'une ou plusieurs entractes. | Optionnel | 0..1 | Booléen |
    | Supplémentaire | Indique que la représentation est une supplémentaires | Optionnel | 0..1 | Booléen |
    | Description | Propriété utilisée seulement si la description de la représentation est différente de celle du spectacle. Si elle est identique, il est recommandé de ne pas utiliser cette propriété. Les consignes d'utilisation de la classe [Spectacle](./spectacle.md) s'appliquent. | Optionnel | 0..1 | Texte long multilingue |
    | Description courte | Propriété utilisée seulement si la description courte de la représentation est différente de celle du spectacle. Si elle est identique, il est recommandé de ne pas utiliser cette propriété. Les consignes d'utilisation de la classe [Spectacle](./spectacle.md) s'appliquent. | Optionnel | 0..1 | Texte long multilingue |
    | Médias | Éléments médiatiques (photo, audio, audiovidéo, articles, documents...) supplémentaires associés à la représentation, lorsqu'ils sont disponibles et qu'il n'est pas possible de les associer au spectacle. Les consignes d'utilisation de la classe [Spectacle](./spectacle.md) s'appliquent. | Optionnel | 0..N | Objet de la classe utilitaire [Média](./media.md) |
    | Autre nom | Propriété utilisée seulement si l'autre nom de la représentation est différente de celle du spectacle. Si elle est identique, il est recommandé de ne pas utiliser cette propriété. Les consignes d'utilisation de la classe [Spectacle](./spectacle.md)] s'appliquent. | Optionnel | 0..1 | Texte court multilingue |
    | URL | Propriété utilisée seulement si l'URL associée à la représentation est différente de celle du spectacle. Ne pas confondre à l'URL de billetterie de la section concernant les offres. Les consignes d'utilisation de la classe [Spectacle](./spectacle.md) s'appliquent. | Optionnel | 0..1 | Texte court multilingue |
    | Contributions supplémentaires | Contributions à la représentation qui ne sont pas documentées dans le spectacle. Les contributions de la représentation sont donc l'ajout des contributions du spectacle et des contributions supplémentaires, desquelles ont retire les contributions retirées. | Optionnel | 0..N | Objets de la classe [Contribution](./contribution.md). |
    | Contributions retirées | Contributions documentées dans le spectacle qui ne s'appliquent pas à la représentation. Les contributions de la représentation sont donc l'ajout des contributions du spectacle et des contributions supplémentaires, desquelles ont retire les contributions retirées. | Optionnel | 0..N | Objets de la classe [Contribution](./contribution.md). |
    | Offres | Description des différentes modalités pour assister à la représentation. Il peut y avoir des modalités pour le présentiel et/ou le virtuel. Les modalités pour le présentiel et le virtuel doivent être documentées pour un spectacle hybride. Une représentation contient donc au maximum deux offres. | Obligatoire | 1..2 | Objets de la classe utilitaire [Offre](./offre.md) |

=== "Affichage étendu"

    | Propriété | Description | Priorité | Cardinalité | Type |
    | ------------ | ------------- | ------------ | ------------ |------------ |
    | Identifiants | Énumération des identifiants connus. | Obligatoire | 1..N | Objets de la classe utilitaire [Identifiant](./identifiant.md) |
    {% include '/references/proprietes/identifiant_inc.md' %}
    | Spectacle | Identification du spectacle dont fait partie la représentation. | Obligatoire | 1 | Objet de la classe [Spectacle](./spectacle.md) |
    | Série | Identification des séries desquelles fait partie le spectacle | Optionnel | 0..N | Objets de la classe [Série](./serie.md) |
    | Début | Date et heure de début de la représentation | Obligatoire | 1 | Date et heure |
    | Fin | Date et heure de fin de la représentation | Optionnel | 0..1 | Date et heure |
    | Durée | Durée de la représentation. | Optionnel | 0..1 | Durée |
    | Devait précédemment débuter | Date et heure de début initialement prévus pour la représentation, dans le cas où il s'agit d'une représentation reportée. | Optionnel | 0..1 | Date et heure |
    | Entracte | Indique la présence d'une ou plusieurs entractes. | Optionnel | 0..1 | Booléen |
    | Supplémentaire | Indique que la représentation est une supplémentaires | Optionnel | 0..1 | Booléen |
    | Description | Propriété utilisée seulement si la description de la représentation est différente de celle du spectacle. Si elle est identique, il est recommandé de ne pas utiliser cette propriété. Les consignes d'utilisation de la classe [Spectacle](./spectacle.md) s'appliquent. | Optionnel | 0..1 | Texte long multilingue |
    | Description courte | Propriété utilisée seulement si la description courte de la représentation est différente de celle du spectacle. Si elle est identique, il est recommandé de ne pas utiliser cette propriété. Les consignes d'utilisation de la classe [Spectacle](./spectacle.md) s'appliquent. | Optionnel | 0..1 | Texte long multilingue |
    | Médias | Éléments médiatiques (photo, audio, audiovidéo, articles, documents...) supplémentaires associés à la représentation, lorsqu'ils sont disponibles et qu'il n'est pas possible de les associer au spectacle. Les consignes d'utilisation de la classe [Spectacle](./spectacle.md) s'appliquent. | Optionnel | 0..N | Objet de la classe utilitaire [Média](./media.md) |
    {% include '/references/proprietes/media_inc.md' %}
    | Autre nom | Propriété utilisée seulement si l'autre nom de la représentation est différente de celle du spectacle. Si elle est identique, il est recommandé de ne pas utiliser cette propriété. Les consignes d'utilisation de la classe [Spectacle](./spectacle.md)] s'appliquent. | Optionnel | 0..1 | Texte court multilingue |
    | URL | Propriété utilisée seulement si l'URL associée à la représentation est différente de celle du spectacle. Ne pas confondre à l'URL de billetterie de la section concernant les offres. Les consignes d'utilisation de la classe [Spectacle](./spectacle.md) s'appliquent. | Optionnel | 0..1 | Texte court multilingue |
    | Contributions supplémentaires | Contributions à la représentation qui ne sont pas documentées dans le spectacle. Les contributions de la représentation sont donc l'ajout des contributions du spectacle et des contributions supplémentaires, desquelles ont retire les contributions retirées. | Optionnel | 0..N | Objets de la classe [Contribution](./contribution.md). |
    {% include '/references/proprietes/contribution_inc.md' %}
    | Contributions retirées | Contributions documentées dans le spectacle qui ne s'appliquent pas à la représentation. Les contributions de la représentation sont donc l'ajout des contributions du spectacle et des contributions supplémentaires, desquelles ont retire les contributions retirées. | Optionnel | 0..N | Objets de la classe [Contribution](./contribution.md). |
    {% include '/references/proprietes/contribution_inc.md' %}
    | Offres | Description des différentes modalités pour assister à la représentation. Il peut y avoir des modalités pour le présentiel et/ou le virtuel. Les modalités pour le présentiel et le virtuel doivent être documentées pour un spectacle hybride. Une représentation contient donc au maximum deux offres. | Obligatoire | 1..2 | Objets de la classe utilitaire [Offre](./offre.md) |
    {% include '/references/proprietes/offre_inc.md' %}
