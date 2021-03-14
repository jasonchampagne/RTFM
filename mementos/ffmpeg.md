# FFmpeg

**SOMMAIRE**
+ [Changer de format (conteneur) sans ré-encodage](#changer-de-format-conteneur-sans-ré-encodage)
+ [Convertir un fichier](#convertir-un-fichier)
+ [Couper l'audio d'une vidéo](#couper-laudio-dune-vidéo)
+ [Extraire la partie audio d'une vidéo](#extraire-la-partie-audio-dune-vidéo)
+ [Lister tous les codecs](#lister-tous-les-codecs)
+ [Lister tous les encodeurs](#lister-tous-les-encodeurs)
+ [Lister tous les décodeurs](#lister-tous-les-décodeurs)
+ [Lister tous les formats (conteneurs)](#lister-tous-les-formats-conteneurs)

---

## Changer de format (conteneur) sans ré-encodage

```powershell
ffmpeg -i video.mp4 -c copy video.avi
```

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
