# Video editing capabilities
This chapter is about audio/video.  
Ecrire est parfois un frein à la documentation.  
Avoir un setup de documentation video au lab, pour réaliser les tutos et peut-être faciliter le partage des skills.     

L'objectif serait de pouvoir faire du broadcast de projet ou du podcast de discussion.  

[Exemple de setup](https://www.youtube.com/watch?v=st1r4QIEEwk)  
[BEST MIC SETTINGS FOR OBS](https://www.youtube.com/watch?v=MU00vRXWXmA)  
[Lighting Guide for Live Streamers](https://www.youtube.com/watch?v=mhIKPl-2aRw)  
## cameras
So we use in the a lab a security cam ["YI1080p home camera 2"](https://www.yitechnology.com/yi-1080p-home-camera-2)

130° d'angle de vue, top pour la documentation mais l'image est un peu "crispy" et la focale est fixe. En attendant mieux, c'est pas mal du tout.

## files
### merging
Mettre ce script dans un fichier .bat à la racine du dossier à joindre.  
Il faut s'assurer d'avoir ffmpeg quelque part et pointer le script vers son emplacement.

```
:: Edit the line below to match your path to the ffmpeg executable.
set path2exe=C:\example\ffmpeg.exe
(for %%i in (*.mp4) do @echo file '%%i') > list.txt
%path2exe% -f concat -i list.txt -c copy output.mp4
del list.tx
```

### converting

[ffmpeg](https://ffmpeg.zeranoe.com/forum/viewtopic.php?t=2572), le codec pour le mp4  


## soft
### streaming
Pour une diffusion de contenu live, il faut distinguer 2 étapes séparées.  
1. le layout, ou habillage d'écran. Le plus souvent avec OBS, on compose le contenu de la diffusion. Titre, ecran de pause, chat, mixage multicam et greenkey (fond vert).
2. la platerforme de streaming, de diffusion. Soit twitch ou youtube dans notre cas.  

#### obs studio
[site officiel obs-project](https://obsproject.com/fr)  
>Partagez votre jeu, l’art et le divertissement avec le monde.  

[Tuto pour créer ses scènes](https://www.youtube.com/watch?v=j2HzbY8E4yQ)
#### twitch
[site officiel](https://www.twitch.tv/)

#### Youtube

### editing
Le montage peut être nécessaire pour une production d'un tuto video plus élaboré.  
Quelques solutions existent, Premiere, Avid, Vegas, etc... bcp de solutions pro et payante.   
Ici, j'ai testé DaVinci et même si j'ai entendu des pros s'en plaindre et se moquer, ma fois, ça marche et c'est gratuit. Très bien pour ce qu'on veut en faire.  

#### DaVinci Resolve
pas opensource mais puissant et version gratuite.  
Mais soucis de format video à l'import.  
>Resolve 15… ce sont des centaines d’améliorations : interface, ergonomie, puissance / rapidité, fonctionalités en workflow, montage, audio et étalonnage bien entendu.  
Et puis, Resolve 15, c’est l’intégration de Fusion, un nouvel outil.. énorme !   
https://www.video-d.com/davinci-resolve-15/

https://www.blackmagicdesign.com/products/davinciresolve

#### KDEnlive
[site officiel](https://kdenlive.org/)  
Bof, j'ai eu des soucis de format video à l'import. J'ai abandonné.
#### Autres pistes Open source à tester:  
- [shotcut](https://shotcut.org/)  
>Shotcut is a free, open source, cross-platform video editor. It supports a ton of audio and video formats and codecs thanks to FFmpeg. This open source video editing tool can do almost all common video editing works that a common video maker or YouTuber needs. The Shotcut multi-track compositing and visual effects may slow down playback during as it not hardware accelerated, however the final version play normally. It supports all popular image formats such as BMP, GIF, JPEG, PNG, SVG, TGA, TIFF as well as image sequences and 4K resolutions. It is the best free alternative video editor to paid Camtasia Video Editor.

- [openshot](https://www.openshot.org/fr/)   
>OpenShot is a free, simple-to-use, feature-rich video editor for Linux, OS X, and Windows. It has the simplest user interface with drag & drop and video effects. If you are totally a newbie to videos editing you can go for this.
