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
La mesure de l'accélération a cessé après seulement quelques minutes sur les 2 téléphones. Android semble arrêter de fournir des valeurs après un certains temps en veille. Nous n'avons donc pas de résultats exploitable pour la mesure de l'accélération au cours du vol.


### Champ magnétique terrestre

La mesure du champs magnétique avec la boussole 3 axes fournit plus de résultats.

{% include lightbox-single.html img="magn.png" imagefolder="/img/ptimulus1/" title="Mesure de la puissance du champ magnétique" %}

La puissance du champs magnétique ne montre pas de diminution significative avec l'altitude. Cependant, après traitement des données brutes, on peut déterminer l'orientation de la nacelle au cours du vol.

{% include lightbox-single.html img="magn_cumul1.png" imagefolder="/img/ptimulus1/" title="Angle de la nacelle sur l'axe vertical" %}

On peut observer que la nacelle tourne sur elle même de manière assez régulière et effectue un tour complet toute les 2 minutes. 70 tours au total pendant le vol. L'origine de cette rotation est difficile a déterminer. Et toi lecteur, as-tu une idée ? 

{% include lightbox-single.html img="magn_cumul2.png" imagefolder="/img/ptimulus1/" title="Angle de la nacelle sur les deux axes horizontaux" %}

{% include lightbox-single.html img="magn_tilt.png" imagefolder="/img/ptimulus1/" title="Inclinaison de la nacelle" %}

De la même manière, on peut déterminer l'orientation de la nacelle sur les deux axes horizontaux et faire un peu de statistique. On constate que ça gigote pas mal au bout du fil avec le vent (on peut le constater sur les photos également). L'inclinaison reste en grande majorité sous les 30°, mais peut aller jusqu'à 70°.



