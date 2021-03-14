# FFmpeg

**SOMMAIRE**
+ [Changer de format (sans ré-encodage)](#changer-de-format-sans-ré-encodage)
+ [Extraire la partie audio d'une vidéo](#extraire-la-partie-audio-dune-vidéo)

---

## Changer de format (sans ré-encodage)

```powershell
ffmpeg -i video.mp4 -c copy video.avi
```

## Extraire la partie audio d'une vidéo

```powershell
ffmpeg -i video.mp4 audio.mp3
```
