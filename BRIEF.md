# Brief: expose.ai – Exposé-Builder für Immobilienmakler

## 1. Produktidee

expose.ai ist eine Plattform, auf der Immobilienmakler in wenigen Minuten ein professionelles, gestaltetes Immobilien-Exposé als PDF (DIN A4) erstellen.

Der Makler lädt eine einfache PDF mit den Eckdaten des Objekts hoch. Das Tool liest die Daten aus, füllt ein Formular vor, analysiert die Lage anhand der Adresse, formuliert Objekt- und Lagebeschreibung und erzeugt daraus ein hochwertig gestaltetes Exposé. Der Makler sieht während des gesamten Prozesses eine Live-Vorschau und bezahlt erst, wenn er das fertige Exposé herunterladen möchte.

## 2. Zielgruppe

- Immobilienmakler (Einzelmakler und Maklerbüros)
- Markt: Deutschland, Sprache: Deutsch

## 3. Geschäftsmodell

- **Pay-per-Exposé:** 30 € pro Exposé. Bezahlt wird beim Download.
- **Abonnement:** für Vielnutzer geplant. Details (Umfang, Stufen, Preis) sind noch offen.
- **Bearbeitungen nach dem Kauf:** Ein gekauftes Exposé kann danach noch **3-mal bearbeitet** und jeweils erneut heruntergeladen werden.
- **Wasserzeichen:** Die Vorschau ist immer mit einem Wasserzeichen versehen. Erst nach der Bezahlung ist das PDF ohne Wasserzeichen verfügbar.

## 4. Konto

Ein Konto ist Pflicht, damit Makler zu ihren Exposés zurückkehren, sie bearbeiten und erneut herunterladen können.

Das Konto enthält:

- **Exposé-Übersicht:** alle Exposés mit Status (Entwurf / gekauft), verbleibenden Bearbeitungen und Download-Möglichkeit
- **Makler-Profil:** Logo, Brand Color, Kontaktdaten, Foto und Impressum. Diese Angaben werden in jedes neue Exposé automatisch übernommen.
- **Hausstil:** Der Makler kann sein gewähltes Design speichern (Layout-Stil, Farben, Schrift). Neue Exposés starten automatisch mit diesem Stil, damit alle Exposés eines Maklers einheitlich aussehen.
- **Rechnungen:** Übersicht und Download aller Rechnungen
- **Abo-Verwaltung:** sobald das Abo-Modell feststeht

## 5. Exposé-Wizard

Ein Exposé wird über einen Wizard in 6 Schritten erstellt.

### Navigation

- Oben befindet sich eine Schrittleiste mit nummerierten Kreisen (1–6), jeweils mit kurzer Beschriftung.
- Jeder Schritt kann direkt angetippt werden. Der Makler kann frei zwischen allen Schritten hin und her springen.
- Der aktuelle Schritt und abgeschlossene Schritte sind erkennbar. Schritte mit fehlenden Pflichtangaben werden markiert.
- Neben dem Wizard wird permanent eine **Live-Vorschau** des Exposés angezeigt, die sich bei jeder Eingabe aktualisiert.
- **Entwürfe werden automatisch gespeichert.** Der Makler kann jederzeit abbrechen und später weitermachen.

### Schritt 1 – Eckdaten

- Upload einer PDF mit den Eckdaten des Objekts
- Das Tool liest alle relevanten Eckdaten automatisch aus und füllt das Formular vor.
- Automatisch erkannte Felder sind als solche erkennbar, damit der Makler sie prüfen kann.
- Fehlende Pflichtfelder werden hervorgehoben und können manuell ergänzt werden.
- Alle Felder sind editierbar und können um weitere Angaben erweitert werden.
- Alternativ ist auch eine Eingabe ganz ohne PDF möglich.

**Pflichtfelder:**

- Titel des Exposés
- Objektart (z. B. Wohnung, Haus, Grundstück, Gewerbe)
- Vermarktungsart (Kauf / Miete)
- Preis (Kaufpreis bzw. Kaltmiete)
- Wohnfläche
- Anzahl Zimmer
- Baujahr
- Adresse
- Energieausweis: Art des Ausweises, Energiekennwert, wesentlicher Energieträger, Energieeffizienzklasse
- Provision / Käuferprovision

**Optionale Felder (Beispiele):** Grundstücksfläche, Etage, Anzahl Bad/Schlafzimmer, Zustand, Ausstattung (Balkon, Garten, Keller, Aufzug, Stellplatz …), Heizungsart, Nebenkosten, Hausgeld, Verfügbarkeit.

### Schritt 2 – Lage

- Die Adresse (aus Schritt 1) wird übernommen und kann angepasst werden.
- Das Tool analysiert das Umfeld des Objekts, zum Beispiel:
  - Einkaufen (Supermärkte, Drogerien)
  - Öffentlicher Verkehr (Bahnhöfe, Haltestellen)
  - Sport und Fitness (Fitnessstudios, Sportplätze, Schwimmbäder)
  - Bildung (Schulen, Kitas)
  - Gesundheit (Ärzte, Apotheken)
  - Gastronomie
  - Freizeit und Natur (Parks, Grünflächen)
- Ergebnisse werden mit Entfernung angezeigt (z. B. „Bahnhof – 450 m“).
- Eine **Karte mit Pins** zeigt das Objekt und die Einrichtungen im Umfeld. Die Karte erscheint auch im Exposé.
- **Adress-Datenschutz:** Der Makler kann wählen, dass die genaue Adresse im Exposé nicht angezeigt wird (z. B. nur Ort / Stadtteil). Die Adresse wird dann nur für die Analyse verwendet.

### Schritt 3 – Bilder

- Upload von Objektfotos
- Upload von Grundrissen (werden als Grundrisse gekennzeichnet)
- Reihenfolge der Bilder festlegen
- Titelbild auswählen
- Bilder wieder entfernen

### Schritt 4 – Texte

- Das Tool formuliert automatisch:
  - eine **Objektbeschreibung** auf Basis der Eckdaten
  - eine **Lagebeschreibung** auf Basis der Umfeldanalyse
- Beide Texte sind frei editierbar.
- Texte können neu generiert werden.

### Schritt 5 – Design

**Layout-Stil**

- Der Makler wählt zwischen mehreren Stilrichtungen, z. B. *minimalistisch*, *elegant*, *hochwertig/Luxus*, *modern*.
- Das Tool schlägt passend zum Objekt einen Stil vor (z. B. „hochwertig“ bei einem teuren Objekt). Der Makler kann den Vorschlag jederzeit ändern.
- Grundlage der Gestaltung ist eine große Sammlung professioneller Referenz-Exposés (ca. 100), die das Tool als Vorlage und Orientierung nutzt.

**Farben**

Drei Möglichkeiten:

1. Eine vorgefertigte Farbpalette auswählen
2. Eine **Brand Color** angeben. Daraus wird automatisch eine passende Palette erzeugt.
3. Alle 4–5 Farben der Palette einzeln festlegen

**Schrift**

- Auswahl aus einer kuratierten Liste hochwertiger Schriftkombinationen (Überschrift + Fließtext)
- Nur seriöse, professionelle Schriften, keine verspielten oder geschwungenen Schriften

**Branding**

- Logo des Maklers (aus dem Profil, hier änderbar)
- Kontaktblock des Maklers im Exposé

**Hausstil speichern**

- Der Makler kann die aktuelle Auswahl als seinen Hausstil speichern, damit alle künftigen Exposés gleich aussehen.

### Schritt 6 – Prüfen & Kaufen

- Gesamtvorschau des Exposés (mit Wasserzeichen), Seite für Seite durchblätterbar
- Prüfung auf Vollständigkeit: Fehlende Pflichtangaben werden aufgelistet und verlinken auf den passenden Schritt.
- Bezahlung (30 €) bzw. Nutzung des Abos
- Nach erfolgreicher Bezahlung: Download des Exposés als PDF (DIN A4) ohne Wasserzeichen
- Rechnung wird automatisch erstellt und im Konto abgelegt.

## 6. Nach dem Kauf

- Das gekaufte Exposé bleibt im Konto gespeichert.
- Es kann **3-mal** bearbeitet und anschließend jeweils neu heruntergeladen werden.
- Die Anzahl der verbleibenden Bearbeitungen ist jederzeit sichtbar.
- Ist das Kontingent aufgebraucht, ist das Exposé nur noch herunterladbar, nicht mehr bearbeitbar.

## 7. Das fertige Exposé

- Format: PDF, DIN A4
- Inhalte (je nach Angaben):
  - Titelseite mit Titelbild, Titel, Eckdaten und Preis
  - Übersicht der Eckdaten
  - Objektbeschreibung
  - Ausstattung
  - Bildergalerie
  - Grundrisse
  - Lagebeschreibung mit Karte und Umfeldanalyse
  - Energieausweis-Angaben
  - Provision und rechtliche Hinweise
  - Kontaktseite des Maklers mit Logo und Kontaktdaten
- Das Design folgt dem gewählten Stil, den Farben und den Schriften.
- Die Vorschau entspricht exakt dem späteren PDF (bis auf das Wasserzeichen).

## 8. Offene Punkte

- Ausgestaltung des Abo-Modells (Umfang, Stufen, Preise, Bearbeitungsregeln im Abo)
- Was gilt nach Ablauf der 3 Bearbeitungen (z. B. erneuter Kauf)?
- Aufbewahrungsdauer von hochgeladenen PDFs und Bildern
- Ob ein Konto mehrere Nutzer haben kann (Maklerbüro mit Team)
