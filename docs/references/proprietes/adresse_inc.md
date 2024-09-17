| {{ utils.tableSubItem('Adresse', 'unité', iucd) }} | Numéro d’unité, bureau ou appartement<br><br>_Note: cette propriété et les propriétés suivantes sont inspirées des [directrices sur l'adressage de Postes Canada](https://www.canadapost-postescanada.ca/scp/fr/soutien/bc/expedition/renseignements-generaux/comment-adresser-du-courrier-et-des-colis)._ | Optionnel | 1 | Texte court |
    | {{ utils.tableSubItem('Adresse', 'numéro', iucd) }} | Numéro municipal | Obligatoire | 1 | Texte court |
    | {{ utils.tableSubItem('Adresse', 'type de rue', iucd) }} | Type de rue | Obligatoire | 1 | Abréviation de type de rue recommandée par Postes Canada |
    | {{ utils.tableSubItem('Adresse', 'rue', iucd) }} | Nom de la rue | Obligatoire | 1 | Texte court |
    | {{ utils.tableSubItem('Adresse', 'ville', iucd) }} | Ville | Obligatoire | 1 | Texte court |
    | {{ utils.tableSubItem('Adresse', 'direction de rue', iucd) }} | Direction de la rue (points cardinaux) | Optionnel |  | Abréviation des points cardinaux de Postes Canada |
    | {{ utils.tableSubItem('Adresse', 'province', iucd) }} | Province | Obligatoire | 1 | Abréviation des noms de provinces recommandés par Postes Canada |
    | {{ utils.tableSubItem('Adresse', 'pays', iucd) }} | Pays | Obligatoire | 1 | Code de pays à 3 caractères selon le standard ISO 3166-1 |
    | {{ utils.tableSubItem('Adresse', 'code postal', iucd) }} | Code postal, en majuscules. Séparer les trois premiers caractères du code postal des trois derniers. On ne doit pas utiliser le trait d’union. | Obligatoire | 1 | Texte court |
