---
description: Installation et usage
---

# Silhouette Cameo 3
[Usage machine](https://www.youtube.com/watch?v=Wa69jf0gaIg)
## Linux and Inkscape
La machine se gère via un plugin Illustrator ou une app propriétaire.  
Sauf que je suis sous linux Manjaro, problem?  
Nope.  
C'est sans compter sur les formidables ressources des fablabs. :)

### extension to drive Silhouette vinyl cutters 
(e.g. Cameo, Portrait series) from within inkscape
[fablabnbg/inkscape-silhouette](https://github.com/fablabnbg/inkscape-silhouette)

To install With [Awesome sauce for Arch ](https://github.com/fablabnbg/inkscape-silhouette#arch-linux)  
- Je check si j'ai bien les dépendances logicielles
  - [x] python2
  - [x] python2-lxml
  - [x] python2-pyusb

- Je clone en local le git.
- Je build le script qui va bien et copie dans les extensions d'inkscape et voilà. 

![image](https://user-images.githubusercontent.com/12049360/77317710-faeb1680-6d0b-11ea-85e9-a195e12508df.png)

### Usage et réglage de base. 
Comme pour le laser, mise en place sur une référence en haut à gauche. 
Plaque 12'x12' = 30x30cm. 

On sélectionne le chemin à couper. _note: les chemins non sélectionné ne sont pas envoyé à la machine_
![image](https://user-images.githubusercontent.com/12049360/77316772-4a304780-6d0a-11ea-8109-ce978833a938.png)

J'ai mis un petit offset mais ça peut se prévoir dans le svg.
Mais bon, en gros, j'ai suivit [le tuto de base](https://github.com/fablabnbg/inkscape-silhouette#usage)

![image](https://user-images.githubusercontent.com/12049360/77316829-646a2580-6d0a-11ea-810d-150991008bf3.png)
