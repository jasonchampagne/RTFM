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
+ [Extraire la partie audio d'une vidéo](#extraire-la-partie-audio-dune-vidéo)
+ [Extraire une partie de fichier, sans ré-encodage](#extraire-une-partie-de-fichier-sans-ré-encodage)
+ [Lister tous les codecs](#lister-tous-les-codecs)
+ [Lister tous les encodeurs](#lister-tous-les-encodeurs)
+ [Lister tous les décodeurs](#lister-tous-les-décodeurs)
+ [Lister tous les formats (conteneurs)](#lister-tous-les-formats-conteneurs)

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

## Extraire la partie audio d'une vidéo

```powershell
ffmpeg -i video.mp4 audio.mp3
```

## Extraire une partie de fichier, sans ré-encodage

```powershell
ffmpeg -i video.flac -ss <hour_begin>:<minute_begin>:<second_begin> -c copy -to <hour_end>:<minute_end>:<second_end> out.flac
```
+ `<hour_begin>` et `<hour_end>` : heure de début et heure de fin
+ `<minute_begin>` et `<minute_end>` : minute de début et minute de fin
+ `<second_begin>` et `<second_end>` : seconde de début et seconde de fin

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
