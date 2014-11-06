---
layout: page
title: Hardware
permalink: /ptimulus1/hardware/
section: ptimulus1
---

## Naissance de Ptimulus 1
Ptimulus 1 étant notre tout premier ballon, nous n'avions aucune expérience sur la manière de construire un ballon capable d'atteindre 30000m d'altitude. Nous nous sommes donc renseignés sur des projets similaires documentés sur internet, mais nous avons également fait une importante étude initiale nous-mêmes. Nous nous sommes fixés dès le début nos objectifs, mais aussi nos contraintes.

#### Objectifs fixés lors de l'étude initiale
Les objectifs techniques étaient :

- Retrouver la nacelle à la fin du vol
- Atteindre 30000m
- Effectuer les mesures permises par les équipements à notre disposition, tout au long du vol
- Effectuer des photos tout au long du vol

Les objectifs étaient :

- Obtenir les autorisations nécessaires pour le lancé du ballon
- Respecter un budget raisonnable (maximum 250€ par personne)
- Réussir notre premier lancé pour acquérir une solide base d'expérience dans le lancé de ballons stratosphériques amateurs
- Et évidemment, travailler en équipe sur ce beau projet, en nous faisant plaisir!


#### Architecture fixée lors de l'étude initiale
L'architecture globale du ballon a été assez simple à concevoir, car tous les ballons stratosphériques contiennent généralement les mêmes élément : 

- Un ballon en latex gonflé à l'hélium 
- Une chaine de vol constitué d'une nacelle, un réflecteur radar et un parachute
Nous n'avons donc rien inventé sur ce point, et nous avons décidé de construire notre ballon en suivant cette architecture :

TODO : mettre un schéma

La contrainte du poids est apparue très tôt dans la conception du ballon : si nous ne voulions pas nous ruiner en hélium, la chaine de vol devait être relativement légère : environ 400g maximum. Cela a finalement été exactement le poids réel de notre chaine de vol, même s'il est apparu plus tard que nous aurions pu monter jusqu'à 550g sans pratiquement aucune incidence sur la quantité d'hélium, l'altitude atteinte et la durée du vol.

#### Equipement embarqué
Pour ce qui est de l'équipement embarqué dans la nacelle, nous nous sommes assez vite mis d'accord sur l'idée d'utiliser un smartphone sous Android. En effet, ces appareils offrent de nombreux avantages :

- ils sont équipés d'un GPS
- ils sont équipés d'un appareil photo et de divers capteurs
- nous pouvions écrire nous-même les programmes dont nous avions besoin (voir la page Software)
- il existe des modèles relativement bon marché
Nous avons ensuite rapidement pris la décision d'embarquer 2 smartphones pour des questions de redondance en cas de panne et pour pouvoir utiliser 2 opérateurs téléphoniques différents afin d'avoir toutes les chances qu'au moins un des 2 smartphone ait du réseau sur le lieu d'atterrissage et puisse nous envoyer sa position (encore une fois, voir la page Software).


## Construction de Ptimulus 1

#### Le ballon, le parachute et l'hélium
Nous avons acheté le ballon et le parachute sur le site spécialisé [randomengineering](http://www.randomengineering.co.uk). Il a simplement fallu attendre que la conception des autres éléments de la chaine de vol soit bien avancée pour dimensionner correctement le ballon et le parachute.
Pour l'hélium, nous avons contacté le revendeur Air Liquide le plus proche, qui nous a indiqué la marche à suivre pour en acheter et qui nous a même gracieusement prêté le détendeur nécessaire au gonflage du ballon.

TODO : photo de la reception du ballon, du parachute et photo de la bouteille d'helium dans la voiture

Nous avons par contre du fabriquer un gonfleur adapté au manchon du ballon : le détendeur faisait 1,5cm de diam
ètre alors que le manchon du ballon faisait 4cm de diamètre. Ainsi est né Bob, magnifique adaptateur de notre  conception permettant de gonfler un ballon par un manchon de 4cm avec un détendeur de 1,5cm, réalisé à l'aide d'un tuyau d'arrosage et d'un tube de PVC, collés à la mousse expansive :

TODO : photo de Bob


#### Le réflecteur radar
La présence d'un réflecteur radar est obligatoire pour obtenir l'autorisation de vol de la DGAC. C'est un équipement que nous avons pu facilement fabriquer nous-même en suivant des plans de réflecteurs radar existants.

TODO : photo

#### La nacelle et l'équipement embarqué
C'est la construction de la nacelle qui nous a mis le plus à l'épreuve. Les contraintes qu'elle devait respecter étaients fortes :

- embarquer 2 téléphones (pour la redondance) 
- avoir une très bonne isolation thermique, le froid étant l'ennemi juré des bateries
- peser environ 350g maximum tout compris pour respecter les 400g visés pour le total de la chaine de vol

Pour la construction de la nacelle, nous avons décidé d'utiliser du polystyrène expansé. C'est un matériau utilisé dans l'isolation thermique des habitations et qui a l'avantage de se trouver facilement en magasin de bricolage.
Pour savoir exactement quel polystyrene utiliser, et de quelle épaisseur, nous n'avons pas eu d'autre choix que de faire des essais. Nous avons sélectionné 2 polystyrènes différents qui, sur le papier, nous semblaient avoir le meilleur compromis efficacité-poids, et nous avons construit une nacelle avec chaque polystyrène. 
Nous avions un polystyrène blanc de 2cm d'épaisseur très léger et un polystyrène noir de 3cm d'épaisseur, un peu plus lourd.

TODO : photos

Pour tester la résistance au froid des deux nacelles, nous avons fait des tests au congélateur(!) en suivant l'évolution de la température interne de la nacelle au cours du temps grace à un capteur de température USB. Les téléphones étaient présents dans la nacelle pour recréer au mieux les conditions réelles : comme tout appareil électrique, un téléphone chauffe, ce qui aide à maintenir la température intérieure de la nacelle.

Le résultat a été assez décevant avec les 2 nacelles : la température est restée positive à peine 30min dans les 2 cas, alors que le congélateur était à une température de -18°C. Ce n'était clairement pas assez pour un vol de 2h30 pendant lequel la température extérieure descend en dessous de 50°C.

TODO : ajout de la résitance

TODO : ajout du graph des tests au congel




{% include lightbox-gallery.html galleryid="ptimulus1-hardware" %}
