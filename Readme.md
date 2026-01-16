# Sovol SV08 Toolchanger Umbau basierend auf Stealthchanger

Diese Anleitung beschreibt, wie du deinen **Sovol SV08 3D-Drucker** auf einen **Toolchanger** basierend auf dem **Stealthchanger** umbauen kannst. 


<img src="https://i.ibb.co/b5080Ymr/Sv08-Toolchanger.png" alt="Logo" width="300"/>






















## 📌 Wichtige Hinweise

1.Trenne den Drucker immer komplett vom Netzstrom, bevor du öffnest oder Komponenten absteckst.

2.Arbeite an einem geerdeten, stabilen Arbeitsplatz. Vermeide Kurzschlüsse.

3.Prüfe nach Umbau vor dem ersten Einschalten alle Verbindungen doppelt (Polung, Steckertypen, Schrauben). Ein Durchgangsprüfffunktion ist eigentlich in jedem Multi-Meter verbaut!

4.Firmware‑Flashen / Pin‑Mapping kann zum Fehlverhalten (z. B. Heizbett falsch angesteuert) führen — wenn du unsicher bist, nicht einschalten oder professionelle Hilfe holen.

5.Für Arbeiten am Netzteil / Austausch von Netzteil‑Kabeln: nur wenn du Erfahrung mit 230V/120V Elektrik hast

---

## 🛠️ Step 1: Vorbereitung des Sovol SV08 auf den Toolchanger

### 1.1 **Mainline Klipper installieren und eMMC auf 32GB erweitern**

<img src="https://upload.wikimedia.org/wikipedia/commons/d/d4/Klipper-logo_svg.svg" alt="Alt-Text" width="200"/>


- **Wichtig**: Wenn du den Toolhead komplett ändern möchtest, überspringe das Programmieren des Toolboards.
- Wenn du aber weiterdrucken möchtest, muss auch das Toolboaed geflasht werden.

**Video-Anleitung**:  
[Klipper Setup Guide](https://www.youtube.com/watch?v=1GHY9XKG7DQ)

**Materialien**:  
- [MKS eMMC 32GB Adapter](https://tinyurl.com/MKS-EMMC-32GB-Adapter)

  <img src="https://i.ibb.co/spjwT4yX/e-MMc-32-GB.png" alt="Logo" width="200"/>







- [ST-Link v2 Programmer](https://tinyurl.com/St-Link-v-2)
  
  <img src="https://i.ibb.co/BKSFJy47/ST-link-v2.png" alt="Logo" width="200"/>
  







---

## 🔧 Step 2: Der Toolchanger - Hardware und Software

### ⚙️ Hardware

#### 2.1 **Netzteil auf 350W erweitern**

- **Empfohlene Leistung**: Mindestens 350W Netzteil, um den Toolchanger und zusätzliche Komponenten zu versorgen.
- **Tipp**: Achte auf den Kabelquerschnitt (mindestens 12AWG oder 2,00mm²).

**Video-Anleitung**:  
[Netzteil Verkabelung](https://tinyurl.com/Netzteil-Verkabelung)

**Druckteile**:  
[Netzteil Befestigung](https://tinyurl.com/Netzteil-Befestigung)

<img src="https://i.ibb.co/FL7htvyj/Netzteil-350w.png" alt="Logo" width="200"/>










**Bild der Verkabelung**:  
[Verkabelung Bild](https://ibb.co/Y73YVfmb)

<img src="https://i.ibb.co/fYjH0sQr/Netzteil-Verkabelung.png" alt="Logo" width="200"/>







**Materialien**:  
- [Meanwell 350W Netzteil](https://tinyurl.com/Meanwell-350watt-Netzteil)
  
<img src="https://i.ibb.co/m5kB82qN/Meanwell-350watt-Netzteil.png" alt="Logo" width="200"/>







#### 2.2 **Rahmen für Toolhead Docks anfertigen**

- **Materialwahl**: Aluminiumprofile (2020) für den Dockrahmen.
- **Tipp**: Die Kapp- und Gehrungssäge sorgt für präzise Schnitte.
- **Druckmaterialien**: PETG ist okay, besser jedoch ABS/ASA, da es mehr Wärmebeständigkeit bietet.

**Detaillierte Anleitung und Materialliste**:  
[Toolhead Frame Guide](https://tinyurl.com/Toolhead-Frame-Bar)

**Für Voron-Bed Umrüstung**:  
[Voron Toolhead Frame](https://tinyurl.com/Toolhead-Frame-Bar-Voron)

#### 2.3 **Toolhead aussuchen und Docks einbauen**

- Der Toolhead muss zum Dockrahmen passen. Wähle ein passendes Dock für deinen Toolhead.
- Du kannst den **Anthead Toolhead** mit deinen gewünschten Extruder / Hotend verwenden.
- Alternativen Toolheads, die ebenfalls passen, sind z.B. **Voron Stealthburner** oder **Dragon Burner**. Diese erfordern jedoch eine Anpassung des Docks per CAD.

**Empfohlene Toolheads und Docks**:  
- [Anthead Toolhead und Dock](https://github.com/PrintersForAnts/AntHead)
- [Dragonburner](https://tinyurl.com/Dragon-Burner)
- [Voron Stealthburner](https://tinyurl.com/Voron-Stealtburner)

**Docks für Toolhead**:  
[Modular Dock Varianten](https://github.com/DraftShift/ModularDock)



#### 2.4 **Stealthchanger Shuttle/neue Riemen einbauen**

- **Materialwahl**: Fycets CNC Shuttle mit allen Kleinteilen und neue 2GT 6mm-Riemen 5meter reichen
- **Tipp**: Die Riemen müssen erneuert werden da man bei den Shuttle die Riemen einstülpen muss, wofür die original Riemen zu kurz sind. Außerdem empfehle ich im Anleitungsvideo die Riemenspannung per App mit Frequenz.
- **Video-Anleitung**: 
[Riemen erneuern](https://www.youtube.com/watch?v=7n_p33_o6dQ)

**Materialien**:   
- [Fycets CNC Shuttle Kit](https://tinyurl.com/fycets-cnc-shuttle-kit)
  
<img src="https://i.ibb.co/M5cHdtdx/CNC-Shuttle.png" alt="Logo" width="200"/>









<img src="https://i.ibb.co/SXx7JWqM/CNC-Shuttle-Fycets.png" alt="Logo" width="200"/>






- [Sovol Sv08 2GT 6mm Riemen](https://tinyurl.com/2GT-6mm-Riemen)
  
<img src="https://i.ibb.co/Tq0bN9nv/2-GT-6mm-Riemen.png" alt="Logo" width="200"/>





---

## 💻 Step 3: Software - Klipper und Toolchanger Integration

- **Klipper Setup**: Installiere Klipper auf deinem Drucker und konfiguriere es für den Toolchanger-Betrieb.
- Konfiguriere das **Toolboard** (z.B. **ebb36**) und stelle sicher, dass du die richtigen Pins und Toolhead-Parameter in der **printer.cfg** definierst.
- **Katapult**: Wenn du mehrere Toolheads verwenden möchtest, solltest du Katapult zur Verwaltung der Toolwechsel einrichten.

---

## 📝 Zusätzliche Tipps:

- **Kabelmanagement**: Verwende Kabelkanäle oder flexible Kabelbänder, um Kabel während des Drucks zu schützen.
- **Hitzeisolierung**: Stelle sicher, dass deine Toolheads gut isoliert sind, besonders bei den Hotends.
- **Materialwahl für Docks**: Docks und Toolheads sollten in **ABS oder ASA** gedruckt werden, um die hohe Temperaturbeständigkeit sicherzustellen.

---

## 📺 Nützliche Links:

- [YouTube Setup Video für Klipper](https://www.youtube.com/watch?v=1GHY9XKG7DQ)
- [MKS eMMC Adapter auf Amazon](https://tinyurl.com/MKS-EMMC-32GB-Adapter)
- [ST-Link v2 Programmer](https://tinyurl.com/St-Link-v-2)
- [Anthead Toolhead GitHub](https://github.com/PrintersForAnts/AntHead)

---

## 🚧 Noch nicht abgeschlossen?

Wenn du Fragen hast oder auf ein Problem stößt, öffne ein **Issue** oder schreib mir eine Nachricht! Viel Spaß beim Umbau und drucke auf!

