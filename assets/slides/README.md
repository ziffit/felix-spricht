# Folien

Präsentationsdateien hier ablegen. Dateinamen müssen im Feld `files` in `_data/talks.yml` registriert sein.

## Struktur

Die Folien werden in `_data/talks.yml` über ein `files`-Array definiert:

```yaml
- id: my-talk
  title: "Mein Talk-Titel"
  files:
    - label: "Folien"
      file: "my-talk.pdf"
    - label: "Demo-Code"
      file: "my-talk-code.zip"
```

Jeder Eintrag im `files`-Array kann folgende Felder enthalten:

- **file** (erforderlich): Der Name der Datei im `assets/slides/` Verzeichnis
- **label** (optional): Ein aussagekräftiger Name für den Download-Button (z.B. "Folien", "Handout", "Demo-Code")

## Kompatibilität

Das alte `slides_file`-Feld ist veraltet und wird durch das neue `files`-Array-Modell ersetzt. Dies ermöglicht mehrere Dateien pro Talk (z.B. Folien + Handout + Code-Beispiele).