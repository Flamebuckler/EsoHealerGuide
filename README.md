# ESO Heilerguide

Ein Heilerguide für The Elder Scrolls Online, gebaut mit [MkDocs](https://www.mkdocs.org/) und dem [Material](https://squidfunk.github.io/mkdocs-material/)-Theme.

🔗 **Live:** https://flamebuckler.github.io/EsoHealerGuide/

## Lokale Vorschau

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
mkdocs serve
```

Die Seite ist danach unter `http://127.0.0.1:8000/EsoHealerGuide/` erreichbar und lädt bei Änderungen an `docs/` oder `mkdocs.yml` automatisch neu.

## Struktur

- `docs/` – Inhalt der Seiten (Markdown), die Navigation wird in `mkdocs.yml` unter `nav:` definiert
- `mkdocs.yml` – Konfiguration (Theme, Navigation, Markdown-Erweiterungen)
- `.github/workflows/deploy.yml` – deployt bei jedem Push auf `main` automatisch auf GitHub Pages

## Deployment

Das Deployment läuft automatisch über GitHub Actions. Ein Push auf `main` baut die Seite und veröffentlicht sie via `mkdocs gh-deploy` auf GitHub Pages.
