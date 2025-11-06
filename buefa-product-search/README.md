# 🔥 BÜFA Produkt-Datenbank

Eine moderne Webapplikation zur intelligenten Suche und Analyse von BÜFA Brandschutzprodukten für Schienenfahrzeuge.

## 📋 Funktionen

### 1. **Produktsuche**
- Schnellsuche nach Produkt-ID, Name oder Produktfamilie
- Echtzeit-Filterung der Ergebnisse
- Übersichtliche Darstellung mit allen wichtigen Eigenschaften
- Statistik-Dashboard mit Produktzahlen

### 2. **Erweiterte technische Filter**
- Filterung nach Harztyp (DCPD, OP, VE, rPET, IP)
- Filterung nach Produktfamilie
- Suche nach spezifischer Dichte (g/cm³)
- Suche nach Viskosität (mPas)
- Minimale Zugfestigkeit (MPa)
- Minimale Wärmeformbeständigkeit HDT (°C)

### 3. **Verarbeitungsverfahren-Filter**
- Hand Lay Up (HLU)
- Resin Transfer Molding (RTM)
- Vacuum Infusion (VI)
- Nachhaltige Produkte (rPET-basiert)

### 4. **Zertifizierungs-Filter**
- EN 45545 Hazard Levels (HL2, HL3)
- Requirement Sets (R1, R2, R3, R7, R17)
- Kombinierte Filterung möglich

### 5. **Kombinationen-Finder**
- Automatische Suche kompatibler Gelcoat-Harz-Kombinationen
- Bidirektionale Suche (Gelcoat → Harz oder Harz → Gelcoat)
- Anzeige von Zertifizierungen und Verarbeitungsparametern
- Validierte Systemkombinationen

### 6. **Produkt-Vergleich**
- Mehrere Produkte parallel vergleichen
- Übersichtliche Tabellen-Darstellung
- Alle technischen Eigenschaften im Überblick
- Export-Funktion für Vergleichsdaten

### 7. **Export-Funktionen**
- JSON-Export für maschinelle Weiterverarbeitung
- CSV-Export für Excel/Spreadsheet-Anwendungen
- Gefilterte oder vollständige Produktliste exportierbar

### 8. **Detailansicht**
- Ausführliche Modal-Ansicht für jedes Produkt
- Alle technischen Eigenschaften
- Verarbeitungsverfahren
- Zertifizierungen
- Besonderheiten und Empfehlungen

## 🚀 Installation & Start

### Voraussetzungen
- Moderner Webbrowser (Chrome, Firefox, Edge, Safari)
- Lokaler Webserver (oder einfach Dateien öffnen)

### Methode 1: Direkt im Browser öffnen
```bash
# Im Projektverzeichnis
cd buefa-product-search
# Öffne index.html in deinem Browser
open index.html  # macOS
start index.html # Windows
xdg-open index.html # Linux
```

### Methode 2: Mit Python HTTP Server
```bash
cd buefa-product-search
python -m http.server 8000
# Öffne im Browser: http://localhost:8000
```

### Methode 3: Mit Node.js HTTP Server
```bash
cd buefa-product-search
npx http-server -p 8000
# Öffne im Browser: http://localhost:8000
```

## 📁 Projektstruktur

```
buefa-product-search/
├── index.html          # Haupt-Webapplikation (HTML + CSS + JavaScript)
├── data/
│   └── products.json   # Produktdatenbank (19 Produkte)
└── README.md          # Diese Datei
```

## 💡 Verwendung

### Schnellsuche
1. Öffne die Webapplikation
2. Gib einen Suchbegriff ein (z.B. "8175", "FIRESTOP", "S425")
3. Drücke Enter oder klicke auf "Suchen"

### Technische Filter
1. Wechsle zum Tab "Erweiterte Filter"
2. Wähle gewünschte Filterkriterien aus
3. Klicke auf "Filter anwenden"

### Verarbeitungsverfahren finden
1. Wechsle zum Tab "Verarbeitung"
2. Wähle ein oder mehrere Verfahren aus (HLU, RTM, VI)
3. Klicke auf "Filter anwenden"

### Zertifizierungen prüfen
1. Wechsle zum Tab "Zertifizierung"
2. Wähle Hazard Level und/oder Requirement Set
3. Klicke auf "Filter anwenden"

### Kompatible Kombinationen finden
1. Wechsle zum Tab "Kombinationen"
2. Wähle entweder ein Gelcoat ODER ein Harz aus
3. Klicke auf "Kombinationen suchen"
4. Siehe alle kompatiblen Systeme mit Zertifizierungen

### Produkte vergleichen
1. Klicke auf einem beliebigen Tab auf "Zum Vergleich hinzufügen" bei gewünschten Produkten
2. Wechsle zum Tab "Vergleich"
3. Klicke auf "Vergleich anzeigen"
4. Siehe Produkte nebeneinander in Tabellenform

### Ergebnisse exportieren
1. Führe eine Suche oder Filterung durch
2. Klicke auf "JSON Export" oder "CSV Export"
3. Datei wird automatisch heruntergeladen

## 🎨 Features

### Modernes Design
- Responsive Layout (funktioniert auf Desktop, Tablet, Smartphone)
- Gradient-Farben mit professionellem Look
- Animierte Übergänge und Hover-Effekte
- Intuitive Bedienung

### Performance
- Schnelle Echtzeit-Suche
- Optimierte Filteralgorithmen
- Keine Abhängigkeiten von externen Bibliotheken
- Pure Vanilla JavaScript

### Benutzerfreundlichkeit
- Tab-basierte Navigation
- Modal-Dialoge für Detailansichten
- Klare visuelle Hierarchie
- Badges für schnelle Identifikation von Eigenschaften
- Statistik-Dashboard auf Startseite

## 📊 Datenbank-Struktur

Die JSON-Datenbank enthält 19 BÜFA Produkte mit folgenden Informationen:

- **Produkt-ID und Name**
- **Produktfamilie** (FIRESTOP, Sustainable, Gelcoat, etc.)
- **Technische Eigenschaften**
  - Harztyp, Dichte, Viskosität
  - Zugfestigkeit, HDT
  - Mechanische Eigenschaften
- **Verarbeitungsverfahren** (HLU, RTM, VI)
- **EN 45545 Zertifizierungen**
  - Hazard Levels (HL2, HL3)
  - Requirement Sets (R1-R17)
- **Kombinationen** (Gelcoat-Harz-Kompatibilität)
- **Besonderheiten und Empfehlungen**

## 🔧 Anpassung

### Eigene Daten hinzufügen
1. Öffne `data/products.json`
2. Füge neue Produkte nach dem gleichen Schema hinzu
3. Speichere die Datei
4. Lade die Webapplikation neu

### Design anpassen
Alle Styles sind in der `<style>`-Sektion in `index.html` definiert:
- Farben über CSS-Variablen (`:root`)
- Layout über CSS Grid und Flexbox
- Responsive Breakpoints bei 768px

## 🌐 Browser-Kompatibilität

✅ Chrome/Edge 90+
✅ Firefox 88+
✅ Safari 14+
✅ Opera 76+

## 📝 Lizenz

Dieses Projekt wurde für BÜFA Composite Systems erstellt.

## 🤝 Support

Bei Fragen oder Problemen:
1. Überprüfe die JSON-Datei auf Syntax-Fehler
2. Teste in verschiedenen Browsern
3. Öffne die Browser-Konsole (F12) für Fehlerme ldungen

## 🚀 Deployment

### Lokales Hosting
Einfach die Dateien auf einen Webserver kopieren und `index.html` aufrufen.

### GitHub Pages
```bash
# Repository initialisieren
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin <your-repo-url>
git push -u origin main

# In Repository Settings → Pages → Source: main branch
```

### Netlify / Vercel
Drag & Drop des `buefa-product-search` Ordners auf die jeweilige Plattform.

## ✨ Highlights

- 🎯 **Keine Installation nötig** - Läuft direkt im Browser
- ⚡ **Schnell & Performant** - Keine externen Dependencies
- 🎨 **Modern & Responsiv** - Funktioniert auf allen Geräten
- 🔍 **Intelligente Suche** - Mehrere Suchkriterien kombinierbar
- 📊 **Professionelle Darstellung** - Übersichtlich und strukturiert
- 💾 **Export-Funktionen** - JSON & CSV für weitere Verarbeitung
- 🔗 **Kombinationen-Finder** - Automatische System-Matching
- ⚖️ **Vergleichsfunktion** - Mehrere Produkte parallel vergleichen

## 🎉 Viel Erfolg!

Die BÜFA Produkt-Datenbank ist bereit für den Einsatz. Viel Spaß beim Suchen und Analysieren der Brandschutzprodukte!
