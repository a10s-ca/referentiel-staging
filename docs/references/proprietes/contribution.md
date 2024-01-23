# Contribution

| Propriété | Description | Priorité | Cardinalité | Type |
| ------------ | ------------- | ------------ | ------------ |------------ |
| Types | Identification du type de contribution.  | Obligatoire | 1..N | Termes d'un vocabulaire contrôlé de type de contribution |
| Type principal | Préavis: cette propriété pourrait être intégrée dans une future version du référentiel, et imposer un vocabulaire contrôlé. | Ne pas utiliser | 1 | À déterminer |
| Contributeur | Identification du contributeur. | Obligatoire | 1 | Objet de la classe Contributeur |
| Numéro de séquence | Précision sur l'ordre de présentation des contributions (les nombres plus petits correspondent à des contributions qui doivent être présentées en premier). | Optionnel | 1 | Nombre |
| Note | Note concernant la contribution, à l'intention des exploitants des systèmes d'information (et donc pas du grand public). Il peut s'agir d'une précision sur le type de contribution, qui ne pourrait pas être exprimée à travers la propriété Types. Les informations compilées dans les notes pourraient être utilisées pour améliorer les vocabulaires contrôllés. | Optionnel | 1 | Texte court |
