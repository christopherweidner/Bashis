# Bashi's Gemüsekebab – Website

Statische Website für **Bashi's Gemüsekebab** (Brandenburger Straße 27, 14467 Potsdam).
Reines HTML/CSS – keine Build-Tools, keine Abhängigkeiten, kein Framework.

## Dateistruktur

```
bashis-website/
├── index.html        # Startseite (Menü, Galerie, Bewertungen, Anfahrt)
├── impressum.html    # Impressum (§ 5 DDG)
├── datenschutz.html  # Datenschutzerklärung (DSGVO)
├── README.md         # Diese Datei
└── assets/           # Bilder, Favicon usw.
```

## Lokale Vorschau

Am einfachsten: `index.html` per Doppelklick im Browser öffnen.

Alternativ mit einem lokalen Server (empfohlen, z. B. für korrekte Pfade):

```bash
npx serve
```

Danach die angezeigte Adresse (z. B. http://localhost:3000) im Browser öffnen.

## Deployment auf Vercel

Es ist keine Konfiguration nötig – Vercel erkennt die statische Seite automatisch.

**Variante 1: Vercel CLI**

```bash
npm i -g vercel
cd bashis-website
vercel          # zum Testen (Preview)
vercel --prod   # für die Live-Version
```

**Variante 2: Drag & Drop**

Auf [vercel.com](https://vercel.com) einloggen, „Add New → Project" wählen und den
Ordner `bashis-website` einfach per Drag & Drop hochladen.

## Vor dem Livegang zu ersetzen (Checkliste für den Kunden)

- [ ] **Platzhalter-Fotos in der Galerie** durch echte Fotos des Restaurants und der Gerichte ersetzen (Ordner `assets/`).
- [ ] **Telefonnummer** überall eintragen (Startseite, Impressum, Datenschutzerklärung – Platzhalter `[Telefonnummer]`).
- [ ] **E-Mail-Adresse** eintragen (Platzhalter `[E-Mail-Adresse]`).
- [ ] **Impressum:** Umsatzsteuer-Identifikationsnummer eintragen (Platzhalter `[USt-IdNr.]`) bzw. den Abschnitt entfernen, falls keine vorhanden ist.
- [ ] **Datenschutzerklärung** prüfen und ggf. an tatsächlich eingesetzte Dienste anpassen.
- [ ] **Bewertungen auf der Startseite:** Die Zitate sind Beispiel-Platzhalter und müssen durch echte Google-Rezensionen ersetzt werden.

## Hinweise

- Farben: Creme `#F9E5D8`, Dunkelrot `#7A1E24`, Rot `#C73C43`
- Schriften: „Baloo 2" (Überschriften) und „Jost" (Fließtext) via Google Fonts
- Instagram: [@bashiskebab](https://www.instagram.com/bashiskebab)
