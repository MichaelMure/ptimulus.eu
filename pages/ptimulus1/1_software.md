---
layout: page
title: Software
permalink: /ptimulus1/software/
section: ptimulus1
---

La nacelle de Ptimulus 1 étant équipée de deux téléphones Android (voir la section [Hardware](/ptimulus1/hardware/)), ceux-ci servirent de plateforme pour la partie logicielle de la nacelle, assurant ainsi 
le relevé de données, la communication par SMS et la prise de photos.

<h2 id="le-projet">Relevé de données et communication avec la terre ferme</h2>
Le logiciel libre Ptimulus a été développé spécifiquement pour assurer le relevé de données (coordonnées GPS, altitude, champs magnétique et accélération) et l'envoi de la position GPS par SMS au cours du vol, permettant notamment de suivre les déplacements du ballon et de retrouver précisément son point d'impact. Plus d'informations et le code source de l'application sont disponibles <a href="https://github.com/NicolasFrd/Ptimulus">sur le projet Github</a>.

## Prise de photos

La prise de photos devait initialement être également assurée par l'application Ptimulus mais le temps a manqué pour implémenter cette fonctionnalité. 
La prise de photo fut donc assuré par un logiciel annexe: <a href="https://code.google.com/p/rrtimelapse/">rrtimelapse</a>.
Cette application a la particularité d'assurer une prise de photo automatique en tâche de fond, c'est à dire sans requérir la moindre interaction avec l'utilisateur du téléphone.
Hélas, l'application ne s'est pas avéré être un modèle de stabilité et a cessé de fonctionner à l'altitude d'environ 16 kilomètres. 
Il s'agit bien évidement de l'une des pistes d'amélioration principales pour Ptimulus 2.

## Logiciels équivalents

Il n'existe à notre connaissance qu'un seul projet open-source similaire pour la plateforme Android: <a href="https://www.noisebridge.net/wiki/icarus">Icarus</a>, partie logicielle du projet [Spacebridge](https://www.noisebridge.net/wiki/spacebridge).
