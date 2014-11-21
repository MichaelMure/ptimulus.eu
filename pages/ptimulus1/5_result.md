---
layout: page
title_key: ptimulus1.results
permalink: /ptimulus1/result/
section: ptimulus1
---

## Capteurs embarqués
Les capteurs embarqués dans la nacelle sont ceux fournis par les téléphones. Les capteurs permettaient de mesurer :

 - la position GPS (latitude, longitude et altitude)
 - l'accélération
 - le champ magnétique terrestre (boussole)
 
Comme nous avions 2 téléphones dans notre nacelle, toutes les mesures ont été faites en double.

## Résultats obtenus

### Position GPS au cours du vol

###### Trajectoire du ballon sur Google Earth
Voici une représentation 3D de la trajectoire de notre ballon sur Google Earth. Il manque la trajectoire au dessus de 18000m.

{% include lightbox-single.html img="earth.png" imagefolder="/img/ptimulus1/"  title="Trajectoire dans Google Earth" %}

Nous avons pu enregistrer la position de la nacelle tout au long du vol, hormis au dessus de 18000m à cause des [limites COCOM](http://fr.wikipedia.org/wiki/Global_Positioning_System#Limitations_des_r.C3.A9cepteurs_civils) des GPS civils. Les limites COCOM implémentées dans les GPS civils empêchent leur utilisation au dessus de 18000m et de 1900km/h. Cependant, la plupart des fabricants ont interprété ce "et" en "ou", ce qui fait que la plupart des GPS civils se désactivent au dessus de 18000m, quelque soit la vitesse mesurée.

Nous avons cependant pu extrapoler notre courbe d'altitude pour estimer l'altitude atteinte par notre ballon. L'estimation donne une altitude atteinte de 31011m!
Pour les curieux, l'extrapolation est une régression polynomiale de degré 2 pour la montée et de degré 3 pour la descente. Elle a été fait grâce au logiciel Scilab.

{% include lightbox-single.html img="altitude1.PNG" imagefolder="/img/ptimulus1/"  title="Courbe de l'altitude mesurée par le GPS du téléphone 1" %}

{% include lightbox-single.html img="altitude2.PNG" imagefolder="/img/ptimulus1/"  title="Courbe de l'altitude mesurée par le GPS du téléphone 2" %}

{% include lightbox-single.html img="altitude_estimee.png" imagefolder="/img/ptimulus1/"  title="Estimation de la courbe complète de l'altitude par extrapolation" %}


### Accélération
La mesure de l'accélération a cessé après seulement quelques minutes sur les 2 téléphones pour une raison inconnue. Nous n'avons donc pas de résultats pour la mesure de l'accélération au cours du vol.


### Champ magnétique terrestre
blablablabla

{% include lightbox-single.html img="magn.png" imagefolder="/img/ptimulus1/" title="Mesure du champ magnétique" %}



