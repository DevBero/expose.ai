# Design: expose.ai

Designsprache der Plattform (App-Oberfläche, Wizard, Konto, Landingpage).
Referenz: **gumloop.com** – analysiert am 07.10.2026 anhand von Screenshots (Desktop 1440 px, Mobile 390 px) und den ausgelesenen CSS-Werten der Seite.

> Gilt für die **Plattform**, nicht für die generierten Exposés. Die Exposés haben ihre eigene Gestaltung (Stil, Farben, Schrift des Maklers).

---

## 1. Charakter in einem Satz

**Ruhige, monochrome Werkzeug-Ästhetik: fast nur Schwarz, Weiß und feine Grautöne, große leichte Headlines, haarfeine Linien, kaum Schatten – Farbe kommt ausschließlich über Inhalte (Produkt-Screens, Icons, Logos), nie über die UI selbst.**

### Leitprinzipien

1. **Monochrom als Bühne.** Die Oberfläche ist neutral, damit das Produkt (bei uns: die Exposé-Vorschau) die Farbe trägt. Gumloop zeigt Farbe nur in Agenten-Icons, Avataren, Logos und Diagrammen.
2. **Produkt statt Illustration.** Statt Stockbildern oder abstrakten Grafiken zeigt die Seite echte, detailreiche UI-Ausschnitte (Fenster mit Ampel-Punkten, Sidebars, Chats, Charts). Das Produkt *ist* die Illustration.
3. **Linien statt Schatten.** Flächen werden durch 1-px-Haarlinien und minimale Grauabstufungen getrennt. Schatten sind so schwach, dass man sie eher spürt als sieht.
4. **Große Typo, wenig Gewicht.** Headlines sind groß, aber nur Medium (500), mit leicht negativer Laufweite – das wirkt selbstbewusst, nicht laut.
5. **Großzügiger Weißraum.** Sektionen atmen mit 120–200 px Abstand. Inhalt sitzt in einem klaren 12-Spalten-Raster mit 40 px Außenrand.
6. **Ein dunkler Akzent-Block.** Genau eine Sektion (Enterprise) kippt in Dunkel. Das setzt einen Rhythmuswechsel, ohne das Gesamtbild zu brechen.

---

## 2. Farben

### Neutrale Basis (trägt 95 % der UI)

| Token | Hex | Verwendung |
|---|---|---|
| `ink` | `#18191B` | Headlines, Fließtext stark, Primär-Button-Fläche, dunkle Sektion |
| `ink-hover` | `#2C2D30` | Hover auf Primär-Button |
| `body-muted` | `#5F5F68` | Fließtext, Beschreibungen (oft mit ~88 % Deckkraft) |
| `neutral-muted` | `#8E8E98` | Meta-Infos, Labels, Datumsangaben, Platzhalter |
| `hairline` | `#E2E2E8` | Rahmen, Trennlinien, Button-Outlines |
| `wash` | `#F4F4F5` | Hintergrund von Produkt-Bühnen und Logo-Kacheln |
| `subtle` | `#F3F3F6` | Aktiver Listeneintrag, Input-Hintergründe |
| `section-bg` | `#F9F9FB` | Seitenhintergrund / sehr helle Flächen |
| `surface` | `#FFFFFF` | Karten, Fenster, Buttons (sekundär) |

### Dunkle Sektion (invertiert)

| Token | Wert | Verwendung |
|---|---|---|
| `inverse-bg` | `#18191B` | Sektionshintergrund |
| `inverse-surface` | `#FFFFFF` @ 5 % | Karten auf Dunkel |
| `inverse-hairline` | `#FFFFFF` @ 14 % | Rahmen auf Dunkel |
| `inverse-body` | `#FFFFFF` @ 68 % | Fließtext auf Dunkel |
| `inverse-muted` | `#9A9AA4` | Meta-Text auf Dunkel |

### Akzentfarben (nur für Inhalte, nie für UI-Chrome)

Gumloop nutzt eine verspielte, gesättigte Palette ausschließlich für Icons, Statuspunkte und Datenvisualisierung:

| Name | Hex |
|---|---|
| Blue | `#0290FF` |
| Purple / Blueberry | `#6E6ADE` / `#7671F9` |
| Pink / Bubblegum | `#DE51A8` / `#FF59AF` |
| Orange / Tangerine | `#ED6142` / `#FF8D00` |
| Yellow | `#FFC200` |
| Green | `#3FCC83` |

Statusfarben folgen demselben Prinzip: kleiner Punkt (8 px) + Text, z. B. Grün „Healthy“, Orange „At risk“, Rot „Failing“.

### Übertragung auf expose.ai

- Die UI bleibt **strikt monochrom** (Ink + Grautöne).
- Farbe entsteht durch die **Live-Vorschau des Exposés** und die Fotos der Immobilie – genau wie Gumloop seine Produkt-Screens als Farbträger nutzt.
- Akzentfarben nur für: Kategorie-Icons der Lageanalyse (Einkaufen, ÖPNV, Sport …), Karten-Pins, Status-Badges (Entwurf / Gekauft / Bearbeitungen übrig) und Erfolgs-/Fehlermeldungen.
- **Keine eigene Markenfarbe als Button-Farbe.** Primär-Aktion ist immer Ink-Schwarz.

---

## 3. Typografie

### Schriften bei Gumloop

| Rolle | Schrift | Charakter |
|---|---|---|
| Display / Headlines | **Gellix** (Medium 500) | Geometrische Grotesk mit runden, freundlichen Formen und markantem „g“ |
| UI / Fließtext | **Geist Sans** (400 / 500) | Neutrale, technische Grotesk, sehr gut lesbar in kleinen Größen |
| Daten / Datum / Code | **Geist Mono** (300 / 500) | Für Zahlen, Datumsangaben („OCT 6, 2026“), Tags |

Gellix ist eine kommerzielle Schrift (Lizenz nötig). Geist Sans und Geist Mono sind frei verfügbar (OFL).

### Schriften für expose.ai (festgelegt)

| Rolle | Schrift | Lizenz |
|---|---|---|
| Display / Headlines | **Plus Jakarta Sans** (Medium 500) | OFL, Google Fonts |
| UI / Fließtext | **Geist Sans** (400 / 500) | OFL |
| Daten / Datum / Zahlen | **Geist Mono** (300 / 500) | OFL |

**Warum Plus Jakarta Sans statt Gellix:** Im direkten Vergleich mit dem Gumloop-Hero kommt sie Gellix am nächsten: zweistöckiges „a“, einstöckiges, rundes „g“, offene Rundungen und eine leicht breite, freundliche Proportion. Getestet wurden außerdem Figtree, Outfit, Urbanist, Manrope, Onest, Instrument Sans und Albert Sans.
**Ausweichoption:** **Figtree** – etwas schmaler und neutraler, ebenfalls OFL.

Für die Plattform-UI gelten nur diese drei Schriften. Die kuratierten Schriften für die *Exposés* sind davon unabhängig.

### Typo-Skala (Desktop)

| Stufe | Größe / Zeilenhöhe | Gewicht | Laufweite | Verwendung |
|---|---|---|---|---|
| Display XL | 48 / 48 px | 500 | −1.2 px (−2.5 %) | H1 Hero |
| Stat | 60 / 60 px | 300 | normal | Große Kennzahlen („1B+“, „326K+“) |
| Display L | 36 / 45 px | 500 | −0.9 px (−2.5 %) | H2 Sektionstitel |
| Title | 24 / 32 px | 500 | −0.6 px | Karten- und Fenstertitel |
| Subtitle | 20 / 25 px | 500 | normal | H3 Feature-Titel |
| Body L | 16 / 24 px | 400 | normal | Sektions-Intro-Texte |
| Body | 14 / 20 px | 400 / 500 | normal | Standard-UI, Navigation, Buttons |
| Small | 12 / 16 px | 400 / 500 | normal / +0.3 px | Labels, Meta, Eyebrows |
| Micro | 11 / 16.5 px | 400 / 500 | normal | Chart-Achsen, Zähler |

### Typo-Regeln

- **Headlines nie fett.** Maximal 500. Hierarchie entsteht über Größe, nicht Gewicht.
- **Negative Laufweite** nur ab 24 px (ca. −2.5 %).
- **Headlines bewusst umbrechen** – zweizeilig mit manuellem Umbruch („Let your experts / build the agents“).
- **Eyebrow über H2:** kleines graues Label + Pfeil („Build →“, „Controls →“) als Einstieg in eine Sektion.
- **Fließtext grau** (`body-muted`), nie reines Schwarz. Schwarz ist Headlines und Interaktion vorbehalten.
- **Kennzahlen dünn** (300) und groß – wirkt edel und ruhig.
- **Mono für Daten**: Datumsangaben in Versalien und Mono („OCT 6, 2026“).

---

## 4. Layout & Raster

- **Container:** 1440 px Viewport, **40 px seitlicher Rand**, Inhalt ca. 1360 px breit.
- **Raster:** 12 Spalten. Typische Aufteilungen:
  - Text links (4–5 Spalten) / Produkt-Screen rechts (7–8 Spalten)
  - Und umgekehrt – Sektionen wechseln die Seite für Rhythmus
  - 2er-, 3er- und 5er-Kachelraster für Features, Kennzahlen und Logos
- **Sektionsabstand:** 120–200 px vertikal. Lieber zu viel als zu wenig.
- **Kachel-Gaps:** 12–20 px.
- **Hero:** linksbündig, nicht zentriert. Headline + zwei Buttons, darunter eine breite Produkt-Bühne.
- **Abschluss-CTA:** einzige zentrierte Komposition der Seite.
- **Navigation:** 52 px hoch, sticky, weißer Hintergrund mit Haarlinie unten. Logo links, Links mittig, zwei Buttons rechts.

### Mobile

- 24 px Seitenrand.
- Buttons werden **volle Breite** und stapeln sich.
- Produkt-Screens werden skaliert, nicht umgebaut.
- Navigation kollabiert auf Burger-Icon.

---

## 5. Flächen, Rahmen, Schatten, Radien

### Ebenen-Logik

1. **Seite** – Weiß / `section-bg`
2. **Bühne** – `wash`-Fläche, Radius 10 px, 1-px-Haarlinie. Darin „schweben“ die Produkt-Fenster.
3. **Fenster / Karte** – Weiß, Haarlinie, ultraleichter Schatten, Radius 8–10 px
4. **Element in Karte** – `subtle`-Hintergrund für aktive Zustände, Radius 6 px

### Schatten

Ein einziger, geschichteter, kaum sichtbarer Schatten – kombiniert mit einer 1-px-Kontur:

```css
box-shadow:
  0 0 0 1px #E2E2E8,              /* Haarlinie als Kontur */
  0 1px 1px -0.5px rgb(0 0 0 / .016),
  0 3px 3px -1.5px rgb(0 0 0 / .016),
  0 6px 6px -3px rgb(0 0 0 / .01),
  0 12px 12px -6px rgb(0 0 0 / .01),
  0 24px 24px -12px rgb(0 0 0 / .01);
```

Für Hover eine stärkere Variante mit 2–5 % statt 1–1.6 % Deckkraft. **Nie harte oder farbige Schatten.**

### Radien

| Token | Wert | Verwendung |
|---|---|---|
| `radius-xs` | 2–4 px | Tags, Code-Chips, Balken in Charts |
| `radius-sm` | 6 px | Listeneinträge, kleine Inputs |
| `radius-md` | 8 px | **Buttons**, Inputs, kleine Karten (Standard) |
| `radius-lg` | 10 px | Karten, Bühnen, Fenster |
| `radius-full` | 9999 px | Avatare, Pills, Icon-Buttons, Statuspunkte |

Keine großen, weichen 24-px-Radien – die Formen bleiben präzise.

---

## 6. Komponenten

### Buttons

| Variante | Stil |
|---|---|
| **Primär** | Ink-Fläche `#18191B`, weißer Text, 14 px / 500, Radius 8 px, Höhe 36 px (Hero 40 px), Padding 14–18 px horizontal |
| **Sekundär** | Weiße Fläche, Ink-Text, 1-px-Haarlinie + ultraleichter Schatten, gleiche Maße |
| **Text-Link** | Grau, 12–14 px, mit Pfeil „→“ (z. B. „Read more →“) |
| **Pill / Chip** | Weiß, Haarlinie, Radius full, Icon + Label + optional „+“-Icon |

Immer **genau ein Primär-Button** pro Bereich, sekundär direkt daneben.

### Inputs

- Weiß oder `subtle`-Fläche, Haarlinie, Radius 8 px.
- Platzhalter in `neutral-muted`.
- Gruppierte Einstellungsfelder als graue Balken mit Label + Zähler + Chevron („Connectors 5 ▾“).

### Listen

- Zeilen ohne Trennlinien, 28–34 px hoch.
- Icon (16 px, farbig) + Label (14 px) + rechtsbündiger Wert (grau).
- Aktiver Eintrag: `subtle`-Hintergrund, Radius 6 px.
- Gruppenüberschriften klein und grau (12 px).

### Karten mit Feature

- Titel 20 px / 500, Beschreibung 14 px grau, darunter oder daneben ein Mini-UI-Ausschnitt.
- Karten in einem Raster teilen sich Haarlinien (wie eine Tabelle) statt einzelne Schatten zu haben.

### Akkordeon / Tabs als Liste

- Inaktiv: nur Icon + Titel in Grau, groß (18–20 px).
- Aktiv: `wash`-Fläche, Titel in Ink + einzeilige Beschreibung. Der Produkt-Screen links wechselt passend dazu.

### Kennzahlen

- Kleines graues Label oben, darunter große dünne Zahl (48–60 px, Gewicht 300).

### Timeline („Recently shipped“)

- Horizontale Haarlinie mit kleinen farbigen Formen als Knoten, darunter Titel, Text und Mono-Datum.

### Fenster-Chrome

- Produkt-Ausschnitte bekommen eine Kopfzeile mit drei Ampel-Punkten (rot/gelb/grün, 8 px).
- Fenster überlappen sich leicht – erzeugt Tiefe ohne Schatten.

---

## 7. Icons & Bildsprache

- **UI-Icons:** Outline, 1.5 px Strich, 16–20 px, in Ink oder Grau (Lucide-Stil).
- **Marken-Icons:** kleine, farbige, verspielte Formen (Geister-Maskottchen, Blobs, Rauten). Sie sind die einzige „Persönlichkeit“ der Marke und tauchen im Hero und im Abschluss-CTA auf.
- **Logos der Kunden:** in Grau auf `wash`-Kacheln (einfarbig), bei Testimonials in Originalfarbe.
- **Avatare:** rund, echte Fotos, klein (24–32 px).
- **Keine Stockfotos, keine Verläufe als Dekoration.** Einzige Ausnahme: sehr zarte, farbige Radial-Verläufe hinter Testimonial-Logos (kaum sichtbar).

---

## 8. Bewegung

- **Dezent und funktional:** kurze Fades und Slides beim Scrollen, Inhalte „bauen sich auf“ (z. B. Agenten-Schritte erscheinen nacheinander, Logzeilen blenden ein).
- **Lebendige Produkt-Demos:** Fortschrittskreise, Lade-Spinner, tippende Chats – das Produkt wirkt „in Betrieb“.
- **Hover:** leichte Farbänderung (Ink → Ink-Hover), stärkerer Schatten bei Karten. Keine Skalierungen oder Sprünge.
- Dauer ca. 150–250 ms, Ease-out. `prefers-reduced-motion` respektieren.

---

## 9. Übertragung auf den expose.ai-Wizard

| Gumloop-Muster | Anwendung bei expose.ai |
|---|---|
| Produkt-Bühne (`wash`-Fläche mit schwebenden Fenstern) | **Live-Vorschau-Bereich:** graue Bühne, darauf die A4-Seiten des Exposés als weiße „Blätter“ mit ultraleichtem Schatten |
| Sticky Navigation mit Haarlinie | **Wizard-Kopfzeile:** Schrittleiste (1–6) sticky oben, weiß, Haarlinie unten |
| Pills / Chips | **Schritt-Kreise:** aktiv = Ink-Fläche mit weißer Zahl; erledigt = Ink-Haken; offen = weiß mit Haarlinie; fehlende Pflichtangaben = kleiner Orange-Punkt |
| Einstellungs-Panel (Model, Connectors, Skills) | **Formular-Spalte:** gruppierte Felder mit grauen Gruppenköpfen und Zählern („Ausstattung 6 ▾“) |
| Listen mit farbigen Icons | **Lageanalyse:** Kategorie-Icon farbig + Name + Entfernung rechtsbündig grau („Bahnhof · 450 m“) |
| Akkordeon-Liste (Slack / Teams / Gmail) | **Design-Schritt:** Stilrichtungen (Minimalistisch, Elegant, Hochwertig …) als Liste; aktive Option zeigt Beschreibung, Vorschau wechselt live |
| Kennzahlen dünn & groß | **Konto-Dashboard:** Anzahl Exposés, verbleibende Bearbeitungen |
| Statuspunkte | **Exposé-Übersicht:** Entwurf (grau), Gekauft (grün), Bearbeitung übrig (Zahl) |
| Dunkle Sektion | **Landingpage:** eine dunkle Sektion für Preise / „Für Maklerbüros“ |
| Eyebrow + Pfeil | Landingpage-Sektionen („Lageanalyse →“, „Design →“) |

### Layout des Wizards (Desktop)

```
┌──────────────────────────────────────────────────────────────┐
│ Logo      ①Eckdaten ─ ②Lage ─ ③Bilder ─ ④Texte ─ ⑤Design ─ ⑥Prüfen   [Speichern] │  ← sticky, Haarlinie
├───────────────────────┬──────────────────────────────────────┤
│ Formular (≈ 40 %)     │ Live-Vorschau (≈ 60 %)               │
│ weiß, scrollt         │ wash-Bühne, A4-Seiten mit            │
│                       │ Wasserzeichen, sticky                │
│                       │                                      │
│ [Zurück]   [Weiter →] │            Seite 1 / 8   – 100 % +   │
└───────────────────────┴──────────────────────────────────────┘
```

Mobile: Formular im Vollbild, Vorschau als Umschalter („Vorschau ansehen“) unten fixiert.

---

## 10. Do & Don't

**Do**
- Schwarz-Weiß-Grau als Grundton, Farbe nur im Inhalt
- Haarlinien statt Schatten
- Große, leichte Headlines mit negativer Laufweite
- Viel Weißraum, linksbündige Kompositionen
- Echte Produkt-Ausschnitte statt Illustrationen
- Ein Primär-Button pro Bereich, immer schwarz

**Don't**
- Keine farbigen Buttons oder Flächen in der UI
- Keine Verläufe, Glas-Effekte oder Neon
- Keine fetten Headlines (> 500)
- Keine großen, weichen Radien (> 10 px bei Karten)
- Keine sichtbaren, dunklen Schatten
- Keine Stockfotos oder Emoji als Icons
