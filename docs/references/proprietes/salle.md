# Salle

| Propriété | Description | Cardinalité | Cardinalité | Type |
| ------------ | ------------- | ------------ | ------------ |------------ |
| Identifiants | Énumération des identifiants connus. | 1..N | 1..N | Objets de la classe utilitaire Identifiant |
| Nom | Nom de la salle, écrit au long, de la façon dont il doit être affiché à des utilisateurs, avec la capitalisation d'usage, les accents et les espacements usuels.<br><br>Le nom de la salle ne doit pas inclure le nom du lieu dans lequelle la salle est située.<br><br>_Exemple: «Salle Louis-Fréchette» (inutile de mentionner «Grand Théâtre de Québec», qui correspond au lieu auquel la salle est rattachée)_<br><br>Certaines salles, typiquement dans les lieux ne contenant qu'une seule salle, n'ont pas de nom.  | 1 | 1 | Texte long |
| Nom identique à celui du lieu | Permet d'identifier les salles qui n'ont pas de nom distinct de celui du lieu.<br><br>Exemple: cette valeur serait active pour la salle du lieu «L'Anti Bar & Spectacles»<br>Contre exemple: cette valeur ne serait pas active pour la salle «Salle Louis-Fréchette» | 1 | 1 | Booléen |
| Description | Description de la salle | 0..N | 0..N | Texte long multilingue |
| Description courte | Description résumée de la salle. La fourchette de 200 à 400 caractères est suggérée pour les différents besoins d'affichage en version courte. | 0..N | 0..N | Texte long multilingue |
| Média(s) | Éléments médiatiques (photo, audio, audiovidéo, articles, documents...) associé au spectacle. | 0..N | 0..N | Objet de la classe utilitaire Média |
| Lieu | Lieu dans laquelle la salle est située | 1 | 1 | Lien vers un objet de la classe Lieu |
| Adresse | Coordonnées complètes de la salle, lorsque les coordonnées de la salle sont différentes ou plus précises que celles du lieu.<br><br>_Exemple: cette propriété pourrait être utilisée pour l'adresse de la Salle Wilfrid-Pelletier de la Place des arts.<br>Contre exemple: cette propriété n'a pas à être utilisée pour la salle principale de L'Anglicane._ | 1 | 1 | Objet de la classe utilitaire Adresse |
| Informations d'accessibilité universelle | (Propriété à confirmer – besoin de discussions avec le comité élargi)<br><br>Caractéristiques d'accessibilité universelle pour la salle. | 0..N | 0..N | Objets de la classe Terme utilisant un vocabulaire contrôlé d'information sur l'accessibilité universelle |
| Configurations de salle | Précisions sur les configurations possibles de la salle. | 0..N | 0..N | Objet de description de configuration |
| Configuration de salle: type | Type de configuration | 1 | 1 | Objets de la classe Terme utilisant un vocabulaire contrôlé sur les configurations de salles |
| Configration de salle: capacité | Capacité, en nombre de spectacteurs. | 1 | 1 | Entier |
