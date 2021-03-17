# FFmpeg

💠 _Les commandes de FFmpeg affichent généralement la version de ce dernier_

![Logo de FFmpeg](https://nsa40.casimages.com/img/2021/03/14/210314041423969272.png)

**SOMMAIRE**
+ [Afficher les informations d'un fichier](#afficher-les-informations-dun-fichier)
+ [Changer de format (conteneur), sans ré-encodage](#changer-de-format-conteneur-sans-ré-encodage)
+ [Changer la résolution d'une vidéo](#changer-la-résolution-dune-vidéo)
+ [Compresser un fichier audio](#compresser-un-fichier-audio)
+ [Convertir un fichier](#convertir-un-fichier)
+ [Couper l'audio d'une vidéo](#couper-laudio-dune-vidéo)
+ [Diviser un fichier en deux parties](#diviser-un-fichier-en-deux-parties)
+ [Extraire des images d'une vidéo](#extraire-des-images-dune-vidéo)
+ [Extraire la partie audio d'une vidéo](#extraire-la-partie-audio-dune-vidéo)
+ [Extraire une partie de fichier, sans ré-encodage](#extraire-une-partie-de-fichier-sans-ré-encodage)
+ [Lister tous les codecs](#lister-tous-les-codecs)
+ [Lister tous les encodeurs](#lister-tous-les-encodeurs)
+ [Lister tous les décodeurs](#lister-tous-les-décodeurs)
+ [Lister tous les formats (conteneurs)](#lister-tous-les-formats-conteneurs)
+ [Rogner une vidéo](#rogner-une-vidéo)

---

## Afficher les informations d'un fichier

```powershell
ffmpeg -i <file> -hide_banner
```

## Changer de format (conteneur), sans ré-encodage

```powershell
ffmpeg -i video.mp4 -c copy video.avi
```

## Changer la résolution d'une vidéo

```powershell
ffmpeg -i video.mp4 -s <width>x<height> -c:a copy output.mp4
```
+ `<width>` : largeur (pixels)
+ `<height>` : hauteur (pixels)

## Compresser un fichier audio

```powershell
ffmpeg -i audio.ogg -ab <bitrate> output.ogg
```
+ `<bitrate>` : débit (kbps)

## Convertir un fichier

```powershell
ffmpeg -i musique.wav musique.mp3
ffmpeg -i video.avi video.mp4
```

## Couper l'audio d'une vidéo

```powershell
ffmpeg -i video.mp4 -vcodec copy -an out.mp4
```

## Diviser un fichier en deux parties

```powershell
ffmpeg -i video.mp4 -t <p1_end> -c copy p1.mp4 -ss <p2_begin> -codec copy p2.mp4
```
+ `<p1_end>` : fin de la première partie, depuis le début du fichier (_heure:minute:seconde_)
+ `<p2_begin>` : début de la seconde partie, jusqu'à la fin du fichier (_heure:minute:seconde_)

## Extraire des images d'une vidéo

```powershell
ffmpeg -i video.avi -r <fps> -f image2 <format_name>.png
```
+ `<fps>` : fréquence d'images par seconde de vidéo
+ `<format_name>` : format du nommage des images (_ex : %3d.png produira des images numérotées à 3 chiffres_)

## Extraire la partie audio d'une vidéo

```powershell
ffmpeg -i video.mp4 audio.mp3
```

## Extraire une partie de fichier, sans ré-encodage

```powershell
ffmpeg -i video.flac -ss <h_begin>:<m_begin>:<s_begin> -c copy -to <h_end>:<m_end>:<s_end> out.flac
```
+ `<h_begin>` et `<h_end>` : heure de début et heure de fin
+ `<m_begin>` et `<m_end>` : minute de début et minute de fin
+ `<s_begin>` et `<s_end>` : seconde de début et seconde de fin

## Lister tous les codecs

```powershell
ffmpeg -codecs
```

## Lister tous les encodeurs

```powershell
ffmpeg -encoders
```

## Lister tous les décodeurs

```powershell
ffmpeg -decoders
```

## Lister tous les formats (conteneurs)

```powershell
ffmpeg -formats
```

## Rogner une vidéo

```powershell
ffmpeg -i video.mp4 -filter:v "crop=<width>:<height>:<origin_x>:<origin_y>" output.mp4
```
+ `<width>` : largeur de la vidéo recadrée
+ `<height>` : hauteur de la vidéo recadrée
+ `<origin_x>` et `<origin_y>` : coordonnées d'origine du recadrage
