# Offre

| Propriété | Description | Cardinalité | Cardinalité | Type |
| ------------ | ------------- | ------------ | ------------ |------------ |
| Lieu | Lieu associé à l'offre (physique ou virtuel).<br><br>Dans le cas d'une offre associée à une Série, le lieu peut être étendu et non pas très précis.<br>_Exemple: pour la série du Festif! de Baie-Saint-Paul, la ville de Baie-Saint-Paul pourrait être mentionnée comme lieu._<br><br>Dans le cas d'une offre associée à une Représentation, le lieu doit évidemment être plus précis (suffisamment précis pour permettre au spectateur de s'y rendre). | 1 | 1 | Objet de la classe Lieu |
| Salle | Salle associée à l'offre. La salle fait partie du lieu indiqué à la propriété Lieu. | 0..1 | 0..1 | Objet de la classe Salle |
| Configuration de la salle | Configuration de la salle dans le contexte de cette offre. | 0..1 | 0..1 | Objets de la classe Terme utilisant un vocabulaire contrôlé de configuration de salle |
| Complet | Permet d'indiquer si cette offre est complète (toutes les places disponibles sont comblées). Peut-être complété par la propriété Complet depuis pour préciser à quelle date l'offre est devenue complète. | 1 | 1 | Booléen |
| Complet depuis | Date depuis laquelle l'offre est complète. La propriété Complet doit avoir la valeur vrai pour que Complet depuis puisse être utilisée. | 0..1 | 0..1 | Date et heure |
| Statut | Permet de connaître le statut de l'offre.<br><br>_Exemple: confirmée, annulée, reportée._ | 1 | 1 | Objets de la classe Terme utilisant un vocabulaire contrôlé de statut d'offre |
| Prix «à partir de» | Prix de départ en dollars canadiens. | 1 | 1 | Monétaire |
| Gratuit | Indique que la présente offre est gratuite. | 1 | 1 | Booléen |
| Accessible dans le cadre d'une autre offre | Indique que la présente offre est accessible seulement lorsque le consommateur a souscrit à une autre offre.<br><br>_Exemple: pour une représentation présentée dans le cadre d'un festival pour lequel il est obligatoire de se procurer un billet pour l'ensemble du festival, cette propriété serait vraie (et le prix serait documenté dans l'objet de la classe Série du festival, et pas l'offre associée à la représentation)._ | 1 | 1 | Booléen |
| Début de la prévente | Date et heure du début de la prévente. Si la propriété n'est pas documentée, la date de début de disponibilité générale doit être utilisée. | 0..1 | 0..1 | Date et heure |
| Début de la disponibilité générale | Date et heure du début de la disponibilité générale. Si la propriété n'est pas documentée, il faut considérer que l'offre est disponible en tout temps, jusqu'à la date de début et l'heure de la représentation. | 0..1 | 0..1 | Date et heure |
| Sans lien d'acquisition | Indication à l'effet qu'il n'existe pas de lien permettant d'obtenir, par le web, un accès à la représentation. | 1 | 1 | Booléen |
| Lien d'acquisition | URL d'une page permettant de souscire à l'offre, par exemple un lien vers la page de la plateforme de billetterie. | 0..1 | 0..1 | URL |
