# FFmpeg

**SOMMAIRE**
+ [Changer de format (sans ré-encodage)](#changer-de-format-sans-ré-encodage)
+ [Convertir un fichier](#convertir-un-fichier)
+ [Couper le son d'une vidéo]()
+ [Extraire la partie audio d'une vidéo](#extraire-la-partie-audio-dune-vidéo)

---

## Changer de format (sans ré-encodage)

```powershell
ffmpeg -i video.mp4 -c copy video.avi
```

## Convertir un fichier

```powershell
ffmpeg -i musique.wav musique.mp3
ffmpeg -i video.avi video.mp4
```

## Couper le son d'une vidéo

```powershell
ffmpeg -i video.mp4 -vcodec copy -an out.mp4
```

## Extraire la partie audio d'une vidéo

```powershell
ffmpeg -i video.mp4 audio.mp3
```
