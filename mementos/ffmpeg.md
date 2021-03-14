# FFmpeg

**SOMMAIRE**
+ [Changer de format (conteneur) sans ré-encodage](#changer-de-format-sans-ré-encodage)
+ [Convertir un fichier](#convertir-un-fichier)
+ [Couper l'audio d'une vidéo](#couper-laudio-dune-vidéo)
+ [Extraire la partie audio d'une vidéo](#extraire-la-partie-audio-dune-vidéo)
+ [Lister tous les codecs](#lister-tous-les-codecs)

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
