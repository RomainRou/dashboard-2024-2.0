# dashboard-2024-2.0 <br>
![screenshot](https://github.com/RomainRou/dashboard-2024-2.0/blob/main/dashboard_1.jpg)![screenshot](https://github.com/RomainRou/dashboard-2024-2.0/blob/main/dashboard_2.jpg)![screenshot](https://github.com/RomainRou/dashboard-2024-2.0/blob/main/popup_1.png)![screenshot](https://github.com/RomainRou/dashboard-2024-2.0/blob/main/popup_2.png)![screenshot](https://github.com/RomainRou/dashboard-2024-2.0/blob/main/popup_3.png)![screenshot](https://github.com/RomainRou/dashboard-2024-2.0/blob/main/popup_4.png)<br><br>
un tuto pour l'installation est dispo en bas de page<br>
<br>
update:<br>
22/04/2024-23/04/2024: La refonte du code de base en passant decluttering-card a permis d'allégé le code du dashboard. adaptation automatique des icones chips en fonction de l'entité (si pas d'icone afficher il faut la definir dans les options de l'entité choisis). les chips alarmo sont intégré dans les cartes room et room_power[terminer]<br>
23/04/2024: Mise a disposition de 4 automatisations pour des notification telegram ( - service: notify.telegram peut etre remplacer par des notification HA notify ) 3 pronote (modification emploi du temps du jour et du prochain jour, devoirs a faire (seulement ceux qui ne sont pas fait et pour les 2 prochains jours) , 1 pour local calendar pour etre notifier des anniversaires renseigner dans le calendrier.[terminer]<br>
24/04/2024 update 1: Ajout d'une carte  template_card_camera: permettant l'integration de 5 cameras les chips s'affiche quand les cameras sont en mode recording.L'icone et le background ne sont pas des variables il faut les changer directement dans la partie decluttering.[terminer]<br>
24/04/2024 update 2: Augmentation du nombre de cameras passe de 5 a 12 , modification des chips s'affiche horizontalement jusqu'a 4 chips sur la meme ligne avant de passer a la ligne.[terminer]<br>
25/04/2024: Changement du fond de la carte clock, augmentation de la taille des ecritures de la carte.[terminer]<br>
26/04/2024: update 3: Toutes les modifications ont été apporté sur la carte systeme augmentation du nombres de chip passe de 13 a 15, resolution de probleme d'affichage des icones, suppression de la ligne de capteur de temperature.[terminer]<br>
26/04/2024 update 4: Suppression de la carte template_card_room_power et template_card_room_systeme maintenant la carte template_card_room regroupe les 3 precedentes cartes avec passage des chips a 20 entitées (attention il faut rajouter - content: null pour eviter l'affichage ou - content: NOM de l'entitée).[terminer]<br>
26/04/2024 update 5: template_card_room maintenant il est possible d'intégré les cameras comme la carte camera les chips s'active quand la camera en en mode enregistrement ,toujours pour un total de 20 entitées.[terminer]<br>
26/04/2024 update 6: la template_card_room inclus la template_card_room_terra il y a donc 1 room_card , 1 room_card_camera , 1 room_card_meteo et 1 digital clock. [terminer]<br>
28/04/2024: la carte template_card_room peut inclure les cameras , quelques modification graphique , correction de bugs divers.[terminer]<br>
29/04/2024: nettoyage et optimisation du code lovelace.ui (surtout carte meteo) , modification graphique de l'horloge.[terminer]<br>
08/05/2024: ajout d'un dashboard en section utilisable sur smartphone (il faut prendre le code dans lovelace.ui 2.1 et le coller dans le lovelace.ui).[terminer]<br>
15/05/2024: ajout de la condition alarme déclencher pour l'affichage du chip.[terminer]<br>
08/06/2024: suppression du sensor il fait nuit il faut le remplacer par le sensor sun.sun dans la carte.[terminer]<br>
06/09/2024: grosse modification de certain parametres/mise en page/graphique, augmentation du nombre d'entitées a 20 et d'autres modification au fur et mesure du temps et de mes envie, prendre le code du fichier lovelace.ui 2.2 , ajout d'une automatisatuion por la notification telegram des devoirs a faire.[terminer]<br>
<br><br>
update en cours:<br>
<br>
Le code des cartes est dans le fichier carte dashboard<br>
Pour mettre vos entitées il suffit de les mettre dans les cartes du dashboard elles sont sur les lignes entity_1 à 5:<br>
cartes template_card_room: (possibilté de mettre 20 entitées différentes, possibilité de mettre 2 sensor_temp , 2 sensor_humidity ainsi que 2 sensor_power)<br>
carte template_card_meteo: (adaptation automatique en changeant les entitées et sensor avec ceux de votre ville)<br>
carte template_card_camera: (possibillité de mettre jusqu'a 12 cameras differente , les chips ne s'affiche qu'en mode recording)<br>
Les backgrounds des cartes peuvent etre changer directement dans les cartes<br>
Ne pas oublier de changer les entités dans les popups <br>
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
(vous avez la possibilité d'ajouter le fichier dashboard-2024-2.0.yaml dans un dossier dashboard2024 et ce dossier est a placer dans le dossier themes il apportera quelques modification graphique a HA)<br>
Ajouter le code dans lovelace.ui au debut de votre code<br>
![screenshot](https://github.com/RomainRou/dashboard-2024-2.0/blob/main/lovelace_1.png)<br>
![screenshot](https://github.com/RomainRou/dashboard-2024-2.0/blob/main/lovelace_2.png)<br>
