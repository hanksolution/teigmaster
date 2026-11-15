# Hankeln's Kitchen Teigmaster

Pizzateig-Rechner als Web-App. Läuft komplett im Browser, ohne Server und ohne Datensammlung.

**Aufs iPhone holen:** Seite in Safari öffnen → Teilen → „Zum Home-Bildschirm“. Danach startet der Teigmaster wie eine App und funktioniert auch offline.

## Wie gerechnet wird
- Mehl, Wasser, Salz: Bäckerprozente vom Mehl.
- Frischhefe (g) = 1,10 × e^1,86072 × Mehl^0,89178 × Gehzeit^−1,44084 × e^(−0,18603 × Raumtemperatur)
  (an 13 Vergleichswerten gefittet, plus 10 % Zuschlag).
- ATH ×0,5497, ITH ×0,444, Lievito Madre fest ×66,07 (50 % Hydration), flüssig ×50,11 (100 %); Mehl und Wasser des Lievito Madre werden vom Hauptteig abgezogen.

## Update veröffentlichen
Dateien ändern, in `sw.js` die `VERSION` hochzählen, committen. GitHub Pages veröffentlicht automatisch.
