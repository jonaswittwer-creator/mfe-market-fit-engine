# Briefing: MFE – Market Fit Engine

Stand: 20.10.2026 · Projekt: Klickdummy für den Kurs „Agentic Engineering"

## Ziel
MFE zeigt als klickbarer Prototyp, wie ein Business Consultant im Dialog mit einer KI in wenigen Schritten zu einer begründeten Markteintritts-Empfehlung für den Vorstand kommt.

**Leitidee:** MFE liefert nicht nur Marktdaten – MFE unterstützt fundierte Markteintrittsentscheidungen.

## Zielgruppe
- **Nutzer:** Lukas, New Business Consultant (Vertrieb/Marketing) bei einem Farben- und Lackhersteller in Berlin. Er bedient das Tool und bereitet die Entscheidung vor.
- **Empfänger:** Geschäftsführung/Vorstand. Erhält am Ende eine Empfehlung als Präsentation (8 Folien).
- **Was Lukas danach tun soll:** Mit einer klar begründeten Empfehlung für einen Zielmarkt in die Vorstandssitzung gehen.

## Produkt (fiktiv)
Firma: „Farbwerk Berlin" (fiktiv). Neue Lack- und Farbenlinie mit drei USPs:
- 100 % ökologische Herstellung
- Selbstreinigende Oberfläche, Schutz vor Schmutz
- Lebenslange Farbqualität: keine Vergilbung, kein Abblättern

## Entscheidungen
1. **Format:** Statischer Klickdummy (HTML/CSS), veröffentlicht über GitHub Pages.
2. **Umfang Version 1:** 6 Screens
   1. Onboarding (mit Login-Attrappe)
   2. Produktdefinition
   3. KI-Erstgespräch
   4. Marktvergleich
   5. KI-Empfehlung
   6. Präsentationsvorschau (8 Folien)
3. **Später (je ein Branch + Pull Request):** die übrigen 10 Screens aus dem Gesamtkonzept: Projektübersicht, Marktscreening, KI-Dialog Kriterien, Daten und Quellen, Shortlist, Deep-Dive I + II, Review, Export, ausführliches Login.
4. **KI-Dialog:** simuliert mit festen Texten in Chat-Bubbles. Tonalität: empathisch, beratend statt belehrend, schrittweise, nicht überfordernd.
5. **Design:** Desktop-Web-App (1440 px). Grundfarbe Anthrazit/Blauschwarz, Akzente Petrol, Violett und Cyan mit dezentem Neon. Minimalistische B2B-SaaS-Ästhetik, Dashboards und Vergleichsansichten. Oberfläche komplett auf Deutsch.
6. **Entscheidungsqualität sichtbar machen:** Vergleich der Märkte, gekennzeichnete Annahmen und Unsicherheiten, angegebene Quellen (Demo), Chancen gegen Risiken, klare Empfehlung.

## Nicht-Ziele
- Keine echte KI-Anbindung, der Dialog ist vorgeschrieben.
- Keine echten Marktdaten. Alle Zahlen sind Beispieldaten und als „Demo-Daten" gekennzeichnet.
- Kein echter Login. Attrappe mit vorausgefülltem Demo-Passwort `12345678`, keine Nutzerkonten.
- Kein echter Export (PowerPoint/PDF), nur eine Folienvorschau.
- Nicht für Mobilgeräte optimiert. Auf dem Handy muss die Seite aber lesbar sein.
- Keine echte Firma, keine echten Kundendaten.
- Keine Mehrsprachigkeit, nur Deutsch.

## Offene Fragen
1. Welche Länder kommen in den Marktvergleich? Vorschlag: Niederlande, Frankreich, Schweden, Polen, Spanien.
2. Welcher Markt wird am Ende empfohlen, und mit welcher Hauptbegründung?
3. Welche 4 bis 6 Kriterien zählen im Marktvergleich? Vorschlag: Kaufkraft, Nachfrage nach Öko-Produkten, Wettbewerbsdichte, Markteintrittsbarrieren, kulturelle Nähe.

## Nächste Schritte
1. Briefing speichern (briefing.md).
2. In claude.ai ein Projekt anlegen, Briefing hochladen, PRD schreiben lassen. Als PRD.md speichern.
3. Im Claude-Panel tech-spec.md und design.md erzeugen, danach /init für CLAUDE.md.