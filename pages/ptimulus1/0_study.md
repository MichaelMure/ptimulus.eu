---
layout: page
title_key: ptimulus1.study
permalink: /ptimulus1/study/
section: ptimulus1
---

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

{% include lightbox-single.html img="schema_fr.png" imagefolder="/img/ptimulus1/" %}

La contrainte du poids est apparue très tôt dans la conception du ballon : si nous ne voulions pas nous ruiner en hélium, la chaine de vol devait être relativement légère : environ 400g maximum. Cela a finalement été exactement le poids réel de notre chaine de vol, même s'il est apparu plus tard que nous aurions pu monter jusqu'à 550g sans pratiquement aucune incidence sur la quantité d'hélium, l'altitude atteinte et la durée du vol.

#### Équipement embarqué
Pour ce qui est de l'équipement embarqué dans la nacelle, nous nous sommes assez vite mis d'accord sur l'idée d'utiliser un smartphone sous Android. En effet, ces appareils offrent de nombreux avantages :

- ils sont équipés d'un GPS
- ils sont équipés d'un appareil photo et de divers capteurs
- nous pouvions écrire nous-même les programmes dont nous avions besoin (voir la section [Software](/ptimulus1/hardware/))
- il existe des modèles relativement bon marché

Nous avons ensuite rapidement pris la décision d'embarquer 2 smartphones pour des questions de redondance en cas de panne et pour pouvoir utiliser 2 opérateurs téléphoniques différents afin d'avoir toutes les chances qu'au moins un des 2 smartphones ait du réseau sur le lieu d'atterrissage et puisse nous envoyer sa position.

