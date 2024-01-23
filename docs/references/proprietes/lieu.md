# Lieu

| Propriété | Description | Cardinalité | Cardinalité | Type |
| ------------ | ------------- | ------------ | ------------ |------------ |
| Identifiants | Énumération des identifiants connus. | 1..N | 1..N | Objets de la classe utilitaire Identifiant |
| Nom | Nom du lieu, écrit au long, de la façon dont il doit être affiché à des utilisateurs, avec la capitalisation d'usage, les accents et les espacements usuels.<br><br>Éviter d'inclure le nom d'une salle spécifique dans le nom d'un lieu, sauf s'il s'agit du même nom.<br><br>_Exemple: «Grand Théâtre de Québec» sans la «Salle Louis-Fréchette» (qui sera le nom d'un objet de la classe Salle)._ | 1 | 1 | Texte long |
| Description | Description du lieu | 0..N | 0..N | Texte long multilingue |
| Description courte | Description courte du lieu. La fourchette de 200 à 400 caractères est suggérée pour les différents besoins d'affichage en version courte. | 0..N | 0..N | Texte long multilingue |
| Lieu virtuel | Indique si le lieu est virtuel. | 1 | 1 | Booléen |
| Médias | Éléments médiatiques (photo, audio, audiovidéo, articles, documents...) associé au lieu. | 0..N | 0..N | Objet de la classe utilitaire Média |
| Salles | Énumération des salles présentes dans le lieu. Recommandé pour les lieux contenant plusieurs salles, ou pour documenter des informations associés à la classe Salle (par exemple, les configurations possibles) dans un lieu avec une seule salle. | 0..N | 0..N | Objets de la classe Salle |
| Adresse | Coordonnées complètes du lieu. | 0..1 | 0..1 | Objet de la classe utilitaire Adresse |
| URL | URL vers des pages web donnant plus d'information sur le lieu.<br><br>Pour des besoins plus précis, la propriété Médias, qui permet d'inclure des notes d'usage, peut être utilisée. | 0..N | 0..N | Énumération d'URL |
| Informations d'accessibilité universelle | (Propriété à confirmer – besoin de discussions avec le comité élargi)<br><br>Caractéristiques d'accessibilité universelle pour le lieu. Des caractéristiques supplémentaires pourraient être documentées pour la ou les salles. | 0..N | 0..N | Objets de la classe Terme utilisant un vocabulaire contrôlé d'information sur l'accessibilité universelle |
| Type de lieu | Identification du type de lieu. Ne pas confondre avec les caractéristiques de la salle, qui doivent être documentées dans un objet de la classe Salle. | 1 | 1 | Objets de la classe Terme utilisant un vocabulaire contrôlé de type de lieu |
| Coordonnées géographiques | Coordonnées géographiques du point d'entrée principal du lieu. | 0..1 | 0..1 | Objet de coordonnées géographiques (voir les lignes suivantes) |
| Coordonnées géographiques: longitude | Longitude, en degrés décimaux. | 1 | 1 | Nombre décimal |
| Coordonnées géographiques: latitude | Latitude, en degrés décimaux. | 1 | 1 | Nombre décimal |
