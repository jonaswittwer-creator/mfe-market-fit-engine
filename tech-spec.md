# Tech-Spec: MFE Klickdummy

## Stack
- Statisches HTML + CSS. Kein Framework, kein Build-Step, kein JavaScript erforderlich.
- Hosting: GitHub Pages.

## Dateistruktur
```
index.html                     Screen 1 – Onboarding
produktdefinition.html         Screen 2
ki-erstgespraech.html          Screen 3
marktvergleich.html            Screen 4
ki-empfehlung.html             Screen 5
praesentationsvorschau.html    Screen 6
styles.css                     Gemeinsames Stylesheet für alle Screens
```

## Navigation
- Jeder Screen verlinkt per normalem `<a href="...">` zum nächsten/vorherigen Screen (kein JS-Routing).
- „Weiter"-Button → nächste Datei in der Reihenfolge oben.
- „Zurück"-Button → vorherige Datei (fehlt auf Screen 1).
- Fortschrittsanzeige „Schritt X von 6" ist reiner Text/Markup, kein dynamischer State.

## Grenzen
- Login, KI-Dialog, Marktdaten und Export sind statische Inhalte – keine Logik, keine Formularverarbeitung.
- Alle Inhalte deutschsprachig.
