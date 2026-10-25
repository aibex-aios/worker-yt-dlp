# worker-yt-dlp

Arbeitspferd von AIbex AIOS (Typ `worker`, Version 0.1.0): [yt-dlp](https://github.com/yt-dlp/yt-dlp) 2026.10.21 mit den Extras `[default]` (11 Pakete), installiert aus PyPI mit Hashes. Die JS-Runtime für YouTube kommt aus `worker-deno` (`depends`).

## Holen

**Voraussetzung:** AIbex AIOS v0.5 ist installiert und das Projekt aktiviert.

```bash
aios --fetch worker-yt-dlp
```

Der Plan zeigt alle Pakete mit Version und richtet `worker-deno` zuerst ein. Aufruf über den Weiterleiter `~/.aios/bin/yt-dlp`; er nimmt die Version, die `lock.yaml` des nächsten Projekts der Kette sperrt, und findet `deno` über `~/.aios/bin`.

## Grenzen

`ffmpeg` gehört nicht dazu; `yt-dlp` warnt ohne `ffmpeg` und kann dann Formate nicht zusammenführen.

## Lizenz

Das Paket steht unter der Apache License 2.0 (`LICENSE`, `NOTICE`). yt-dlp selbst ist gemeinfrei (Unlicense).
