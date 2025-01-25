# Projekt IT-Sicherheit: Strukturanalyse / IT-Grundschutz-Modellierung / Risikoanalyse

### Im Repository enthaltene Dokumente

- **ISMS-Tool-Leer.ods**:  
  Enthält die Vorlagen für die Strukturanalyse, IT-Grundschutz-Modellierung und Risikoanalyse ohne Testdaten, um eigene Analysen durchführen zu können.

- **ISMS-Tool-TestDatei.ods**:  
  Eine Beispieldatei, die bereits mit Testdaten gefüllt ist, um die Funktionen und Abläufe des Projekts nachvollziehen und testen zu können.

- **XML_Kompendium_2023.xml**:  
  Dieses Dokument wird benötigt, um die Risikoanalysen automatisiert zu erstellen und relevante Risiken aus dem BSI-Grundschutz-Kompendium auszulesen.

- **README.md**:  
  Enthält eine Übersicht über das Repository sowie eine detaillierte Anleitung, wie mit dem LibreOffice-Dokument gearbeitet werden soll, einschließlich der einzelnen Schritte für Strukturanalyse, IT-Grundschutz-Modellierung und Risikoanalyse.

## Zusammenfassung
Dieses Projekt dient der Durchführung einer Strukturanalyse, der IT-Grundschutz-Modellierung und der Risikoanalyse
nach den Standards des BSI IT-Grundschutzes. Es umfasst die Erfassung, Zuordnung und Bewertung von Assets, die Zuordnung
relevanter Bausteine und Anforderungen aus dem BSI IT-Grundschutz, der Erstellung von Risikoanalysen für relevante Assets,
sowie die Erstellung von Berichten zur Dokumentation der Ergebnisse.

## Hinweis!
Die BASIC-Skripte, welche die Arbeitsschritte durch automatisierte Funktionen und Buttons in den Tabellenblättern unterstützen,
wurden zum großen Teil mithilfe von ChatGPT erarbeitet und anschließend an die spezifischen Anforderungen des Projekts angepasst.

# Anleitung zur Nutzung des Tools 

## Inhaltsverzeichnis
1. [Strukturanalyse]
2. [IT-Grundschutz-Modellierung]
3. [Risikoanalyse]

---

## 1. Strukturanalyse

### Ausführung
1. **Erfassung der Assets:**
   - Trage alle relevanten Assets in die Tabellenblätter **(Geschäftsprozesse, Applikationen, IT-Systeme, Räumlichkeiten, Kommunikationsverbindungen)** ein.
   - Ergänze bei den Geschäftsprozessen die Werte für die Grundwerte **Vertraulichkeit**, **Integrität** und **Verfügbarkeit**.

2. **Mapping der Assets:**
   - Fülle die Mapping-Tabellen mit einem Klick auf den Button **"Hole Assets"** oben links mit den Assets.
   - Führe das Mapping durch, indem du die entsprechenden Felder mit einem **"X"** markierst.

3. **Aktualisierung der Asset-Tabellen:**
   - Aktualisiere die Asset-Tabellenblätter mit einem Klick auf den Button **"Aktualisiere ..."** (oben neben der Tabellenüberschrift).
   - Die gemappten Assets werden in den Tabellen angezeigt, und die höchsten Werte der Grundwerte werden nach dem Maximalprinzip übernommen.

---

## 2. IT-Grundschutz-Modellierung

### Ausführung
1. **Vorbereitung:**
   - Lade alle Assets aus der Strukturanalyse mithilfe des Buttons **"Hole Assets"** in das Tabellenblatt **"Grundschutz-Bausteine Modellierung"**.

2. **Zuordnung von Bausteinen:**
   - Ordne den Assets in der Tabelle **"Grundschutz-Bausteine Modellierung"** die passenden Bausteine aus dem IT-Grundschutz über die Dropdown-Liste in den entsprechenden Zellen zu.

3. **Laden der Anforderungen:**
   - Übertrage die Assets und zugehörigen Bausteine mit dem Button **"Hole Assets, Bausteine und Anforderungen"** in die Tabelle **"Grundschutz-Realisierungsplan"**.
   - Die dazugehörigen Anforderungen der Bausteine werden automatisch hinzugefügt.

4. **Planung der Maßnahmen:**
   - Formuliere für jede Anforderung eine geeignete Maßnahme in der Spalte **"Maßnahmen"**.
   - Dokumentiere den Umsetzungsstatus der Maßnahmen in der Spalte **"Status"**.

5. **Erstellung des Reports zur Strukturanalyse und der IT-Grundschutz-Modellierung**
   - Erstelle den Report mithilfe eines Klick auf den Button **"Report zur Strukturanalyse und BSI IT-Grundschutz Modellierung erstellen"** auf dem Tabellenblatt **"Grundschutz-Realisierungsplanung"**

---

## 3. Risikoanalyse

### Ausführung
1. **Vorbereitung:**
   - Lade die Assets aus Teil 1 inklusive der Grundwerte mit dem Button **"Hole Assets"** in das Tabellenblatt **"Liste aller Assets"**.
   - Die Spalte **"Relevanz"** zeigt an, ob ein Asset für die **"Risikoanalyse"** relevant ist (mindestens ein Grundwert "Hoch" oder "Sehr hoch").

2. **Erstellung der Risikoanalysen:**
   - Verwende den Button **"Risikoanalyse erstellen (Auswahl des Kompendiums erforderlich)"**, um Risikoanalysen zu generieren.
   - Wähle die XML-Datei mit dem IT-Grundschutz-Kompendium, um die elementaren Risiken zu laden. (Im Repository hinterlegt)

3. **Durchführung der Risikoanalysen:**
   - Iteriere durch die elementaren Risiken und wähle aus, ob diese für die Grundwerte und das Asset relevant sind. Ergänze optional Kommentare.
   - Füge bei Bedarf zusätzliche Risiken mit dem Button **"Zusätzliches Risiko hinzufügen"** hinzu.

4. **Erstellung und Durchführung der Risikobehandlungen:**
   - Generiere Risikobehandlungen mit dem Button **"Risikobehandlungen erstellen"** für relevante Risiken.
   - Bewerte jedes Risiko anhand der **"BSI-Risikomatrix (200-3)"**:
     - Wähle Werte für "Häufigkeit" und "Auswirkung".
     - Das Risiko wird automatisch anhand der **"BSI-Risikomatrix (200-3)"** berechnet.
     - Ergänze Details zum Risiko im Feld **"Beschreibung"**.
   - Definiere Risikobehandlungsmaßnahmen und aktualisiere die Werte nach der Umsetzung.

5. **Erstellung des Risikoanalyse-Reports:**
   - Stelle sicher dass vor der Generierung des **"Report zur Risikoanalys"** kein solcher Report mehr im Libre Office Dokument vorhanden ist.
   - Generiere den Bericht mit dem Button **"Erstelle Report zur Risikoanalyse"** auf dem Tabellenblatt **"Liste aller Assets"**.
   - Es wird eine Übersicht als Tabellenblatt **"Report zur Risikoanalyse"** und eine PDF-Datei erstellt.


