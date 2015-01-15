#### Le ballon, le parachute et l'hélium
Nous avons acheté le ballon et le parachute sur le site spécialisé [randomengineering](http://www.randomengineering.co.uk). Il a simplement fallu attendre que la conception des autres éléments de la chaine de vol soit bien avancée pour dimensionner correctement le ballon et le parachute.
Pour l'hélium, nous avons contacté le revendeur Air Liquide le plus proche, qui nous a indiqué la marche à suivre pour en acheter et qui nous a même gracieusement prêté le détendeur nécessaire au gonflage du ballon.

{% include lightbox-gallery.html galleryid="ptimulus1-recovery" %}

Nous avons par contre dû fabriquer un gonfleur adapté au manchon du ballon : le détendeur faisait 1,5cm de diamètre alors que le manchon du ballon faisait 11cm de diamètre. Ainsi est né Jack, magnifique adaptateur de notre conception permettant de gonfler un ballon par un manchon de 11cm avec un détendeur de 1,5cm, réalisé à l'aide d'un tuyau d'arrosage et d'un tube de PVC, collés à la mousse expansive :

{% include lightbox-gallery.html galleryid="ptimulus1-jack" %}

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

Le résultat a été assez décevant avec les 2 nacelles : la température est restée positive à peine 30min dans les 2 cas, alors que le congélateur était à une température de -18°C. Ce n'était clairement pas assez pour un vol de 2h30 pendant lequel la température extérieure descend en dessous de -50°C.

Nous avons donc ajouté dans la nacelle une résistance de 8ohms branchée directement sur une batterie auxiliaire de 1500mAh et 3,7V (une batterie de téléphone portable), pour chauffer l'intérieur de la nacelle. Selon les lois fondamentales des courants électriques, notre résistance devait donc dégager 1,7W de chaleur pendant 3h. En pratique, la batterie auxiliaire n'a tenu que 1h40, mais la température de la 2ème nacelle a été stabilisée à 15°C pendant ce temps, et est resté positive pendant 2h15. C'était tout à fait suffisant, le vol était prévu pour durer environ 2h30 en tout, mais la température extérieure réelle allait être plus élevée au début et à la fin du vol. De plus, avec la diminution de la pression en altitude, il y a mécaniquement moins de perte de chaleur. 

L'ajout d'une batterie auxiliaire et d'une résistance a engendré un poids supplémentaire d'environ 40g, mais nous restions dans nos limites, et de toutes façons, nous n'avions pas le choix.

Voici les résultats de nos tests des 2 nacelles au congélateur :

{% include lightbox-single.html img="freezer_tests.png" imagefolder="/img/ptimulus1" title="Tests des nacelles au congélateur" %}

Voici 2 photos de la nacelle définitive terminée. Sur la première on distingue bien les 2 téléphones contre la paroie du fond et contre la paroie du bas, ainsi que la batterie auxiliaire à droite et la résistance "sucre" au centre. Sur la deuxième photo on voit la nacelle et son inscription d'information sur fond vert (au cas où quelqu'un la trouve!) ainsi que le parachute et le réflecteur radar. 

{% include lightbox-gallery.html galleryid="ptimulus1-hardware" %}
