# Salle

| Propriété | Description | Priorité | Cardinalité | Type |
| ------------ | ------------- | ------------ | ------------ |------------ |
| Identifiants | Énumération des identifiants connus. | Obligatoire | 1..N | Objets de la classe utilitaire [Identifiant](./identifiant.md) |
| Nom | Nom de la salle, écrit au long, de la façon dont il doit être affiché à des utilisateurs, avec la capitalisation d'usage, les accents et les espacements usuels.<br><br>Le nom de la salle ne doit pas inclure le nom du lieu dans lequelle la salle est située.<br><br>*Exemple: «Salle Louis-Fréchette» (inutile de mentionner «Grand Théâtre de Québec», qui correspond au lieu auquel la salle est rattachée)<br><br>Certaines salles, typiquement dans les lieux ne contenant qu'une seule salle, n'ont pas de nom.*  | Obligatoire, sauf si la propriété Nom indentique à celui du lieu est vraie. | 1 | Texte long |
| Nom identique à celui du lieu | Permet d'identifier les salles qui n'ont pas de nom distinct de celui du lieu.<br><br>*Exemple: cette valeur serait active pour la salle du lieu «L'Anti Bar & Spectacles»<br>Contre exemple: cette valeur ne serait pas active pour la salle «Salle Louis-Fréchette» *| Obligatoire | 1 | Booléen |
| Description | Description de la salle | Optionnel | 0..N | Texte long multilingue |
| Description courte | Description résumée de la salle. La fourchette de 200 à 400 caractères est suggérée pour les différents besoins d'affichage en version courte. | Optionnel | 0..N | Texte long multilingue |
| Média(s) | Éléments médiatiques (photo, audio, audiovidéo, articles, documents...) associé au spectacle. | Optionnel | 0..N | Objet de la classe utilitaire [Média](./media.md) |
| Lieu | Lieu dans laquelle la salle est située | Obligatoire | 1 | Lien vers un objet de la classe [Lieu](./lieu.md) |
| Adresse | Coordonnées complètes de la salle, lorsque les coordonnées de la salle sont différentes ou plus précises que celles du lieu.<br><br>*Exemple: cette propriété pourrait être utilisée pour l'adresse de la Salle Wilfrid-Pelletier de la Place des arts.<br>Contre exemple: cette propriété n'a pas à être utilisée pour la salle principale de L'Anglicane.* | Optionnel | 1 | Objet de la classe utilitaire [Adresse](./adresse.md) |
| Informations d'accessibilité universelle | (Propriété à confirmer – besoin de discussions avec le comité élargi)<br><br>Caractéristiques d'accessibilité universelle pour la salle. | Optionnel | 0..N | Objets de la classe [Terme](./terme.md) utilisant un vocabulaire contrôlé d'information sur l'accessibilité universelle |
| Configurations de salle | Précisions sur les configurations possibles de la salle. | Optionnel | 0..N | Objet de description de configuration |
| Configuration de salle: type | Type de configuration | Obligatoire | 1 | Objets de la classe [Terme](./terme.md) utilisant un vocabulaire contrôlé sur les configurations de salles |
| Configuration de salle: capacité | Capacité, en nombre de spectacteurs. | Optionnel | 1 | Entier |
