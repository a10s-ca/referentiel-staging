# Terme

| Propriété | Description | Cardinalité | Cardinalité | Type |
| ------------ | ------------- | ------------ | ------------ |------------ |
| Vocabulaire | Identification du vocabulaire duquel est tiré le terme.<br><br>Typiquement, cette identification correspond à l'appellation du vocabulaire dont l'usage est le plus fréquent, tout en minuscules, sans accents, et avec les espaces remplacés par des barres de soulignement. | 1 | 1 | Texte court |
| Version | Version du vocabulaire utilisé, lorsque c'est applicable. | 1 | 1 | Texte court |
| Code | Identification du terme selon le vocabulaire identifié. En cas d'incohérence entre l'étiquette et le code transmis, c'est ce dernier qui doit être priorisé. | 1 | 1 | Texte court |
| Étiquette | Version textuelle du terme tiré du vocabulaire choisi. | 1 | 1 | Texte court multilingue |
| Numéro de séquence | Priorité d'utilisation du terme (les nombres plus petits représentant un niveau de priorité plus élevé). | 1 | 1 | Nombre |
