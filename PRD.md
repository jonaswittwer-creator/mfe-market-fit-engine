# PRD: MFE – Market Fit Engine (Klickdummy v1)

Stand: 20.10.2026 · Grundlage: briefing.md

## 1. Ziel
MFE zeigt als klickbarer Prototyp, wie ein Business Consultant im Dialog mit einer KI in wenigen Schritten zu einer begründeten Markteintritts-Empfehlung für den Vorstand kommt.

## 2. Zielgruppe
- **Nutzer:** Lukas, New Business Consultant (Vertrieb/Marketing) bei „Farbwerk Berlin" (fiktiv). Er klickt sich durch das Tool und bereitet die Entscheidung vor.
- **Empfänger:** Vorstand/Geschäftsführung. Sieht am Ende die Empfehlung als 8-Folien-Vorschau.

## 3. Nicht-Ziele
- Keine echte KI. Der Dialog besteht aus festen Texten.
- Keine echten Marktdaten. Alle Zahlen sind Demo-Daten.
- Kein echter Login, keine Nutzerkonten. Attrappe mit Demo-Passwort `12345678`.
- Kein echter Export (PowerPoint/PDF), nur eine Vorschau.
- Nicht für Mobilgeräte optimiert, nur lesbar.
- Keine echte Firma, keine Kundendaten, keine Mehrsprachigkeit.

## 4. Annahmen
- **Märkte im Vergleich:** Niederlande, Frankreich, Schweden, Polen, Spanien.
- **Kriterien:** Kaufkraft, Nachfrage nach Öko-Produkten, Wettbewerbsdichte, Markteintrittsbarrieren, kulturelle Nähe.
- **Empfohlener Markt:** Niederlande (Demo-Begründung: hohe Öko-Nachfrage, hohe Kaufkraft, geringe Eintrittsbarrieren, kulturelle Nähe). Kann später geändert werden.
- **Technik:** statisches HTML/CSS, ein HTML-Dokument pro Screen, verlinkt über Buttons, gehostet auf GitHub Pages.

## 5. Screens (Version 1)
1. Onboarding mit Login-Attrappe
2. Produktdefinition
3. KI-Erstgespräch
4. Marktvergleich
5. KI-Empfehlung
6. Präsentationsvorschau

## 6. Akzeptanzkriterien

### Ablauf
- **A1** Von Screen 1 aus erreicht man über „Weiter"-Buttons alle 6 Screens der Reihe nach.
- **A2** Jeder Screen hat einen „Zurück"-Button (außer Screen 1).
- **A3** Eine Fortschrittsanzeige zeigt auf jedem Screen „Schritt X von 6".

### Screen 1: Onboarding
- **S1.1** Ein Login-Feld mit vorausgefülltem Demo-Passwort; der Klick auf „Anmelden" führt zu Screen 2.
- **S1.2** Ein Satz erklärt in max. 25 Wörtern, was MFE leistet.

### Screen 2: Produktdefinition
- **S2.1** Die 3 USPs der Produktlinie sind sichtbar.
- **S2.2** Ein Ziel ist formuliert (z. B. „Ersten Auslandsmarkt für die Öko-Linie finden").

### Screen 3: KI-Erstgespräch
- **S3.1** Mindestens 4 Chat-Bubbles im Wechsel KI/Lukas.
- **S3.2** Die KI stellt mindestens eine Rückfrage zu Prioritäten und fasst am Ende zusammen.

### Screen 4: Marktvergleich
- **S4.1** Eine Tabelle oder Grafik vergleicht 5 Märkte anhand von 5 Kriterien.
- **S4.2** Jeder Markt hat eine Gesamtbewertung; der beste Markt ist hervorgehoben.
- **S4.3** Unter der Tabelle steht eine Quellenangabe mit dem Hinweis „Demo-Daten".

### Screen 5: KI-Empfehlung
- **S5.1** Ein Markt wird klar empfohlen.
- **S5.2** Genau 3 Gründe dafür und mindestens 2 Risiken sind genannt.
- **S5.3** Mindestens eine Annahme ist als „Annahme" gekennzeichnet.

### Screen 6: Präsentationsvorschau
- **S6.1** 8 Folien sind als Vorschau sichtbar, jede mit Titel.
- **S6.2** Ein Button „Exportieren" ist vorhanden und zeigt den Hinweis „In der Demo nicht verfügbar".

### Allgemein
- **G1** Alle Texte sind auf Deutsch.
- **G2** Die Farben stimmen mit design.md überein (Anthrazit-Basis, Petrol/Violett/Cyan-Akzente).
- **G3** Text ist gut lesbar: Schrift mindestens 16 px, ausreichender Kontrast.
- **G4** Bei 1440 px Breite gibt es kein horizontales Scrollen. Auf dem Handy ist der Text lesbar.
- **G5** Auf jedem Screen mit Zahlen ist der Hinweis „Demo-Daten" sichtbar.
- **G6** Alle Buttons und Links lassen sich mit der Tab-Taste erreichen.
- **G7** Die Seite läuft ohne Fehlermeldung über die GitHub-Pages-Adresse.