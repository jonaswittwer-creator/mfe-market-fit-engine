# Design: MFE Klickdummy

## Ansprache
Durchgängig Siezen („Sie"), nie Duzen.

## Typografie
Eine serifenlose Schrift (z. B. System-Font-Stack: `-apple-system, Segoe UI, Roboto, sans-serif`), mindestens 16 px Grundgröße für gute Lesbarkeit.

## Farbkonzept
Basis: Anthrazit/Blauschwarz. Akzente: Petrol, Violett, Cyan, jeweils mit dezentem Neon-Effekt (sparsam, z. B. als Glow auf Hover/aktiven Elementen, nicht flächig).

### Farb-Tokens (CSS Custom Properties)
Definiert z. B. in `:root` in `styles.css`:

| Token | Verwendung |
|---|---|
| `--color-bg` | Haupt-Hintergrund, Anthrazit/Blauschwarz |
| `--color-bg-elevated` | Hintergrund für Karten/Panels, etwas heller als `--color-bg` |
| `--color-text` | Primärer Fließtext, hoher Kontrast zu `--color-bg` |
| `--color-text-muted` | Sekundärtext (z. B. „Demo-Daten"-Hinweise) |
| `--color-accent-petrol` | Akzentfarbe Petrol |
| `--color-accent-violet` | Akzentfarbe Violett |
| `--color-accent-cyan` | Akzentfarbe Cyan |
| `--color-glow` | Neon-Glow-Farbe für Hover-/Fokuszustände (meist cyan-basiert) |
| `--color-border` | Dezente Rahmenfarbe auf dunklem Grund |

## Seitenstruktur (6 Screens)
1. **Onboarding** – Login-Attrappe, Kurzerklärung MFE in max. 25 Wörtern.
2. **Produktdefinition** – 3 USPs, formuliertes Ziel.
3. **KI-Erstgespräch** – Chat-Bubbles (KI/Lukas im Wechsel), Rückfrage + Zusammenfassung.
4. **Marktvergleich** – Tabelle/Grafik mit 5 Märkten × 5 Kriterien, Gesamtbewertung, bester Markt hervorgehoben, Quellenhinweis „Demo-Daten".
5. **KI-Empfehlung** – Empfohlener Markt, genau 3 Gründe, mindestens 2 Risiken, mindestens 1 gekennzeichnete Annahme.
6. **Präsentationsvorschau** – 8 Folien-Vorschau mit Titeln, „Exportieren"-Button mit Hinweis „In der Demo nicht verfügbar".

Jeder Screen zeigt eine Fortschrittsanzeige „Schritt X von 6". Zahlenbasierte Inhalte tragen sichtbar den Hinweis „Demo-Daten". Barrierefreiheit: Alle Buttons/Links per Tab erreichbar, ausreichender Kontrast auch bei Neon-Akzenten.
