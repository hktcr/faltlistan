# Fältlistan — Digital Krysslista 🐦

En standalone digital krysslista för fågelskådning, byggd som en enda HTML-fil utan externa beroenden.

## Funktioner

- **Multi-column grid** med ~260 arter i taxonomisk ordning (Sverigelistan)
- **Tap-to-check** — ett klick markerar arten
- **Kommentarmodal** — klicka igen för antal, fritext, Årskryss-flagga
- **Realtidssökning** på svenskt/latinskt namn
- **"Ingen träff → Lägg till"** för arter som saknas på listan
- **localStorage auto-save** — utkast sparas automatiskt, återställs vid omladdning
- **JSON-export** — System C-kompatibelt format med kopiera-till-clipboard
- **Haptic feedback** vid kryss (Android)
- **Offline-resilient** — system-fonter, inga externa beroenden

## Användning

1. Öppna [hktcr.github.io/faltlistan](https://hktcr.github.io/faltlistan) på telefonen
2. Fyll i datum + lokal
3. Kryssa arter under exkursionen
4. Klicka **Generera** → **Kopiera**
5. Klistra in i gAIa-chat → `/krysslista`-workflow

## Exportformat

```json
{
    "version": "1.0",
    "date": "2026-03-03",
    "location": "Åstorps kommun",
    "species": [
        { "name": "Grågås", "latin": "Anser anser", "count": 1, "flags": [] },
        { "name": "Skedand", "latin": "Spatula clypeata", "count": 8, "flags": ["Årskryss"] }
    ],
    "source": "faltlistan"
}
```

## Licens

Privat verktyg.
