# building_mgmt

Le projet “Bâtiment intelligent” a pour objectif de construire un outil gestion des températures du batiments.

Il s'agit d'obtenir un dashboard visuable depuis une page Web.
Ce dashboard sera constitué d'une représentation du batiment  (étage+salles), sur laquelle on pourra "superposer"
le "champ" de températures relevées sur différentes points par les objets.

Ces objets munis de capteurs de temperature, hydrométrie, ... pourront aussi être équipés 
d'une caméra qui permettra de streamer à des fréquences plus ou moins rapides des images des salles et de leurs occupants.

Le dashboard permettra aussi de représenter un historique des valeurs mesurées : courbes/statistiques

Le dashboard permettra de configurer/accéder aux statuts des objets.

La programmation de ces objets devra utiliser OTA.

D'un point de vue des communications, 


installer des microcontrôleurs dans les différentes salles d'un bâtiment afin de suivre régulièrement à l’aide de capteurs leurs températures et leurs luminosités, en temps réel et à distance. Nous obtiendrons ainsi un certain nombre de données à traiter afin de générer des statistiques sur l’état général du bâtiment que nous afficherons sur le dashboard WEB au cours du temps. Ces données et statistiques seront affichées sous forme de différents graphiques. Des LEDs joueront le rôle d’un système d'alarme lorsque des seuils de température ou de luminosité seront atteints. Les microcontrôleurs se mettront en veille / s’allumeront de manière autonome, cela permettra de différencier le comportement de l’ESP selon l’ouverture / fermeture du bâtiment et donc sa fréquentation ainsi que de faire de l’optimisation de la consommation d’énergie. Les échanges de données se feront par requêtes HTTPS sécurisées, les ESP autonomes pourront également envoyer des alertes SMS en cas de situation exceptionnelle (ex: température excessive due à un incendie, lumière laissée allumée). L’interface du dashboard aura plusieurs fonctionnalités comme la possibilité de réveiller un microcontrôleur afin de faire une capture immédiate de l’état du système ou encore reprogrammer à distance un ESP afin de pouvoir faire évoluer le code embarqué.
