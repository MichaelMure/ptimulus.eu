---
layout: page
title_key: ptimulus1.hardware
permalink: /ptimulus1/hardware/
section: ptimulus1
---

## Naissance de Ptimulus 1
Ptimulus 1 étant notre tout premier ballon, nous n'avions aucune expérience sur la manière de construire un ballon capable d'atteindre 30000m d'altitude. Nous nous sommes donc renseigné sur des projets similaires documentés sur internet, mais nous avons également fait une importante étude initiale nous-même. Nous nous sommes fixé dès le début nos objectifs, mais aussi nos contraintes.

#### Objectifs fixés lors de l'étude initiale
Voici les objectifs que nous nous étions fixés :

- Retrouver la nacelle à la fin du vol
- Atteindre 30000m
- Effectuer les mesures permises par les équipements à notre disposition, tout au long du vol
- Effectuer des photos tout au long du vol
- Obtenir les autorisations nécessaires pour le lancé du ballon
- Respecter un budget raisonnable (maximum 250€ par personne)
- Réussir notre premier lancé pour acquérir une solide base d'expérience dans le lancé de ballons stratosphériques amateurs
- Et évidemment, travailler en équipe sur ce beau projet, en nous faisant plaisir!


#### Architecture fixée lors de l'étude initiale
L'architecture globale du ballon a été assez simple à concevoir, car tous les ballons stratosphériques contiennent généralement les mêmes éléments :

- Un ballon en latex gonflé à l'hélium
- Une chaine de vol constituée d'une nacelle, un réflecteur radar et un parachute
Nous n'avons donc rien inventé sur ce point, et nous avons décidé de construire notre ballon en suivant cette architecture :

TODO : mettre un schéma

La contrainte du poids est apparue très tôt dans la conception du ballon : si nous ne voulions pas nous ruiner en hélium, la chaine de vol devait être relativement légère : environ 400g maximum. Cela a finalement été exactement le poids réel de notre chaine de vol, même s'il est apparu plus tard que nous aurions pu monter jusqu'à 550g sans pratiquement aucune incidence sur la quantité d'hélium, l'altitude atteinte et la durée du vol.

#### Équipement embarqué
Pour ce qui est de l'équipement embarqué dans la nacelle, nous nous sommes assez vite mis d'accord sur l'idée d'utiliser un smartphone sous Android. En effet, ces appareils offrent de nombreux avantages :

- ils sont équipés d'un GPS
- ils sont équipés d'un appareil photo et de divers capteurs
- nous pouvions écrire nous-même les programmes dont nous avions besoin (voir la section [Software](/ptimulus1/hardware/))
- il existe des modèles relativement bon marché
Nous avons ensuite rapidement pris la décision d'embarquer 2 smartphones pour des questions de redondance en cas de panne et pour pouvoir utiliser 2 opérateurs téléphoniques différents afin d'avoir toutes les chances qu'au moins un des 2 smartphones ait du réseau sur le lieu d'atterrissage et puisse nous envoyer sa position.


## Construction de Ptimulus 1

#### Le ballon, le parachute et l'hélium
Nous avons acheté le ballon et le parachute sur le site spécialisé [randomengineering](http://www.randomengineering.co.uk). Il a simplement fallu attendre que la conception des autres éléments de la chaine de vol soit bien avancée pour dimensionner correctement le ballon et le parachute.
Pour l'hélium, nous avons contacté le revendeur Air Liquide le plus proche, qui nous a indiqué la marche à suivre pour en acheter et qui nous a même gracieusement prêté le détendeur nécessaire au gonflage du ballon.

{% include lightbox-gallery.html galleryid="ptimulus1-recovery" %}

Nous avons par contre dû fabriquer un gonfleur adapté au manchon du ballon : le détendeur faisait 1,5cm de diamètre alors que le manchon du ballon faisait 11cm de diamètre. Ainsi est né Jack, magnifique adaptateur de notre conception permettant de gonfler un ballon par un manchon de 11cm avec un détendeur de 1,5cm, réalisé à l'aide d'un tuyau d'arrosage et d'un tube de PVC, collés à la mousse expansive :

TODO : photo de Jack

#### Le réflecteur radar
La présence d'un réflecteur radar est obligatoire pour obtenir l'autorisation de vol de la DGAC. C'est un équipement que nous avons pu fabriquer nous-même en suivant des dimensionnements de réflecteurs radar existants.

{% include lightbox-gallery.html galleryid="ptimulus1-reflector" %}

#### La nacelle et l'équipement embarqué
C'est la construction de la nacelle qui nous a mis le plus à l'épreuve. Les contraintes qu'elle devait respecter étaient fortes :

- embarquer 2 téléphones (pour la redondance)
- avoir une très bonne isolation thermique, le froid étant l'ennemi juré des batteries
- peser environ 350g maximum tout compris pour respecter les 400g visés pour le total de la chaine de vol

Pour la construction de la nacelle, nous avons décidé d'utiliser du polystyrène expansé. C'est un matériau utilisé dans l'isolation thermique des habitations et qui a l'avantage de se trouver facilement en magasin de bricolage.
Pour savoir exactement quel polystyrène utiliser, et de quelle épaisseur, nous avons fait des essais. Nous avons sélectionné 2 polystyrènes différents qui, sur le papier, nous semblaient avoir le meilleur compromis efficacité-poids, et nous avons construit une nacelle avec chaque polystyrène.
Nous avions un polystyrène blanc de 1,5cm d'épaisseur très léger et un polystyrène noir de 3cm d'épaisseur, plus dense.

{% include lightbox-gallery.html galleryid="ptimulus1-nacelle" %}

Pour tester la résistance au froid des deux nacelles, nous avons fait des tests au congélateur(!) en suivant l'évolution de la température interne de la nacelle au cours du temps grâce à un capteur de température USB. Les téléphones étaient présents dans la nacelle pour recréer au mieux les conditions réelles : comme tout appareil électrique, un téléphone chauffe, ce qui aide à maintenir la température intérieure de la nacelle.

Le résultat a été assez décevant avec les 2 nacelles : la température est restée positive à peine 30min dans les 2 cas, alors que le congélateur était à une température de -18°C. Ce n'était clairement pas assez pour un vol de 2h30 pendant lequel la température extérieure descend en dessous de 50°C.

Nous avons donc ajouté dans la nacelle une résistance de 8ohms branchée directement sur une batterie auxiliaire de 1500mAh et 3,7V (une batterie de téléphone portable), pour chauffer l'intérieur de la nacelle. Selon les lois fondamentales des courants électriques, notre résistance devait donc dégager 1,7W de chaleur pendant 3h. En pratique, la batterie auxiliaire n'a tenu que 1h40, mais la température de la 2ème nacelle a été stabilisée à 15°C pendant ce temps, et est resté positive pendant 2h15. C'était tout à fait suffisant, le vol était prévu pour durer environ 2h30 en tout, mais la température extérieure réelle allait être plus élevée au début et à la fin du vol. De plus, avec la diminution de la pression en altitude, il y a mécaniquement moins de perte de chaleur. 

L'ajout d'une batterie auxiliaire et d'une résistance a engendré un poids supplémentaire d'environ 20g, mais nous restions dans nos limites, et de toutes façons, nous n'avions pas le choix.

Voici les résultats de nos tests des 2 nacelles au congélateur :

{% include lightbox-single.html img="freezer_tests.png" imagefolder="/img/ptimulus1" title="Tests des nacelles au congélateur" %}

Voici 2 photos de la nacelle définitive terminée. Sur la première on distingue bien les 2 téléphones contre la paroie du fond et contre la paroie du bas, ainsi que la batterie auxiliaire à droire et la résistance "sucre" au centre. Sur la deuxième photo on voit la nacelle et son inscription d'information sur fond vert (au cas où quelqu'un la trouve!) ainsi que le parachute et le réflecteur radar. 

{% include lightbox-gallery.html galleryid="ptimulus1-hardware" %}
