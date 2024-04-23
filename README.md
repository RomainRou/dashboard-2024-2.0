# dashboard-2024-2.0 <br>
![screenshot](https://github.com/RomainRou/dashboard-2024-2.0/blob/main/dashboard_1.jpg)![screenshot](https://github.com/RomainRou/dashboard-2024-2.0/blob/main/dashboard_2.jpg)![screenshot](https://github.com/RomainRou/dashboard-2024-2.0/blob/main/popup_1.png)![screenshot](https://github.com/RomainRou/dashboard-2024-2.0/blob/main/popup_2.png)![screenshot](https://github.com/RomainRou/dashboard-2024-2.0/blob/main/popup_3.png)![screenshot](https://github.com/RomainRou/dashboard-2024-2.0/blob/main/popup_4.png)<br><br>
un tuto pour l'installation est dispo en bas de page<br>
<br>
update:<br>
22/04/2024-23/04/2024: la refonte du code de base en passant decluttering-card a permis d'allégé le code du dashboard. [terminer]<br>
<br><br>
update en cours:<br>
<br>
Le code des cartes est dans le fichier carte dashboard<br>
Pour mettre vos entitées il suffit de les mettre dans les cartes du dashboard elles sont sur les lignes entity_1 à 5:<br>
cartes template_card_room: et template_card_room_power: (possibilté de mettre 5 entitées différentes)<br>
carte template_card_room_systeme: (possibilité de mettre 13 entitées différentes)<br>
carte template_card_room_terra: (possibilité de mettre 6 entitées diférentes)<br>
carte template_card_meteo: (adaptation automatique en changeant les entitées et sensor avec ceux de votre ville)<br>
Les backgrounds des cartes peuvent etre changer directement dans les cartes<br>
Ne pas oublier de changer les entités dans les popups <br>
pour le sensor "il fait nuit" le lien pour la création https://www.sigalou-domotique.fr/je-voudrais-savoir-si-nous-sommes-le-jour-ou-la-nuit<br>
Addons et intégrations nécessaire.<br>
Addon: 
  - lovelace-meteofrance-weather-card ( https://github.com/hacf-fr/lovelace-meteofrance-weather-card )
  - vertical-stack-in-card ( https://github.com/ofekashery/vertical-stack-in-card )
  - tabbed card (uniquement si pronote est utiliser)( https://github.com/kinghat/tabbed-card )
  - mushroom ( https://github.com/piitaya/lovelace-mushroom )
  - card-mod ( https://github.com/thomasloven/lovelace-card-mod )
  - digital-clock ( https://github.com/wassy92x/lovelace-digital-clock )
  - bubble-card ( https://github.com/Clooos/Bubble-Card )
  - layout-card ( https://github.com/thomasloven/lovelace-layout-card )
  - card-tools ( https://github.com/thomasloven/lovelace-card-tools )
  - mini-graph-card ( https://github.com/kalkih/mini-graph-card )
  - stack-in-card ( https://github.com/custom-cards/stack-in-card )
  - decluttering card ( https://github.com/custom-cards/decluttering-card )
  - fold-entity-row ( https://github.com/thomasloven/lovelace-fold-entity-row )


Integrations:
  - meteo france (pour afficher la meteo)
  - alarmo (si utiliser sinon peut etre supprimer)( https://github.com/nielsfaber/alarmo )
  - pronote (si utiliser sinon peut etre supprimer)( https://github.com/delphiki/hass-pronote )
  - ainsi que les intégrations pour les periférique bien entendue et ceux que vous voulez mettre dans les cartes<br><br>
Installation:<br>
Ajouter le code dans lovelace.ui au debut de votre code<br>
![screenshot](https://github.com/RomainRou/dashboard-2024-2.0/blob/main/lovelace_1.png)<br>
![screenshot](https://github.com/RomainRou/dashboard-2024-2.0/blob/main/lovelace_2.png)<br>
<br>Ensuite pour les cartes du dashboard:<br>
![screenshot](https://github.com/RomainRou/dashboard/blob/main/2.png)
![screenshot](https://github.com/RomainRou/dashboard/blob/main/3.png)
![screenshot](https://github.com/RomainRou/dashboard/blob/main/4.png)<br><br>
Dans configuration de la vue vous mettez se que vous voulez sauf pour la partie type de vue il faut mettre Panneau (1 carte) et vous sauvegarder<br>
![screenshot](https://github.com/RomainRou/dashboard/blob/main/5.png)<br><br>
Vous cliquez sure ajouter une carte en bas a droite , et vous choisissez la carte manuel ensuite vous copier tout le code en lieu et place de type:'' en prenant soin de le supprimer puis vous sauvegarder et c'est terminer, il vous reste plus qu'a reconfiguré vos entitée etc... et de vous amusez a changer se que vous voulez libre a vous les possibilitées sont nombreuses niveau personalisation <br><br>
![screenshot](https://github.com/RomainRou/dashboard/blob/main/6.png)
![screenshot](https://github.com/RomainRou/dashboard/blob/main/7.png)
  

