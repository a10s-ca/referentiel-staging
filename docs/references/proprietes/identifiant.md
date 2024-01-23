# Identifiant

| Propriété | Description | Cardinalité | Cardinalité | Type |
| ------------ | ------------- | ------------ | ------------ |------------ |
| Type | Type d'identifiant utilisé. Dans la mesure du possible, il est suggéré d'utiliser des URI comme identifiants, en spécifiant la valeur `uri` pour le type, et l'URI complet comme valeur. Lorsque ce n'est pas possible, l'approche préconisée par Schema.org est utilisée: type doit correspondre à l'identification dont l'usage est le plus fréquent pour le système d'identification, tout en minuscules.<br><br>Il est entendu que les types d'identifiants seront différents selon la classe décrite. Par exemple, le type d'identifiant ISNI s'applique bien aux contributeurs mais pas aux spectacles. | 1 | 1 | Texte court |
| Valeur | L'identifiant lui-même. | 1 | 1 | Texte court |
