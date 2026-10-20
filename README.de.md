[ 🌐 عربي ](README.ar.md) | [ 🇩🇪 Deutsch ](README.de.md) | [ 🇫🇷 Français ](README.fr.md) | [ 🇳🇱 Nederlands ](README.nl.md) | [ 🇪🇸 Español ](README.sp.md) | [ 🇬🇧 English ](README.md)

# Multi-Node-Bestandsabstimmung & Schwundanalyse | Shopify- & 3PL-Excel-Vorlage
<img width="1920" height="790" alt="image" src="https://github.com/user-attachments/assets/6689bffe-1aac-43d7-9f63-6e85a14470f0" />


[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](#license)
[![Platform: Browser + Excel](https://img.shields.io/badge/Platform-Browser%20%2B%20Excel-217346.svg)](#quick-start-tutorial-how-to-automate-your-inventory-reconciliation)
[![Tool Type: Decision Support](https://img.shields.io/badge/Tool%20Type-Decision%20Support-2251FF.svg)](#what-it-helps-you-track-inventory-pain-points-vs-solutions)

**Eine automatisierte Bestandsabstimmungs-Tabelle und Schwundanalyse-Vorlage für Multichannel-E-Commerce-Marken. Vergleichen Sie sofort Shopify-Bestandsmengen, interne Lagerverwaltungssystem-Datensätze (WMS) und physische Zählungen Drittanbieter-Logistikpartner (3PL), um Abweichungen zu lokalisieren und Stückverluste in direkte finanzielle Auswirkungen umzurechnen — ohne VLOOKUP-Formeln zu schreiben oder Berichte jeden Monat neu aufzubauen.**

**Keine Registrierung. Keine Installation. Kostenlos in Ihrem Browser.**

Testen Sie Ihre Betriebsdaten sofort in der kostenlosen Browserversion. Für laufende monatliche Monatsabschlüsse und Offline-Datensicherheit wechseln Sie zur vollständig freigeschalteten Excel-Vorlage mit 30-tägiger Geld-zurück-Garantie ohne Fragen.

> 🌐 **Interaktives Dashboard öffnen**  
> [Testen Sie den kostenlosen browserbasierten 3PL-Bestandsabstimmungs-Simulator](https://hyvoid.github.io/MULTI-NODE-INVENTORY-RECONCILIATION/)
> 
> 📥 **Wiederverwendbare Tabelle holen**  
> [Laden Sie die Vorlage für Bestandsschwund & Prüfung in Excel herunter](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)

---

## Was es nachverfolgt: Bestandsprobleme im E-Commerce vs. Lösungen

Anstatt lediglich festzustellen, dass „Zahlen nicht übereinstimmen", übersetzt dieses Toolkit rohe Bestandsdifferenzen in einen finanziellen Aktionsplan.

| Bestandsproblem im E-Commerce (das „Warum") | Abstimmungslösung (das „Wie") |
| :--- | :--- |
| **Systemübergreifende blinde Flecken:** Unsicherheit, welches System (Shopify vs. 3PL vs. WMS) die Wahrheit über den verfügbaren Bestand kennt. | **Multi-Node-Triangulation:** Gleicht systemgemeldete Mengen Seite an Seite ab, um genau zu lokalisieren, wo die Datensynchronisierung scheitert. |
| **Nicht quantifizierter finanzieller Schwund:** Eine Abweichung von 20 Stück bei einem 5-€-Artikel genauso behandeln wie bei einem 50-€-Artikel. | **COGS-gewichtete Varianzanalyse:** Multipliziert Stückabweichungen mit den SKU-Kosten, um die tatsächliche finanzielle Abschreibungsgefahr aufzudecken. |
| **Leckage bei Drittanbieter-Logistik (3PL):** Verdacht, dass Fulfillment-Partner Bestände verlieren, aber ohne harte Beweise für SLA-Ansprüche. | **Abweichungsquoten-Verfolgung:** Isoliert 3PL- gegenüber internen Lagervarianzquoten, um eine faktische Grundlage für vertragliche Schadensersatzansprüche zu schaffen. |
| **Analyseparalyse durch Rohdaten:** Tausende Zeilen von Zählungs-Tabellen durchscrollen, um Fehler zu finden. | **Ausnahmebasiertes Dashboard:** Reiht automatisch die „Top 10 der verlustwertstärksten SKUs", um Managementuntersuchungen zu priorisieren. |

---

## Schnellstart-Anleitung: So automatisieren Sie Ihre Bestandsabstimmung

Verwandeln Sie unstrukturierte Exporte aus mehreren Quellen in vier strukturierten Schritten in ein Prüfaudit auf Führungsebene.

### Schritt 1: Konfigurieren Sie Ihre SKU-Stammdaten (einmalige Einrichtung)
Navigieren Sie zum Blatt `Config_Master`. Definieren Sie Ihre Standard-SKU-Nomenklatur, die Stückkosten (COGS) und unternehmensspezifische Warnschwellen (z. B. jede Abweichung > 5 Stück oder > 100 € Wert markieren). Diese Basis stellt sicher, dass alle eingehenden Daten an einer einzigen Quelle der Wahrheit gemessen werden.

### Schritt 2: WMS-, 3PL- und Shopify-Exporte importieren
Umgehen Sie die manuelle Datennormalisierung. Fügen Sie Ihre rohen CSV-Exporte direkt in die dafür vorgesehenen Registerkarten ein:
*   `Import_Shopify` (Ihre Storefront-Verfügbarkeit)
*   `Import_WMS` (Ihre internen Lagerdatensätze)
*   `Import_3PL` (Ihre externen physischen Zählungen des Fulfillment-Partners)
*Hinweis: Das System ist darauf ausgelegt, rohe Exporte direkt zu verarbeiten — kein manuelles Löschen von Spalten oder Neuerstellen erforderlich.*

### Schritt 3: Das Schwund-Dashboard erstellen & Ausnahmen prüfen
Navigieren Sie zur Ausgabe `Dashboard`. Die automatisierte Abstimmungs-Engine bereinigt sofort Formatierungen, gleicht SKUs ab und berechnet Abweichungen. Prüfen Sie Ihre wertstärksten Bestandsvarianzen, den gesamten Schwundwert und die Knoten-zu-Knoten-Genauigkeitsquoten, ohne eine einzige Zelle manuell zu berechnen.

### Schritt 4: Eine Routine etablieren & für wiederholte Nutzung herunterladen
Verwenden Sie für Ihre erste Prüfung die Browserversion, um unmittelbare Bestandsprobleme zu identifizieren. Um einen robusten monatlichen Bestandskontroll-Rhythmus zu etablieren, exportieren Sie das System für die langfristige Nutzung.

👉 **Handlung erforderlich:** Sobald Sie Ihren Arbeitsablauf validiert haben, **[laden Sie die wiederverwendbare Excel-Vorlage für die Bestandsabstimmung hier herunter](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)**. Nächsten Monat fügen Sie einfach den neuen Bestandsschnappschuss über die alten Daten ein — die gesamte Varianzanalyse aktualisiert sich automatisch.

---

## Die Betriebslogik & Methodik

Dieses Toolkit ist um professionelle Prüfungsprinzipien herum konstruiert und verlagert den Fokus von der Datenaggregation zum proaktiven Vermögensschutz. Hier ist die Betriebsmethodik, die die Arbeitsmappe antreibt:

### 1. Methodik: 3-Wege-Bestandsabgleich
*   **Die Methode:** Ähnlich wie bei Finanzprüfungen von Kreditorenbuchhaltung verwendet dieses Framework ein **3-Wege-Abgleichsprinzip** über digitalen Vertrieb (Shopify), interne Nachverfolgung (WMS) und physische Lagerung (3PL). 
*   **Die betriebliche Auswirkung:** Es beendet das „Schuldzuweisungsspiel". Durch Triangulation der Daten können Betriebsleiter erkennen, ob ein Problem ein Storefront-Synchronisierungsfehler (API-Verzögerung) oder ein physischer Fulfillment-Verlust (Schwund) ist, was die Lösungszeit drastisch verkürzt.

### 2. Methodik: Priorisierung nach finanziellem Verlustrisiko (VaR)
*   **Die Methode:** Abweichungen werden inhärent nach Wareneinsatzkosten (COGS) gewichtet. Die Berechnungsschicht transformiert `Stückvarianz` in `finanzielle Abschreibungsgefahr`.
*   **Die betriebliche Auswirkung:** Es optimiert die Arbeitskraftzuteilung. Anstatt dass Lagerpersonal 4 Stunden mit der Untersuchung einer 50-Stück-Abweichung bei Poly-Mailern verbringt, wird es vom Dashboard umgeleitet, eine 3-Stück-Abweichung bei hochmargiger Elektronik zu untersuchen.

### 3. Methodik: Ausnahmebasiertes Berichtswesen
*   **Die Methode:** Das Toolkit filtert Tausende übereinstimmende SKUs in eine kondensierte Liste betrieblicher Ausnahmen auf Basis benutzerdefinierter Toleranzschwellen (z. B. akzeptabler Schwund < 0,5 %).
*   **Die betriebliche Auswirkung:** Es schafft **produktisiertes Denken**. Der Lieferkettendirektor sieht keinen Datenauszug; er sieht eine umsetzbare Aufgabenliste für interne Prozesskorrekturen oder die Einreichung von 3PL-Ansprüchen.

---

## Praxisnahe Szenarien: Wann Sie diese Bestandsprüfungs-Vorlage verwenden

Dieses System ist für kritische Wendepunkte in der Lieferkette konzipiert, bei denen die physische Bestandsgenauigkeit die finanzielle Gesundheit bestimmt.

*   **Szenario A: Monatlicher Finanzabschluss.** Finanzteams benötigen eine exakte COGS-Abschreibungszahl für die Buchhaltung. Verwenden Sie diese Vorlage, um den exakten Dollarwert des verlorenen Bestands über alle Lager am letzten Tag des Monats zu berechnen.
*   **Szenario B: 3PL-SLA-Vertragsstreitigkeiten.** Sie vermuten, dass Ihr Fulfillment-Partner Waren über die 1,5-%-Schwundgrenze hinaus verliert. Verwenden Sie den Multi-Node-Vergleich, um einen dokumentierten Anspruchsbericht für fehlende hochwertige SKUs zu erstellen.
*   **Szenario C: Vorbeugung gegen Lagerfehlbestände in der Hochsaison (Q4/Black Friday).** Shopify zeigt 100 Stück, aber der 3PL hat nur 20. Führen Sie diese Abstimmung während Q4 wöchentlich durch, um „Geisterbestand" zu erkennen, bevor Kunden Bestand kaufen, den Sie physisch nicht besitzen, und verhindern Sie massive Rückerstattungsquoten und Kundendiensttickets.

---

## Häufige Betriebsprobleme im Bestandsmanagement, die dies löst

| Betriebsproblem im Bestandsmanagement | Manueller Tabellenkalkulationsprozess | Automatisierte Vorlagenlösung |
| :--- | :--- | :--- |
| **Drei uneinheitliche Systeme widersprechen sich** | Operatoren führen manuell `INDEX/MATCH` über Shopify-, WMS- und 3PL-Dateien aus, was das Risiko defekter Verweise erhöht. | Eine standardisierte Abstimmungsschicht gleicht alle Lagerhaltungseinheiten (SKUs) automatisch ab. |
| **Unstrukturierte Formatierung exportierter Daten** | Leerzeilen, nachgestellte Leerzeichen und groß-/kleinschreibungssensitive SKUs erzeugen Fehlabweichungsfehler. | Die Berechnungsschicht normalisiert Zeichenfolgen und Datentypen vor der Varianzprüfung. |
| **Schwund wird nur in Stück gemessen** | Das Management sieht ein Stückdefizit, kann aber die COGS-Auswirkung nicht genau schätzen. | Die eingebettete SKU-Kostenmatrix rechnet Mengendefizite in geschätzte finanzielle Abschreibungen um. |
| **Große Ausnahmen gehen im Detail unter** | Controller scannen Tausende Zeilen und übersehen geschäftlich fatale Bestandsabweichungen. | Das Führungs-Dashboard hebt 3PL-Fehlerquoten, toten Bestand und die Top 10 der verlustwertstärksten Artikel hervor. |
| **3PL-Verluste sind schwer zu belegen** | Fehlender Bestand bleibt eine informelle Lagerbeschwerde ohne Dokumentation. | Erzeugt ein faktisches Varianz-Hauptbuch zur Unterstützung formeller 3PL-SLA-Ansprüche und Rückerstattungen. |

---

## Für wen sich dieses eignet: Rollen & Anwendungsfälle

Dieses Werkzeug schlägt die Brücke zwischen physischer Lagerung und Finanzberichterstattung. Es ist absichtsvoll konzipiert für:

*   **E-Commerce-Betriebsleiter**, die eine *Shopify-Bestandsabstimmungs-Vorlage* benötigen, um digitale Storefronts mit physischen Fulfillment-Zentren zu synchronisieren.
*   **Lieferkettendirektoren**, die eine *Alternative zu 3PL-Prüfungssoftware* suchen, um externe Partner für vertragliche Schwundquoten zur Verantwortung zu ziehen.
*   **Bestandscontroller & Lagerleiter**, die monatliche *Zykluszählungs-Abstimmungen* über mehrere interne Knoten durchführen.
*   **Teilzeit-CFOs & Finanzleiter**, die eine genaue Methode zur Berechnung von *Bestandsschwund und COGS-Auswirkung* für monatliche Buchhaltungsabschlüsse benötigen.
*   **DTC-Gründer**, die einen Überblick auf Führungsebene über die Bestandsgesundheit benötigen, ohne in komplexe, sechsstellige ERP-Integrationen zu investieren.

*Hinweis: Dieses Toolkit ist **nicht** dazu bestimmt, Echtzeit-APIs, ERP-Systeme oder Live-WMS-Barcodescannen zu ersetzen. Es ist ein periodisches Entscheidungsunterstützungs-Framework zur Prüfung dieser Systeme.*

---

## Über den Entwickler

Ich entwickle leichtgewichtige Betriebs-Tracker und Entscheidungsunterstützungs-Werkzeuge für Situationen, in denen zu viele bewegliche Teile im Spiel sind, um sie im Kopf zu behalten, aber nicht genug Komplexität, um ein weiteres Unternehmenssystem zu rechtfertigen.

Die zentrale Frage ist einfach: **Welche Informationen müssen an einem zentralen Ort versammelt sein, bevor die nächste strategische Lieferkettenentscheidung sicher getroffen werden kann?**

Diese Multi-Node-Bestandsabstimmungs-Arbeitsmappe ist ein Beispiel für diesen Ansatz: wiederkehrende systemübergreifende Bestandsvergleiche in einen standardisierten analytischen Arbeitsablauf zu verwandeln, der betriebliche Abweichungen mit finanziellen Konsequenzen verknüpft.


## Technische Details

<details>
<summary>Für technische Prüfer, Excel-Praktiker und Mitarbeiter</summary>

### Arbeitsmappen-Architektur

Die Arbeitsmappe ist absichtlich als **Datenbereinigungs- und Abstimmungs-Engine + Entscheidungs-Dashboard für Finanzverluste** strukturiert und nicht als permanente Bestandsdatenbank. Jeder Abstimmungszyklus kann den vorherigen Importsatz überschreiben oder als separate Arbeitsmappe gespeichert werden, wodurch die Datei leichtgewichtig bleibt und unnötige Datenbank- oder Makroabhängigkeiten vermieden werden.

Die Architektur folgt einem einfachen:

**Eingabe → Normalisieren → Abstimmen → Quantifizieren → Markieren → Darstellen**

```text
                    ┌──────────────────────┐
                    │    Config_Master      │
                    │ SKU / Cost / Rules    │
                    └──────────┬───────────┘
                               │
             ┌─────────────────┼─────────────────┐
             │                 │                 │
             ▼                 ▼                 ▼
     Import_Shopify       Import_WMS       Import_3PL
     System snapshot      WMS snapshot     Physical stock
             │                 │                 │
             └─────────────────┼─────────────────┘
                               ▼
                    ┌──────────────────────┐
                    │     Calc_Engine      │
                    │ Normalize + Match    │
                    │ Variance Calculation  │
                    │ Loss Valuation        │
                    │ Exception Flagging    │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │      Dashboard       │
                    │ KPI + Loss Analysis  │
                    │ Risk Ranking         │
                    └──────────────────────┘
```

Die Arbeitsmappe ist in sechs funktionale Blätter unterteilt:

| Blatt            | Ebene         | Verantwortlichkeit                                                            | Primärer Nutzer           |
| ---------------- | ------------- | ------------------------------------------------------------------------- | ---------------------- |
| `Dashboard`      | Entscheidung | KPI-Zusammenfassung, Verlustgefahr, Knotenvergleich, Top-10-Ausnahmen            | CEO / Management       |
| `Config_Master`  | Konfiguration | Standard-SKU-Liste, Produktinformationen, Stückkosten, Abweichungsschwellen | Betrieb / Finanzen   |
| `Import_Shopify` | Eingabe         | Roher Shopify-Bestandsexport                                              | Betrieb             |
| `Import_WMS`     | Eingabe         | Roher interner WMS-Bestandsexport                                         | Lager / Betrieb |
| `Import_3PL`     | Eingabe         | Roher physischer 3PL-Bestandsexport                                         | 3PL / Betrieb       |
| `Calc_Engine`    | Berechnung   | Datennormalisierung, SKU-Abgleich, Varianzberechnungen, finanzielle Auswirkung | Verborgene technische Ebene |

Die drei Importblätter sind absichtlich als **Einfügezonen** gehalten. Die Quellspezifikation erlaubt es Benutzern, die Originalexporte direkt einzufügen, einschließlich Kompatibilität mit führenden Leerzeilen, anstatt sie zu zwingen, die Dateien vor der Abstimmung manuell umzugestalten.

### Datenfluss und Abstimmungslogik

Die Kernberechnungsschicht verwendet `Config_Master` als Referenzpunkt für standardisierte SKUs.

```text
Raw Export
   ↓
Trim / Normalize
   ↓
Standard SKU Key
   ↓
Cross-System Lookup
   ↓
Shopify Quantity
WMS Quantity
3PL Quantity
   ↓
Absolute Variance
   ↓
Relative Variance
   ↓
Unit Cost
   ↓
Estimated Financial Loss
   ↓
Warning / Exception Status
   ↓
Dashboard
```

Das Design adressiert spezifisch das Problem **unstrukturierter Daten**. Die Quellarchitektur sieht `TRIM()` zum Entfernen versteckter oder versehentlicher Leerzeichen und `UPPER()` zur Normalisierung der Groß-/Kleinschreibung vor, gefolgt von `XLOOKUP` oder `INDEX + MATCH` für nicht-invasives tabellenübergreifendes Abrufen.

Dies ist wichtig, weil eine SKU wie:

```text
ABC-001
```

nicht zu einer Fehlausnahme werden sollte, nur weil ein anderer Export enthält:

```text
 abc-001
```

Die Abstimmungs-Engine behandelt Normalisierung daher als Voraussetzung für den Vergleich, anstatt zu versuchen, Datenqualitätsprobleme zu lösen, nachdem der Varianzbericht bereits erstellt wurde.

### Abstimmungs-Stichtag-Prinzip

Bestandsschnappschüsse müssen denselben **betrieblichen Stichtag** darstellen.

Beispielsweise:

```text
Shopify Snapshot     → Sunday 23:59:59
WMS Snapshot         → Sunday 23:59:59
3PL Physical Count   → Sunday 23:59:59
```

Wenn die Schnappschüsse zu wesentlich unterschiedlichen Zeiten erstellt werden, können Bestandsbewegungen, Rückgaben oder in Trans befindliche Aufträge scheinbare Differenzen erzeugen, die kein tatsächlicher Schwund sind.

Die Quellarchitektur identifiziert konsistente Stichtagzeiten ausdrücklich als zentrale Betriebseinschränkung und warnt, dass nicht übereinstimmende Schnappschüsse „falsche Differenzen" erzeugen können.

Dies ist daher eine **Anforderung der Betriebskontrolle**, nicht bloß eine Anforderung an eine Tabellenkalkulationsformel.

### SKU als einziger Abstimmungsschlüssel

Die SKU wird als Standardidentität behandelt, die die drei Quellsysteme verbindet.

Die Konfigurationsschicht pflegt:

* Standard-SKU
* Produktname
* Stückkosten
* Abweichungsschwelle
* Warnschwelle

Die Berechnungs-Engine verwendet dann diesen Standardschlüssel, um Mengen aus jeder Quelle abzurufen.

Dies verhindert, dass die Abstimmung von der Zeilenreihenfolge der importierten Dateien abhängt. Shopify kann SKUs in einer Reihenfolge auflisten, WMS in einer anderen und 3PL in einer dritten; die Berechnungs-Engine vergleicht dennoch dasselbe Produkt mit demselben Produkt.

Die Quellspezifikation betont SKU-Eindeutigkeit und -Konsistenz als grundlegende Einschränkung: ein physisches Produkt sollte nicht durch mehrere inkonsistente Kennungen dargestellt werden.

### Dashboard-Architektur

Das Dashboard ist absichtlich für **ausnahmefirst-Management** konzipiert, nicht zur Reproduktion der rohen Quelltabellen.

Die primäre KPI-Ebene enthält:

* Gesamtmengenvarianz
* Geschätzter gesamter Finanzverlust
* 3PL-Abweichungsquote
* Interne Lagerabweichungsquote

Die visuelle Ebene stellt dann bereit:

* Verlustwertverteilung zwischen 3PL und internem Lager
* Top 10 der SKUs nach Verlustwert
* Identifikation von Ausnahmen mit hohem Risiko

Diese Ausgaben sind in der Quellarchitektur direkt spezifiziert.

Die beabsichtigte Managementsequenz ist:

```text
Wie viel unterscheidet sich?
        ↓
Wie viel Geld ist gefährdet?
        ↓
Wo konzentriert sich die Gefährdung?
        ↓
Welche SKUs sind am wichtigsten?
        ↓
Welche Ausnahmen sollten untersucht werden?
        ↓
Ist eine Prozesskorrektur oder ein 3PL-Anspruch erforderlich?
```

Deshalb wird die Arbeitsmappe besser als **Entscheidungsunterstützungsschicht** verstanden denn als einfache Bestandsvergleichs-Tabelle.

### Drei Fallen, die selbst erfahrene Bestandsoperatoren zur Strecke bringen

#### Falle 1 — Jede Mengendifferenz als Schwund behandeln

**Entscheidung:**
Ein Operator sieht, dass Shopify 1.000 Stück meldet, während der 3PL 970 meldet, und zeichnet sofort 30 Stück als verloren.

**Fehlerhafte Zahl:**
Der Vergleich verwendet Schnappschüsse, die zu unterschiedlichen Zeiten erstellt wurden.

**Warum sich die Empfehlung ändert:**
Die 30-Stück-Differenz kann Lieferungen, Rückgaben, Anpassungen oder andere Bewegungen darstellen, die zwischen den beiden Schnappschüssen stattfanden.

**Korrekter Ansatz:**
Zuerst eine gemeinsame Stichtagzeit festlegen und gleichartige Bestandsschnappschüsse vergleichen.

| Ansatz                 | Ergebnis                                             |
| ------------------------ | -------------------------------------------------- |
| Unterschiedliche Schnappschusszeiten | 30-Stück-Differenz als Verlust behandelt                 |
| Gemeinsamer Stichtag           | Nur verbleibende unerklärte Varianz wird untersucht |

Die Quelle identifiziert Stichtag-Inkonsistenz spezifisch als Ursache falscher Abweichungen.

Die korrigierte Entscheidung ist daher **„die verbleibende Varianz untersuchen"**, nicht **„die gesamte Varianz als Schwund beanspruchen."**

<details>
<summary>Berechnungslogik</summary>

```text
Comparable Variance
= Quantity at Node A
- Quantity at Node B

Only when:
Snapshot_A_Time = Snapshot_B_Time
```

Eine Abweichung sollte nicht als finanzieller Verlust interpretiert werden, bevor die Vergleichsbasis selbst gültig ist.

</details>

#### Falle 2 — Probleme nach Stück statt nach Geld reihen

**Entscheidung:**
Der Operator sortiert den Abstimmungsbericht nach der größten Mengenabweichung.

**Fehlerhafte Metrik:**
Eine 50-Stück-Abweichung wird über einer 10-Stück-Abweichung gereiht, einfach weil `50 > 10`.

**Warum die Empfehlung unvollständig ist:**
Menge stellt keine wirtschaftliche Bedeutung dar.

Angenommen:

| SKU   | Variance | Unit Cost | Estimated Exposure |
| ----- | -------: | --------: | -----------------: |
| SKU-A |       50 |        $2 |               $100 |
| SKU-B |       10 |       $40 |               $400 |

Eine reine Mengenreihung würde SKU-A zuerst untersuchen. Eine Finanzverlust-Reihung würde SKU-B zuerst untersuchen.

Die Quellarchitektur verlangt ausdrücklich die Einführung einer SKU-Kostenmatrix, damit Mengendifferenzen in finanziellen Verlust übersetzt werden können.

**Korrekte Entscheidung:** Ausnahmen sowohl nach **Mengenvarianz als auch finanzieller Gefährdung** priorisieren, nicht nach Menge allein.

<details>
<summary>Berechnungslogik</summary>

```text
Estimated Loss Value
= Variance Quantity × Unit Cost
```

Für das Beispiel:

```text
SKU-A = 50 × $2  = $100
SKU-B = 10 × $40 = $400
```

Die zweite Ausnahme hat die kleinere Menge, aber die größere finanzielle Konsequenz.

</details>

#### Falle 3 — Annehmen, dass ein sauberer SKU-Abgleich saubere Daten bedeutet

**Entscheidung:**
Der Operator verwendet einen direkten Abgleich zwischen den drei Exporten und nimmt an, dass nicht zugeordnete Datensätze fehlenden Bestand darstellen.

**Fehlerhafte Annahme:**
Es wird vermutet, dass die SKU-Zeichenfolgen über alle Systeme hinweg identisch sind.

**Warum sich die Empfehlung ändert:**
Exportierte Daten können führende/nachgestellte Leerzeichen, inkonsistente Groß-/Kleinschreibung, Sonderzeichen, Leerzeilen oder historische SKU-Benennungskonventionen enthalten. Die Quelle identifiziert diese spezifisch als praktische Datenqualitätsprobleme.

Beispielsweise:

```text
Shopify → "sku-001"
WMS     → "SKU-001"
3PL     → " SKU-001 "
```

Ein naiver exakter Abgleich kann diese als unterschiedliche Produkte interpretieren.

**Korrekter Ansatz:** die Kennung vor dem systemübergreifenden Abruf normalisieren.

<details>
<summary>Normalisierungslogik</summary>

```excel
=UPPER(TRIM([@SKU]))
```

Dann den normalisierten Schlüssel für tabellenübergreifendes Abrufen verwenden.

Konzeptionell:

```text
Raw SKU
   ↓
TRIM()
   ↓
UPPER()
   ↓
Standardized SKU Key
   ↓
XLOOKUP / INDEX + MATCH
```

Dies reduziert Fehlausnahmen, die durch Formatierung und nicht durch Bestandsbewegung verursacht werden.

</details>

### Beispielszenario

Angenommen, eine wöchentliche Abstimmung wird für eine einzelne SKU durchgeführt, nachdem alle drei Systeme zum selben Stichtag erfasst wurden.

Die importierten Schnappschüsse melden:

| Quelle  | Menge |
| ------- | -------: |
| Shopify |    1.000 |
| WMS     |      992 |
| 3PL     |      970 |

Die konfigurierten Stückkosten der SKU betragen **18 $**.

Der erste analytische Schritt ist nicht, 30 Stück als verloren zu erklären. Das System stellt die Differenzen zwischen jeder gemeldeten Bestandsposition fest:

```text
Shopify vs. WMS
= 1,000 - 992
= 8 units

WMS vs. 3PL
= 992 - 970
= 22 units
```

Dies liefert sofort eine nützlichere betriebliche Frage.

Die Gesamtabweichung ist nicht einfach „30 Stück fehlen". Die Daten deuten darauf hin, dass die größte unerklärte Lücke zwischen dem WMS- und dem 3PL-Knoten konzentriert ist.

Wenn die 22-Stück-3PL-Abweichung nach Prüfung von Lieferzeitpunkten, Rückgaben, Anpassungen und anderen legitimen Bewegungen unerklärt bleibt, ist die geschätzte finanzielle Gefährdung bei den konfigurierten Kosten:

```text
22 × $18 = $396
```

Die Managementimplikation unterscheidet sich daher von einer generischen Bestandswarnung.

Die nächste Maßnahme ist nicht, jede SKU gleich zu inspizieren. Der Operator sollte zuerst die **3PL-seitige Ausnahme untersuchen**, prüfen, ob die Abweichung physischen Verlust, Beschädigung, Zeitprobleme oder ein Meldewesen darstellt, und dann bestimmen, ob die Abweichung die vertragliche oder interne Toleranz des Unternehmens überschreitet.

Das Dashboard ist darauf ausgelegt, diese Priorisierung sichtbar zu machen: das Management kann die gesamte finanzielle Gefährdung, die Verlustverteilung zwischen den Knoten und die wertstärksten SKU-Ausnahmen sehen, ohne die rohen Exporte manuell zu scannen.

Das Werkzeug unterstützt daher eine Sequenz von:

**Abstimmung → Ausnahmenisolierung → finanzielle Quantifizierung → betriebliche Untersuchung → potenzieller Anspruch oder Prozesskorrektur.**

Es bestimmt selbst nicht, ob eine Abweichung rechtlich erstattungsfähig ist. Das bleibt eine Management- und Vertragsentscheidung.

### Formelreferenz

Die folgenden Formeln beschreiben die für die Abstimmungsarchitektur spezifizierten Kernberechnungsmuster. Sie sollen die Argumentation der Arbeitsmappe prüfbar machen, statt das README in einen generischen Excel-Formelkatalog zu verwandeln.

<details>
<summary>SKU-Normalisierung</summary>

**Zweck:** importierte SKU-Zeichenfolgen vor dem Vergleich standardisieren.

```excel
=UPPER(TRIM([@SKU]))
```

**Logik:**

* `TRIM()` entfernt führende, nachgestellte und redundante Leerzeichen.
* `UPPER()` standardisiert die Groß-/Kleinschreibung von Buchstaben.
* Der resultierende normalisierte Schlüssel wird für systemübergreifenden Abgleich geeignet.

Die Quelle empfiehlt `TRIM()` und `UPPER()` ausdrücklich für diesen Zweck.

</details>

<details>
<summary>Systemübergreifender Abruf</summary>

**Zweck:** die entsprechende Menge aus einer Quelltabelle abrufen, nachdem die SKU standardisiert wurde.

```excel
=XLOOKUP(
    Normalized_SKU,
    Source_SKU_Column,
    Source_Quantity_Column,
    0
)
```

Die Architektur erlaubt `XLOOKUP` oder `INDEX + MATCH` als tabellenübergreifenden Abrufmechanismus.

Das wichtige Designprinzip ist nicht die spezifische Abruffunktion. Es ist, dass **SKU-Identität statt Zeilenposition die Abstimmung steuert**.

</details>

<details>
<summary>Varianzberechnung</summary>

**Zweck:** die Differenz zwischen vergleichbaren Bestandspositionen quantifizieren.

```text
Absolute Variance
= Source Quantity - Reference Quantity
```

Die Implementierung sollte das Vorzeichen bewahren, wo eine richtungsbezogene Interpretation nützlich ist, und Absolutwerte verwenden, wenn die Größe der Abweichung gereiht wird.

```text
Variance Magnitude
= ABS(Source Quantity - Reference Quantity)
```

Dies unterstützt sowohl:

* richtungsbezogene Abstimmung;
* Ausnahmenreihung.

</details>

<details>
<summary>Finanzverlust-Umrechnung</summary>

**Zweck:** Bestandsvarianz in eine geschätzte finanzielle Gefährdung umrechnen.

```text
Estimated Loss Value
= Variance Quantity × Unit Cost
```

Die Stückkosten werden in `Config_Master` gepflegt, wodurch dieselbe Abstimmungs-Engine wiederverwendet werden kann, wenn sich Produktkosten ändern.

Die Quelle definiert die Kostenmatrix ausdrücklich als Mechanismus zur Übersetzung von Bestandsabweichungen in finanziellen Verlust.

</details>

<details>
<summary>Relative Varianz und Risikoschwelle</summary>

**Zweck:** eine kleine numerische Differenz von einer materiellen betrieblichen Ausnahme unterscheiden.

Konzeptionell:

```text
Discrepancy Rate
= Absolute Variance ÷ Reference Inventory
```

Die resultierende Quote kann gegen die konfigurierte Warn- oder Toleranzschwelle verglichen werden.

Das Quelldesign sieht vor, dass `Config_Master` Abweichungsschwellen pflegt und bedingte Formatierung Zeilen markiert, deren Menge oder Abweichungsquote die konfigurierte Grenze überschreitet.

</details>

### Validierungsregeln

Die Abstimmungs-Engine hängt von einer kleinen Anzahl von Kontrollen ab, die respektiert werden müssen, bevor die Ausgabe als entscheidungsreif behandelt werden kann.

| Feld / Kontrolle                  | Regel                                                                                                           | Fehlerverhalten                                                                                                            |
| -------------------------------- | -------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| **SKU**                          | Muss standardisiert und konsistent über die Quelldateien hinweg identifizierbar sein.                                        | Nicht zugeordnete oder fehlerhafte Datensätze sollten als Datenqualitätsausnahmen behandelt werden statt stillschweigend als Schwund klassifiziert zu werden. |
| **SKU-Eindeutigkeit**               | Ein physisches Produkt sollte auf eine Standard-SKU-Identität abgebildet werden.                                                  | Doppelte oder widersprüchliche Kennungen erfordern eine Stammdatenkorrektur vor zuverlässiger Abstimmung.                       |
| **Stückkosten**                    | Muss für finanzielle Bewertung in `Config_Master` existieren.                                                         | Mengenvarianz kann noch sichtbar sein, aber finanzielle Gefährdung kann ohne Kosten nicht zuverlässig bewertet werden.                    |
| **Schnappschuss-Stichtag**             | Shopify-, WMS- und 3PL-Daten sollten denselben Zeitpunkt darstellen.                                               | Unterschiedliche Zeitstempel können falsche Varianz erzeugen und Re-Export oder Anpassung erfordern.                                       |
| **Importierte Quelldaten**         | Rohe Exporte sollten konsistent in ihre vorgesehenen Importzonen eingefügt werden.                                  | Strukturelle oder Quellformat-Anomalien sollten korrigiert werden, bevor die resultierenden Ausnahmen interpretiert werden.                   |
| **Abweichungsschwelle**        | Mengen-/Quotenschwellen sollten in der Konfiguration gepflegt werden statt in einzelne Ausgaben hartcodiert zu werden. | Ausnahmen, die die Schwelle überschreiten, werden zur Untersuchung markiert.                                                      |
| **3PL-Toleranz / SLA**          | Vertragliche Verlusttoleranz muss berücksichtigt werden, wenn entschieden wird, ob eine Ausnahme anspruchsberechtigt ist.              | Die Arbeitsmappe liefert Beweise; das Management bestimmt, ob ein vertraglicher Anspruch initiiert werden sollte.                    |
| **Rückgabezeitpunkte**               | Von einem 3PL erfasste Rückgaben und in Shopify erfasste Rückerstattungen können zu unterschiedlichen Zeiten auftreten.                        | Kurzfristige Nichtübereinstimmungen sollten nicht automatisch als dauerhafter Schwund interpretiert werden.                                     |
| **Historische SKU-Benennung**        | Legacy-Benennungsinkonsistenzen müssen normalisiert oder abgebildet werden.                                                    | Nicht abgebildete historische SKUs sollten als Datenqualitätsausnahmen sichtbar bleiben.                                                |
| **Systemsynchronisierungsverzögerung** | Vorübergehende Shopify-/3PL-Synchronisierungsprobleme liegen außerhalb der Abstimmungslogik der Tabelle.               | Als Systemintegrationsproblem behandeln statt eine VBA-basierte Tabellenkalkulations-Umgehung zu erzwingen.                               |

Die Quelle unterscheidet ausdrücklich zwischen Problemen, die Excel lösen kann, und Problemen, die betriebliche oder systemseitige Intervention erfordern. Standardisierte Abstimmung, Verlustbewertung und Ausnahmen-Dashboards gehören in die Arbeitsmappe; Zykluszählungsdisziplin, 3PL-Anspruchsverwaltung, API-Synchronisierung und GPS-Verfolgung nicht.



### Was diese Arbeitsmappe nicht zu lösen versucht

Die Architektur hält absichtlich eine klare Grenze um die Excel-Ebene aufrecht.

**Betriebliche Managementprobleme:**

* inkonsistente 3PL-Zykluszählungsverfahren;
* unzureichende physische Bestandszählhäufigkeit;
* Versäumnis, Ansprüche zu initiieren, wenn vertragliche Verlustgrenzen überschritten werden.

Diese erfordern Managementmaßnahmen statt einer weiteren Formel.

**Systemintegrationsprobleme:**

* Echtzeit-Shopify-↔-3PL-Synchronisierungsverzögerungen;
* API-Kommunikation;
* automatisierte ERP-Integration.

Die Quelle empfiehlt ausdrücklich, diese Probleme nicht durch VBA in eine leichtgewichtige Excel-Arbeitsmappe zu zwingen.

**Transporttransparenz-Probleme:**

* Echtzeit-GPS-Verfolgung von Bestand in Transit;
* Transportmanagement-Arbeitsabläufe.

Diese erfordern ein dediziertes TMS statt einer Bestandsabstimmungs-Tabelle.

Diese Grenze ist absichtlich. Der Zweck der Arbeitsmappe ist es, eine **wiederholbare Abstimmungs- und Finanzverlust-Analyseschicht** bereitzustellen, nicht vorzugeben, dass jedes Bestandskontrollproblem ein Excel-Problem ist.

### Die Arbeitsmappe holen

Das Werkzeug ist für wiederkehrende Abstimmung statt für einmalige Tabellenkalkulationsanalyse konzipiert.

Der beabsichtigte Betriebszyklus ist:

```text
Export Shopify inventory
        ↓
Export WMS inventory
        ↓
Export 3PL physical inventory
        ↓
Paste the three snapshots
        ↓
Refresh the reconciliation
        ↓
Review financial loss + exception ranking
        ↓
Investigate / correct / claim
```

Die Quell-Blaupause spezifiziert einen wöchentlichen oder monatlichen Rhythmus, wobei Benutzer die drei Quellexporte in ihre jeweiligen Eingabeblätter einfügen und aktuelle SKU-Kosten und Warnschwellen in `Config_Master` pflegen.

**Browserversion:** verwenden Sie die HTML-Version für eine schnelle betriebliche Durchsicht.

**Excel-Version:** verwenden Sie die Arbeitsmappe, wenn die Abstimmung mit tatsächlichen Shopify-, WMS- und 3PL-Exporten aktualisiert werden muss.

Das Werkzeug ist absichtlich so konzipiert, dass ein nicht-technischer Betriebs- oder Finanzanwender die wiederkehrende Abstimmung durchführen kann, ohne das analytische Modell jedes Mal neu aufzubauen. Das Quellziel sind etwa **10 Minuten** für Bereinigung, Abstimmung und Prüfung von Ausnahmen.

### Einschränkungen

Diese Arbeitsmappe ist eine **Abstimmungs- und Verlustanalyseschicht**, keine Bestandskontrollplattform.

Sie kann nicht:

* Echtzeit-Shopify-↔-WMS-↔-3PL-Synchronisierung garantieren;
* einen Lagermitarbeiter daran hindern, einen Artikel physisch zu versenden, wenn der Bestand unzureichend ist;
* ein WMS, ERP oder Bestandsmanagementsystem ersetzen;
* 3PL-Zykluszählungsverfahren durchsetzen;
* automatisch bestimmen, ob eine Abweichung vertraglich erstattungsfähig ist;
* Echtzeit-GPS-Verfolgung von Bestand in Transit bereitstellen;
* historische SKU-Stammdatenprobleme ohne eine angemessene Abbildungsentscheidung lösen.

Diese Grenzen sind im Quelldesign explizit. Standardisierte Abstimmung, Abweichungsbewertung, Ausnahmenreihung und Dashboard-Berichtswesen gelten als angemessene Excel-Probleme. Zykluszählungsdisziplin und 3PL-Anspruchsverwaltung erfordern Managementkontrollen; Echtzeit-API-Synchronisierung gehört zur Systemintegration; physische Sendungsverfolgung gehört zu einem TMS.

Es gibt auch wichtige Interpretationsbeschränkungen.

**Eine Mengendifferenz ist nicht automatisch Schwund.** Rückgaben können von einem 3PL zu einem anderen Zeitpunkt erfasst werden als die entsprechende Shopify-Rückerstattung, und inkonsistente Schnappschusszeitpunkte können temporäre Differenzen erzeugen. Der Operator muss den betrieblichen Kontext validieren, bevor eine Abweichung als dauerhafter Verlust klassifiziert wird.

**Die Finanzverlustzahl ist eine Schätzung, keine Buchung.** Sie hängt von den konfigurierten SKU-Stückkosten und der Interpretation der zugrunde liegenden Mengendifferenz ab.

**Ein sauberes Tabellenkalkulationsergebnis garantiert keine sauberen Quelldaten.** Historische SKU-Benennungsinkonsistenzen, unvollständige Exporte, doppelte Datensätze oder falsche physische Zählungen können dennoch irreführende Schlussfolgerungen erzeugen.

Die Arbeitsmappe sollte daher als **Mechanismus zur Faktenfindung und Priorisierung** verwendet werden, nicht als automatische Urteilsmaschine.

</details>


## Weitere Werkzeuge dieser Reihe

Eine Sammlung leichtgewichtiger Excel-Entscheidungsunterstützungs-Werkzeuge, die Betriebskontrolle, Abstimmung, Rentabilität, Bestand und Finanzanalyse abdecken.

* **Bestandsplanung & Nachbestellungssteuerung** — Bedarf, Nachschub, Bestandsgefährdung und Einkaufsentscheidungen.
* **Order-Level-Profit-Engine** — Umsatz, variable Kosten, Versandverteilung und Auftragsrentabilität.
* **Einzelprojekt-Bausteuerung** — Projektbudget, Verpflichtungen, Auftragskosten und Projektrentabilität.
* **Betriebs- & Rentabilitätsmanagementsystem für Auftragnehmer** — Arbeitsablauf Lead → Schätzung → Auftrag → Arbeit & Material → Auftragskosten → Gewinn → Kundenhistorie.

## Lizenz

Dieses Projekt steht unter der **Apache License 2.0**.

Sie dürfen das Projekt gemäß den Bedingungen der Apache License 2.0 verwenden, verändern, verteilen und anpassen.

Die vollständige Lizenz finden Sie in der Lizenzdatei des Repositorys.


