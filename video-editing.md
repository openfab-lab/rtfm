#Video editing capabilities
## cameras
So we use in the a lab a security cam "YI1080p home camera 2"   
https://www.yitechnology.com/yi-1080p-home-camera-2

130° d'angle de vue, top pour la documentation mais l'image est un peu "crispy" et la focale est fixe. En attendant mieux, c'est pas mal du tout.

## files
### merging
Mettre ce script dans un fichier .bat à la racine du dossier à joindre. Il faut s'assurer d'avoir ffmpeg quelque part et pointer le script vers son emplacement.

```
:: Edit the line below to match your path to the ffmpeg executable.
set path2exe=C:\example\ffmpeg.exe
(for %%i in (*.mp4) do @echo file '%%i') > list.txt
%path2exe% -f concat -i list.txt -c copy output.mp4
del list.tx
```

### converting

ffmpeg, le codec pour le mp4:  
https://ffmpeg.zeranoe.com/forum/viewtopic.php?t=2572

## soft
### streaming
#### obs studio
https://obsproject.com/fr  
Partagez votre jeu, l’art et le divertissement avec le monde.
#### twitch
#### Youtube

### editing
#### DaVinci Resolve
pas opensource mais puissant et version gratuite
>Resolve 15… ce sont des centaines d’améliorations : interface, ergonomie, puissance / rapidité, fonctionalités en workflow, montage, audio et étalonnage bien entendu.  
Et puis, Resolve 15, c’est l’intégration de Fusion, un nouvel outil.. énorme !   
https://www.video-d.com/davinci-resolve-15/

https://www.blackmagicdesign.com/products/davinciresolve
