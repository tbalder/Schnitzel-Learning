# Schnitzel Learning

Woordjes leren met herhaling en vrij oefenen. Werkt als app: installeerbaar op telefoon, tablet en computer, en ook zonder internet.

## Als app installeren

De app moet eerst op een echte link staan (zie `DELEN.md`, bijvoorbeeld GitHub Pages). Open die link daarna:

- **iPhone/iPad (Safari):** Deel-knop → *Zet op beginscherm*
- **Android (Chrome):** menu (⋮) → *App installeren* of *Toevoegen aan startscherm*
- **Computer (Chrome/Edge):** installeer-icoon rechts in de adresbalk

Lokaal proberen kan ook: dubbelklik op `index.html`. Installeren en offline werken gaan dan niet, want dat vereist een link (https).

## Wat zit erin

- Herhalen met wachttijd tussen kaartjes, zoals Anki.
- Vrij oefenen wanneer je wilt, zoals StudyGo.
- Kies tussen kaartjes bekijken of antwoorden typen.
- Bij typen wordt de eerste letter getoond en telt een antwoord met 1 letter verschil nog als goed.
- Bibliotheek met lege boeken voor:
  - Frans Libre Service 2 VWO
  - Pallas Griekse taal en letterkunde
  - Zugspitze Duits
  - Minerva Latijn
- Je voegt hoofdstukken zelf toe bij import.
- Elk woordpaar wordt opgeslagen als: woord in de taal -> Nederlandse betekenis.
- Bij oefenen en herhalen kun je kiezen tussen Taal -> NL en NL -> taal.

## Woordjes toevoegen

Ga naar `Nieuw` en plak twee kolommen:

```text
Woord in de taal	Nederlandse betekenis
la pomme	de appel
le sucre	de suiker
```

Complete woordenlijsten uit schoolboeken staan er niet vooraf in, omdat die uit jouw eigen boeken of eigen exports moeten komen.

## Bestanden

- `index.html`, `app.js`, `styles.css`: de app zelf
- `manifest.webmanifest`: naam, kleuren en iconen voor installatie
- `sw.js`: service worker, bewaart de app voor offline gebruik
- `icons/`, `icon.svg`: app-iconen

## Nieuwe versie uitrollen

Pas je iets aan, verhoog dan `CACHE_VERSION` bovenin `sw.js` (bijv. `schnitzel-v2`). Anders blijven bestaande gebruikers de oude versie uit hun cache zien.
