[ 🌐 عربي ](README.ar.md) | [ 🇩🇪 Deutsch ](README.de.md) | [ 🇫🇷 Français ](README.fr.md) | [ 🇳🇱 Nederlands ](README.nl.md) | [ 🇪🇸 Español ](README.sp.md) | [ 🇬🇧 English ](README.md)

# Voorraadreconciliatie Excel-sjabloon voor Shopify & 3PL: magazijnvoorraadverschillen, cyclustelling-variantie & shrinkagekosten-calculator
<img width="1102" height="790" alt="image" src="https://github.com/user-attachments/assets/3a637973-b460-4160-a098-eed931e2dc18" />



[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](#license)
[![Platform: Web Browser + Microsoft Excel (.xlsx)](https://img.shields.io/badge/Platform-Web%20Browser%20%2B%20Microsoft%20Excel%20(.xlsx)-217346.svg)](#quick-start-tutorial-how-to-reconcile-shopify-wms--3pl-inventory-in-4-steps)
[![Tool Type: Plug-and-Play Ecommerce Inventory Spreadsheet](https://img.shields.io/badge/Tool%20Type-Plug--and--Play%20Inventory%20Spreadsheet-2251FF.svg)](#what-it-helps-you-track-ecommerce-inventory-pain-points-vs-solutions)

**Een kant-en-klaar Shopify & 3PL voorraadreconciliatie Excel-sjabloon (`.xlsx`) en een gratis online voorraadverschillen-calculator, gebouwd voor e-commerce merken, DTC-operatoren en magazijnmanagers die voorraadtellingen willen auditen zonder zelf formules te schrijven.** Vergelijk **Shopify-webwinkel voorraadniveaus**, interne **Warehouse Management System (WMS)-registraties** en **fysieke cyclustellingen van je Third-Party Logistics (3PL)-partner** naast elkaar, bereken de **COGS-gewogen voorraadshrinkage ($)**, stop **oververkopen door spookvoorraad** en genereer **gedocumenteerde 3PL-terugvorderingsclaims** in één voorgebouwde spreadsheet.

**Test je SKU-data nu gratis in je browser, of download het ontgrendelde Excel-bestand voor maandelijkse audits.**

Elke SKU-matchregel, tekstopschoonformule en dollarafwijking-berekening is al ingebouwd. Kopieer en plak je ruwe CSV-exports uit Shopify, je WMS en je 3PL om binnen enkele seconden je exacte voorraadverschillen en financiële verliesexposure te zien — met een 30-daagse geld-terug-garantie zonder vragen.

> 🌐 **Probeer eerst de online reconciliatiecalculator**  
> [Start de gratis interactieve webcalculator voor Shopify & 3PL voorraadreconciliatie (browserdemo, geen installatie nodig)](https://hyvoid.github.io/multi-node-inventory-reconciliation/)
> 
> 📥 **Download het kant-en-klare Excel-sjabloon**  
> [Download het ontgrendelde multi-node voorraadreconciliatie- & shrinkage-audit Excel-sjabloon (.xlsx met automatisch bijwerkende formules)](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)
>
> *Zowel de gratis browsercalculator als de downloadbare Microsoft Excel-werkmap draaien op exact dezelfde voorgeconfigureerde 3-weg SKU-matching en COGS-variantietabellen.*

---

## Wat het je laat volgen: e-commerce voorraadpijnpunten vs. oplossingen

Ontdekken dat je voorraadcijfers niet kloppen is slechts de helft van het probleem — je moet ook weten waar de units zijn gebleven en hoeveel geld op het spel staat. Deze **plug-and-play voorraadaudit-spreadsheet** lost de vijf meest voorkomende blinde vlekken in voorraadbeheersing op voor multichannel e-commerce merken:

| Veelgezocht zoekonderwerp & volgdoel | Het dagelijkse e-commerce voorraadpijnpunt (waar geld weglekt) | Hoe dit voorgebouwde Excel-sjabloon het oplost en volgt |
| :--- | :--- | :--- |
| **Shopify vs. 3PL vs. WMS voorraadverschillen (`3-weg voorraadmatching`)** | Shopify zegt dat je 120 units hebt, je WMS zegt 100 en je 3PL zegt 85 — zonder dat je weet welk systeem de echte voorraadtelling bevat. | Legt **Shopify-, WMS- en 3PL-hoeveelheden per SKU naast elkaar** zodat je IT-synchronisatievertragingen kunt scheiden van echte fysieke magazijnverliezen. |
| **Shrinkagekosten & COGS-afboeking (`$`-impact vs. aantal units)** | Een verschil van 20 units op een $2 verpakkingsinvoegsel met dezelfde urgentie behandelen als een verlies van 20 units op een $75 toproduct. | Vermenigvuldigt unitvarianties met de **kostprijs per unit (COGS)** van elke SKU om de exacte **dollarschrinkage-exposure ($)** te berekenen voor boekhoudkundige afboekingen. |
| **Verloren 3PL-voorraad & SLA-terugvorderingsclaims (`Shrinkage-toelage` audit)** | Je weet dat je fulfillmentcenter merchandise verliest, maar je mist het SKU-niveau variantiebewijs dat nodig is voor een contractuele claim. | Volgt de **discrepantiepercentages (%) 3PL vs. intern magazijn** tegen je contractuele shrinkage-plafond om een feitelijk terugvorderingsregister op te bouwen. |
| **Spookvoorraad & oververkopen in het hoogseizoen (`voorraaduitval`-preventie)** | Shopify toont meer beschikbare units dan er echt op de 3PL-schappen liggen, waardoor betaalde advertenties orders genereren die je moet annuleren en terugbetalen — met verkoopbaarheid en marge als gevolg. | Vlagt elke SKU waar **digitale winkelvoorraad de fysieke 3PL-voorraad overschrijdt** zodat je voorraadniveaus corrigeert vóór het oververkopen. |
| **Analyseparalyse bij cyclustelling (`Top 10 SKU's naar verlieswaarde`)** | Duizenden spreadsheetrijen doorscrollen na een magazijn-cyclustelling terwijl je de 5 SKU's mist die 80% van je financiële verlies veroorzaken. | Filtert automatisch overeenkomende rijen uit en rangschikt de **Top 10 SKU's met de hoogste dollarverlies** op één overzichtsdashboard voor directe actie. |

---

## Snelstart-tutorial: hoe je Shopify-, WMS- & 3PL-voorraad in 4 stappen reconcilieert

Je hebt geen geavanceerde Excel-vaardigheden of handmatige `VLOOKUP`-formules nodig om een magazijnaudit uit te voeren. Volg deze vier stappen om ruwe CSV-exports om te zetten in een duidelijk **voorraadshrinkage- & discrepancyrapport**:

### Stap 1: Vul je SKU-stamlijst, unit-COGS & waarschuwingsdrempels in (`Config_Master`)
Open het `Config_Master`-tabblad om je voorraadregels als baseline in te stellen:
- Plak je **SKU-lijst** en de **kostprijs per verkochte eenheid (COGS)**.
- Stel je aangepaste **waarschuwingsdrempels voor discrepanties** in (markeer bijvoorbeeld elke SKU met een verschil van meer dan `5 units` of meer dan `$100` aan ontbrekende voorraadwaarde).

*Bekijk het live:* zie hoe de stamconfiguratietabel nu werkt in de [gratis online 3PL voorraadreconciliatie-browsercalculator](https://hyvoid.github.io/multi-node-inventory-reconciliation/).

---

### Stap 2: Kopieer en plak je ruwe Shopify-, WMS- & 3PL-CSV-exports
Sla handmatige kolomopmaak en tekstopschoning over. Plak je ruwe voorraadexports direct in de drie invoertabbladen:
- `Import_Shopify`: je geëxporteerde Shopify-productvoorraad CSV (voorraadniveaus van de webwinkel).
- `Import_WMS`: je interne magazijnbeheer- of ERP-voorraadrapport.
- `Import_3PL`: de fysieke cyclustelling of eindvoorraadrapportage van je fulfillmentpartner (compatibel met exports van ShipBob, ShipMonk, Flexport, Amazon MCF en eigen 3PL-portals).
- **Nul handmatig formules slepen:** de voorgebouwde tabellen reinigen overtollige spaties, stemmen SKU-codes af en breiden automatisch uit wanneer je nieuwe rijen plakt.

---

### Stap 3: Bekijk je shrinkagedashboard & Top 10 SKU's naar verlieswaarde (`Dashboard`)
Schakel naar het `Dashboard`-tabblad om je voltooide auditresultaten te bekijken:
- Zie de totale **shrinkagewaarde ($)**, de **netto unitvariantie** en de **systeem-tot-systeem nauwkeurigheidspercentages (%)** automatisch berekend.
- Bekijk de lijst **Top 10 SKU's naar verlieswaarde** om te zien welke exacte producten een fysieke hertelling in het magazijn of een dringende voorraadcorrectie op Shopify nodig hebben.

---

### Stap 4: Download het ontgrendelde Excel-sjabloon voor maandelijkse audits met één klik
Gebruik de gratis browsertool om vandaag nog je workflow te testen en directe voorraadgaten te ontdekken. Om je SKU-kostenbaselines lokaal op te slaan, terugkerende maandelijkse boekhoudafsluitingen uit te voeren en historische 3PL-claimlogboeken op te bouwen, download je de ontgrendelde `.xlsx`-spreadsheet.

> 💡 **Waarom groeiende e-commerce merken dit Excel-sjabloon gebruiken in plaats van zelf te bouwen:**  
> Rommelige SKU-strings over drie verschillende exports heen schoonmaken, niet-overeenkomende rijen afstemmen en voorraadvarianties wegen op unit-COGS vergt lastige spreadsheet-engineering. **In dit Excel-sjabloon is elke 3-weg matchregel, tekstnormalisator en automatisch bijwerkende formule al voor je gebouwd.**  
> 
> Je hoeft niet eens op celhoeken te dubbelklikken of formules naar beneden te slepen. Download de werkmap naar je computer, plak je maandelijkse Shopify- en 3PL-exports over de data van vorige maand en krijg een bijgewerkte financiële shrinkage-audit met één klik. Zelfs zonder technische spreadsheetachtergrond krijg je direct inzicht in je voorraadgezondheid — zodat je je kunt richten op marketing, bijbestellen van bestsellers en het afsluiten van verkopen tijdens de piekmaanden Q4 en Black Friday, terwijl een eenvoudig kopieer-en-plak-sjabloon de datareconciliatie afhandelt.  
> 
> 👉 **[Download vandaag het ontgrendelde Shopify & 3PL voorraadreconciliatie Excel-sjabloon (.xlsx) en automatiseer je voorraadaudits](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)**

---

## De bedrijfslogica & methodiek: 4 verborgen voorraadblinde vlekken die dit Excel-sjabloon voor je oplost

De meeste e-commerce merken verliezen duizenden dollars aan voorraadshrinkage en oververkopen, niet omdat ze vergeten voorraad te tellen, maar omdat standaard 2-weg controles en eenvoudige unit-spreadsheets verbergen waar de echte financiële schade ontstaat. Hier is hoe dit sjabloon je voorraad en cashflow in gewone taal beschermt:

### 1. Alleen twee systemen vergelijken verbergt of je een IT-bug of magazijndiefstal hebt (3-weg voorraadtriangulatie)
**De objectieve feiten:** als je alleen Shopify (100 units) vergelijkt met je 3PL (80 units), weet je dat 20 units ontbreken, maar je weet niet *waarom*. Die 20 units kunnen in niet-verzonden orders zitten omdat een API-webhook faalde, of 20 fysieke dozen kunnen via de achterdeur het magazijn uit zijn gelopen.  
**Jouw directe voordeel:** door **Shopify (digitale webwinkel) + WMS (intern grootboek) + 3PL (fysieke schaptelling)** naast elkaar in één rij te leggen, isoleert het sjabloon het exacte breekpunt:
- Als `Shopify ≠ WMS`, maar `WMS = 3PL`: je hebt een winkelsynchronisatie- of niet-verzonden-ordervertraging. Corrigeer je integratie-instellingen.
- Als `Shopify = WMS`, maar `3PL < WMS`: fysieke voorraad is verloren gegaan, beschadigd of misgeteld in het fulfillmentcenter. Dien een 3PL-claim in.

### 2. Ontbrekende units tellen in plaats van ontbrekende dollars verspilt magazijnarbeid (COGS-gewogen variantieranking)
**De objectieve feiten:** een standaard cyclustellingsblad behandelt elke unit gelijk. Als je team discrepancies alleen op aantal units sorteert, zullen ze uren bestaan aan het hertellen van goedkope verpakkingsmaterialen terwijl ze dure producten negeren die stilletjes je winstmarge aantasten. Kijk hoe ruwe unaantallen magazijnteams misleiden vergeleken met COGS-gewogen shrinkage:

```text
SKU-A (Branded Poly-Mailer):   -50 Units Missing  ×  $0.20 Unit COGS  =   -$10.00 Financial Loss
SKU-B (Wireless Headphones):    -4 Units Missing  × $115.00 Unit COGS =  -$460.00 Financial Loss

```

In een basale spreadsheet op unaantal lijkt `SKU-A` (-50 units) een noodgeval terwijl `SKU-B` (-4 units) een kleine afrondingsfout lijkt — terwijl `SKU-B` je bedrijf **46 keer meer geld** kost.

**Jouw directe voordeel:** het sjabloon vermenigvuldigt elke unitdiscrepancie automatisch met de unit-COGS en rangschikt je **Top 10 SKU's naar verlieswaarde op dollarimpact**. Je team onderzoekt eerst het $460-verlies in plaats van $10 aan enveloppen na te jagen.

### 3. 3PL fulfillmentcontracten hebben strikte claimdeadlines en shrinkageplafonds (gedocumenteerd SLA-claimbewijs)

**De objectieve feiten:** bijna alle Third-Party Logistics (3PL)-contracten bevatten een ingebouwde "shrinkage-toelage" (meestal 0,5% tot 2,0% van het totale aantal behandelde units) en eisen dat handelaren binnen 15 tot 30 dagen na een cyclustelling SKU-voor-SKU-variantiebewijs indienen om in aanmerking te komen voor terugbetaling. Klachten die per e-mail worden verstuurd zonder gestructureerde variantielogboeken worden routinematig afgewezen door 3PL-accountmanagers.

**Jouw directe voordeel:** het sjabloon berekent exacte **node-tot-node discrepantiepercentages** en genereert een overzichtelijke SKU-variantietabel met verwachte voorraad, fysieke telling, tekort aan units en COGS-waarde — zodat je kant-en-klare documentatie hebt om geld terug te vorderen van je 3PL.

### 4. "Spookvoorraad" op Shopify verbrandt betaalde advertentiebudgetten en veroorzaakt chargebacks (fantomenvoorraaddetectie)

**De objectieve feiten:** wanneer je Shopify-winkel denkt dat je 50 units op voorraad hebt, blijven je Meta- en Google-shoppingadvertenties geld uitgeven om verkeer naar die productpagina te trekken. Als je 3PL in werkelijkheid 0 units op de schap heeft ("spookvoorraad"), leidt elke nieuwe klantorder tot een fulfillmentvertraging, een handmatige annulering, verloren betaalverwerkingskosten en boze klantensupporttickets.

**Jouw directe voordeel:** het sjabloon markeert elke SKU waar webwinkelbeschikbaarheid de fysieke magazijnvoorraad overschrijdt zodat je Shopify-voorraadhoeveelheden kunt aanpassen vóór het oververkopen tijdens drukke verkoop events.

---

## Handmatige voorraadspreadsheets (`VLOOKUP`) vs. dit geautomatiseerde Shopify & 3PL reconcilietiesjabloon

| Magazijn- & boekhoudkundige vergelijkingsfactor | Handmatige Excel-sheets (`VLOOKUP` / `INDEX-MATCH` vanaf nul) | Gestandaardiseerd multi-node voorraadreconcilietiesjabloon (deze tool) |
| --- | --- | --- |
| **Voorraadafstemming over 3 systemen (`Shopify` + `WMS` + `3PL`)** | Medewerkers stikken elke maand handmatig drie losse CSV-bestanden aan elkaar, met risico op kapotte celverwijzingen en overgeslagen SKU's. | De voorgebouwde **3-weg matching-engine** stemt Shopify-, WMS- en 3PL-hoeveelheden automatisch af zodra je je exports plakt. |
| **Rommelige CSV-opmaak & SKU-mismatches** | Extra spaties aan het einde, voorloopnullen en hoofdlettergevoelige SKU-codes veroorzaken valse `#N/A`-fouten over duizenden rijen. | Een ingebouwde **tekstnormalisatielaag** reinigt witruimte en standaardiseert SKU-strings voordat voorraadverschillen worden berekend. |
| **Financiële shrinkagewaardering (`COGS-afboeking`)** | Rapporten tonen alleen ontbrekende unaantallen, waardoor boekhouders productkosten handmatig moeten opzoeken bij de maandafsluiting. | Een ingebouwde **SKU-kostenmatrix** zet elk unietekort om in exacte **dollarschrinkage-exposure ($)** voor boekhoudkundige boeking. |
| **Uitzonderingsfiltering (`Top verlies-SKU's`)** | Managers scrollen door meer dan 5.000 overeenkomende rijen om te ontdekken welke producten gevaarlijke voorraadgaten hebben. | Het **geautomatiseerde uitzonderingsdashboard** filtert normale rijen uit en rangschikt automatisch de **Top 10 SKU's met de hoogste dollarverlies**. |
| **3PL SLA-terugvorderingsdocumentatie** | Ontbrekende magazijnunits worden informeel besproken via e-mail zonder historische nauwkeurigheidspercentages of dollartotalen. | Levert een auditklare **3PL-variantie- & discrepancypercentage-ledger** om formele SLA-credits en terugvorderingsclaims te onderbouwen. |

---

## Voor wie is dit: e-commerce rollen, voorraadgebruiksscenario's & spreadsheetworkflows

Deze toolkit overbrugt de kloof tussen fysieke magazijnplanken en e-commerce financiële rapportages. Hij is gebouwd voor **groeiende DTC-merken, multichannel Shopify-verkopers, 3PL-gebruikers en e-commerce financeteams** die betrouwbare voorraadbeheersing willen zonder $30.000+ per jaar te betalen voor een enterprise ERP:

* **Shopify-winkeleigenaren & DTC-merkoprichters (`Shopify voorraadreconciliatie Excel-sjabloon`):** spot spookvoorraad en ontbrekende magazijnvoorraad binnen enkele minuten zonder een data-analist in te huren of complexe spreadsheetformules te leren.
* **E-commerce operations- & fulfillmentmanagers (`3PL voorraaddiscrepantie- & SLA-audit spreadsheet`):** houd externe fulfillmentcentra (zoals ShipBob, ShipMonk of regionale 3PL's) verantwoordelijk door maandelijkse shrinkagepercentages te volgen tegen contractuele SLA-plafonds.
* **Magazijnmanagers & voorraadbeheerders (`plug-and-play cyclustelling variantiecalculator`):** reconcileer fysieke bin-tellingen met WMS-grootboekregistraties na wekelijkse of maandelijkse cyclustellingen, met prioriteit voor hertellingen op basis van de hoogste dollarwaarde die op het spel staat.
* **E-commerce boekhouders & fractional CFO's (`voorraadshrinkage- & COGS-afboekingsmodel`):** bereken exacte eindvoorraadwaardering-aanpassingen en maandelijkse COGS-shrinkage-afboekingen voor QuickBooks Online, Xero of NetSuite.
* **Multichannel Amazon-, Walmart- & Shopify-verkopers (`multi-magazijn voorraadvergelijkingsblad`):** audit voorraaddistributie en niet-gekoppelde SKU-hoeveelheden over interne magazijnen, 3PL-nodes en online verkoopkanalen vanuit één bestand.

*Opmerking: deze Excel-werkmap vervangt geen live barcodescanners, realtime API-voorraadsynchronisatie-apps of je WMS. Het fungeert als je onafhankelijke **audit- en reconciliatielaag** om de synchronisatiefouten en fysieke shrinkage te vinden die geautomatiseerde software mist.*

---

## Praktijksenario's: hoe je veelvoorkomende Shopify- & 3PL-voorraadproblemen oplost

Als je operations- of financeteam een van deze terugkerende voorraadhoofdpijn tegenkomt, is deze spreadsheet zo gebouwd dat ze uit de doos worden opgelost:

* **Hoe je oververkopen voorkomt tijdens Black Friday / Cyber Monday (Q4 hoogseizoen):** Shopify toont 100 beschikbare units, maar je 3PL heeft er slechts 20 op de schap. Voer deze reconciliatie wekelijks uit tijdens Q4 om "spookvoorraad" te vangen en je winkeltellingen te synchroniseren voordat klanten uitverkochte artikelen kopen.
* **Hoe je verloren 3PL-voorraad bewijst en SLA-terugbetalingen claimt:** je fulfillmentpartner verliest high-ticket SKU's boven zijn contractuele shrinkage-toelage van 1,5%. Plak je WMS-verzendlogboeken en de fysieke telling van de 3PL in het sjabloon om een gedetailleerd dollarverliesrapport voor je terugvorderingsclaim te genereren.
* **Hoe je maandelijkse voorraadshrinkage berekent voor e-commerce boekhouding:** je boekhouder heeft een exact dollarcijfer nodig voor verloren of beschadigde voorraad om de maandelijkse P&L af te sluiten. Gebruik het COGS-gewogen dashboards totaal om in enkele minuten nauwkeurige voorraadafboekingsjournaalposten te boeken.
* **Hoe je rommelige magazijn-CSV-exports reconcileert zonder kapotte `VLOOKUP`-formules:** verschillende systemen exporteren SKU-codes met extra spaties of inconsistente opmaak. Drop de ruwe exports in de invoertabbladen en laat het sjabloon elke SKU automatisch afstemmen en vergelijken.

---

## Over Theseus Workshop

**Theseus Workshop** bouwt plug-and-play Microsoft Excel-modellen en browsergebaseerde beslissingstools voor operatoren die vandaag duidelijke, betrouwbare cijfers nodig hebben — zonder opgeblazen enterprise-software of complexe spreadsheetprogrammering.

Elke tool is ontworpen rond één praktische vraag:

> **"Welke exacte operationele en financiële cijfers moeten in één voorgebouwde tabel staan zodat je volgende zakelijke beslissing seconden in plaats van uren kost?"**

Als je wilt stoppen met worstelen met kapotte `VLOOKUP`-sheets, verrassingsvoorraaduitval en ongecompenseerde 3PL-vooraadverliezen, pak dan hieronder het volledige Excel-sjabloon of verken onze complete bibliotheek met operationele spreadsheets:

* 📥 **Download dit voorraadreconcilietiesjabloon:** [Download het ontgrendelde Shopify & 3PL voorraadreconciliatie Excel-sjabloon (.xlsx)](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)
* 🌐 **Test de gratis webcalculator:** [Open de interactieve 3PL voorraadreconciliatie-browsersimulator](https://hyvoid.github.io/MULTI-NODE-INVENTORY-RECONCILIATION/)
* 🧰 **Verken alle kant-en-klare Excel-modellen & businesskits:** [Bezoek de officiële Theseus Workshop Store op TheseusWorkshop.com](https://www.google.com/search?q=https://www.theseusworkshop.com%3Futm_source%3Dgithub%26utm_medium%3DGitHub%2520README%26utm_campaign%3Dreadme%2520new%2520launch%26utm_content%3Dinventory-readme-store-link)

---


## Technische details

<details>
<summary>Voor technische reviewers, Excel-beoefenaars en medewerkers</summary>

### Werkmaparchitectuur

De werkmap is bewust gestructureerd als een **data-opschoon- en reconciliatie-engine + beslissingsdashboard voor financieel verlies**, en niet als een permanente voorraaddatabase. Elke reconciliecyclus kan de vorige importset overschrijven of als aparte werkmap worden opgeslagen, waardoor het bestand lichtgewicht blijft en onnodige database- of macro-afhankelijkheden worden vermeden.

De architectuur volgt een eenvoudige:

**Input → Normaliseren → Reconciliëren → Kwantificeren → Vlaggen → Presenteren**

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

De werkmap is verdeeld in zes functionele werkbladen:

| Werkblad         | Laag          | Verantwoordelijkheid                                                      | Primaire gebruiker      |
| ---------------- | ------------- | ------------------------------------------------------------------------- | ---------------------- |
| `Dashboard`      | Beslissing    | KPI-samenvatting, verliesblootstelling, nodevergelijking, Top 10 uitzonderingen            | CEO / Management        |
| `Config_Master`  | Configuratie  | Standaard SKU-lijst, productinformatie, kostprijs, discrepantiedrempels | Operations / Finance   |
| `Import_Shopify` | Input         | Ruwe Shopify-voorraadexport                                               | Operations              |
| `Import_WMS`     | Input         | Ruwe interne WMS-voorraadexport                                           | Magazijn / Operations   |
| `Import_3PL`     | Input         | Ruwe 3PL fysieke voorraadexport                                           | 3PL / Operations        |
| `Calc_Engine`    | Berekening    | Datanormalisatie, SKU-matching, variantieberekeningen, financiële impact  | Verborgen technische laag |

De drie importwerkbladen worden bewust als **plakzones** gehouden. De bron-specificatie staat gebruikers toe de originele exports direct te plakken, inclusief compatibiliteit met voorlooprijen die leeg zijn, in plaats van hen te dwingen de bestanden vóór de reconciliatie handmatig te herstructureren.

### Datastroom en reconciliatielogica

De centrale rekenlaag gebruikt `Config_Master` als referentiepunt voor gestandaardiseerde SKU's.

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

Het ontwerp pakt specifiek het probleem van **rommelige data** aan. De bronarchitectuur voorziet `TRIM()` om verborgen of toevallige spaties te verwijderen en `UPPER()` om hoofdlettergebruik te normaliseren, gevolgd door `XLOOKUP` of `INDEX + MATCH` voor niet-invasieve kruistabelopvraag.

Dit is belangrijk omdat een SKU als:

```text
ABC-001
```

geen valse uitzondering mag worden simpelweg omdat een andere export bevat:

```text
 abc-001
```

De reconciliatie-engine behandelt normalisatie daarom als een voorwaarde vóór vergelijking, in plaats van te proberen datakwaliteitsproblemen op te lossen nadat het variantierapport al is gegenereerd.

### Het afsnijmoment-principe van reconciliatie

Voorraadsnapshots moeten het **zelfde zakelijke afsnijmoment** vertegenwoordigen.

Bijvoorbeeld:

```text
Shopify Snapshot     → Sunday 23:59:59
WMS Snapshot         → Sunday 23:59:59
3PL Physical Count   → Sunday 23:59:59
```

Als de snapshots op wezenlijk verschillende momenten worden genomen, kunnen voorraadbewegingen, retourzendingen of orders in transit schijnbare verschillen creëren die geen echte shrinkage zijn.

De bronarchitectuur identificeert expliciet een consistente afsnijtijd als een kernoperationele beperking en waarschuwt dat mismatched snapshots «valse verschillen» kunnen creëren.

Dit is daarom een **zakelijke beheerseis**, niet louter een vereiste van spreadsheetformules.

### De SKU als de enkele reconcilie-sleutel

De SKU wordt behandeld als de standaardidentiteit die de drie bronsystemen verbindt.

De configuratielaag onderhoudt:

* Standaard SKU
* Productnaam
* Kostprijs per eenheid
* Discrepantiedrempel
* Waarschuwingsdrempel

De rekenengine gebruikt die standaardsleutel vervolgens om hoeveelheden uit elke bron op te halen.

Dit voorkomt dat de reconciliatie afhangt van de rijvolgorde van de geïmporteerde bestanden. Shopify kan SKU's in de ene volgorde tonen, WMS in een andere en 3PL in een derde; de rekenengine vergelijkt nog steeds hetzelfde product met hetzelfde product.

De bron-specificatie benadrukt uniciteit en consistentie van SKU's als fundamentele beperking: één fysiek product mag niet door meerdere inconsistente identificatoren worden vertegenwoordigd.

### Dashboardarchitectuur

Het Dashboard is bewust ontworpen voor **uitzondering-eerst-management**, niet voor het reproduceren van de ruwe brontabellen.

De primaire KPI-laag bevat:

* Totale hoeveelheidsvariantie
* Totale geschatte financiële verlies
* 3PL-discrepantiepercentage
* Intern magazijn-discrepantiepercentage

De visuele laag biedt vervolgens:

* Verlieswaardeverdeling tussen 3PL en intern magazijn
* Top 10 SKU's gerangschikt op verlieswaarde
* Identificatie van hoogrisicouitzonderingen

Deze uitvoeren zijn direct gespecificeerd in de bronarchitectuur.

De beoogde managementvolgorde is:

```text
How much is different?
        ↓
How much money is exposed?
        ↓
Where is the exposure concentrated?
        ↓
Which SKUs matter most?
        ↓
Which exceptions should be investigated?
        ↓
Is a process correction or 3PL claim required?
```

Daarom wordt deze werkmap beter begrepen als een **beslissingsondersteuningslaag** dan als een eenvoudige voorraadvergelijkingsspreadsheet.

### Drie valkuilen die zelfs ervaren voorraadoperatoren raken

#### Valkuil 1 — Elke hoeveelheidsverschil als shrinkage behandelen

**Beslissing:**
Een operator ziet dat Shopify 1.000 stuks rapporteert terwijl de 3PL er 970 rapporteert en registreert onmiddellijk 30 stuks als verloren.

**Fout cijfer:**
De vergelijking gebruikt snapshots die op verschillende momenten zijn genomen.

**Waarom de aanbeveling verandert:**
Het verschil van 30 stuks kan zendingen, retourzendingen, correcties of andere bewegingen tussen de twee snapshots vertegenwoordigen.

**Juiste aanpak:**
Leg eerst een gemeenschappelijk afsnijmoment vast en vergelijk vergelijkbare voorraadsnapshots.

| Aanpak                          | Resultaat                                              |
| ------------------------------- | ------------------------------------------------------ |
| Snapshots op verschillende tijden | Verschil van 30 stuks als verlies behandeld          |
| Gemeenschappelijk afsnijmoment  | Alleen de resterende onverklaarde variantie wordt onderzocht |

De bron identificeert afsnij-inconsistentie specifiek als oorzaak van valse discrepanties.

De gecorrigeerde beslissing is daarom **«onderzoek de resterende variantie»**, niet **«claim de volledige variantie als shrinkage»**.

<details>
<summary>Berekeningslogica</summary>

```text
Comparable Variance
= Quantity at Node A
- Quantity at Node B

Only when:
Snapshot_A_Time = Snapshot_B_Time
```

Een discrepancy mag pas als financieel verlies worden geïnterpreteerd wanneer de vergelijkingsbasis zelf geldig is.

</details>

#### Valkuil 2 — Problemen rangschikken op stuks in plaats van op geld

**Beslissing:**
De operator sorteert het reconcilierapport op de grootste hoeveelheidsdiscrepantie.

**Foute metric:**
Een afwijking van 50 stuks wordt hoger gerangschikt dan een van 10 stuks simpelweg omdat `50 > 10`.

**Waarom de aanbeveling incompleet is:**
Hoeveelheid vertegenwoordigt geen economische significantie.

Stel:

| SKU   | Afwijking | Kostprijs | Geschatte blootstelling |
| ----- | -------: | --------: | -----------------: |
| SKU-A |       50 |        $2 |               $100 |
| SKU-B |       10 |       $40 |               $400 |

Een rangschikking alleen op hoeveelheid zou eerst SKU-A onderzoeken. Een rangschikking op financieel verlies zou eerst SKU-B onderzoeken.

De bronarchitectuur vraagt expliciet om een SKU-kostenmatrix in te voeren, zodat hoeveelheidsverschillen kunnen worden vertaald naar financieel verlies.

**Juiste beslissing:** prioriteer uitzonderingen op basis van zowel **hoeveelheidsvariantie als financiële blootstelling**, niet alleen op hoeveelheid.

<details>
<summary>Berekeningslogica</summary>

```text
Estimated Loss Value
= Variance Quantity × Unit Cost
```

Voor het voorbeeld:

```text
SKU-A = 50 × $2  = $100
SKU-B = 10 × $40 = $400
```

De tweede uitzondering heeft de kleinere hoeveelheid maar de grotere financiële consequentie.

</details>

#### Valkuil 3 — Aannemen dat een schone SKU-match schone data betekent

**Beslissing:**
De operator gebruikt een directe opvraag tussen de drie exports en gaat ervan uit dat niet-matchende records ontbrekende voorraad vertegenwoordigen.

**Foute aanname:**
Er wordt van uitgegaan dat de SKU-strings identiek zijn over de systemen heen.

**Waarom de aanbeveling verandert:**
Geëxporteerde data kan voorloop-/naloopspaties, inconsistent hoofdlettergebruik, speciale tekens, lege rijen of historische SKU-naamgevingsconventies bevatten. De bron identificeert deze specifiek als praktische datakwaliteitsproblemen.

Bijvoorbeeld:

```text
Shopify → "sku-001"
WMS     → "SKU-001"
3PL     → " SKU-001 "
```

Een naïeve exacte match kan deze als verschillende producten interpreteren.

**Juiste aanpak:** normaliseer de identificator vóór de systeemoverstijgende opvraag.

<details>
<summary>Normalisatielogica</summary>

```excel
=UPPER(TRIM([@SKU]))
```

Gebruik vervolgens de genormaliseerde sleutel voor de kruistabelopvraag.

Conceptueel:

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

Dit vermindert valse uitzonderingen veroorzaakt door opmaak in plaats van voorraadbeweging.

</details>

### Voorbeeldscenario

Stel dat een wekelijkse reconciliatie wordt uitgevoerd voor één SKU nadat alle drie de systemen op hetzelfde afsnijmoment zijn vastgelegd.

De geïmporteerde snapshots rapporteren:

| Bron    | Hoeveelheid |
| ------- | -------: |
| Shopify |    1,000 |
| WMS     |      992 |
| 3PL     |      970 |

De geconfigureerde kostprijs van de SKU is **$18**.

De eerste analytische stap is niet om 30 stuks als verloren te declareren. Het systeem stelt de verschillen vast tussen elke gerapporteerde voorraadpositie:

```text
Shopify vs. WMS
= 1,000 - 992
= 8 units

WMS vs. 3PL
= 992 - 970
= 22 units
```

Dit levert onmiddellijk een nuttigere operationele vraag op.

De totale discrepantie is niet simpelweg «30 stuks kwijt». De data suggereert dat de grootste onverklaarde kloof geconcentreerd is tussen de WMS- en de 3PL-node.

Als de 3PL-variantie van 22 stuks onverklaard blijft na het controleren van verzendtiming, retourzendingen, correcties en andere legitieme bewegingen, is de geschatte financiële blootstelling tegen de geconfigureerde kostprijs:

```text
22 × $18 = $396
```

De managementimplicatie verschilt daarom van een generieke voorraadwaarschuwing.

De volgende actie is niet om elke SKU gelijk te inspecteren. De operator moet eerst de **3PL-zijuitzondering onderzoeken**, verifiëren of de variantie fysiek verlies, schade, timing of een rapportageprobleem vertegenwoordigt, en vervolgens bepalen of de discrepancy de contractuele of interne tolerantie van het bedrijf overschrijdt.

Het dashboard is ontworpen om deze prioritering zichtbaar te maken: het management kan de totale financiële blootstelling, de verliesverdeling tussen nodes en de SKU-uitzonderingen met de hoogste waarde zien zonder handmatig de ruwe exports te doorzoeken.

De tool ondersteunt daarom een reeks van:

**reconciliatie → uitzonderingsisolatie → financiële kwantificering → operationeel onderzoek → mogelijke claim of procescorrectie.**

De tool zelf bepaalt niet of een discrepancy juridisch verhaalbaar is. Dat blijft een management- en contractbeslissing.

### Formuliereferentie

De onderstaande formules beschrijven de kernberekeningspatronen die voor de reconciliatiearchitectuur zijn gespecificeerd. Ze zijn bedoeld om het redeneren van de werkmap auditeerbaar te maken, niet om van de README een generieke Excel-formulecatalogus te maken.

<details>
<summary>SKU-normalisatie</summary>

**Doel:** standaardiseer geïmporteerde SKU-strings vóór vergelijking.

```excel
=UPPER(TRIM([@SKU]))
```

**Logica:**

* `TRIM()` verwijdert voorloop-, naloop- en overtollige spaties.
* `UPPER()` standaardiseert hoofdlettergebruik.
* De resulterende genormaliseerde sleutel is geschikt voor systeemoverstijgende matching.

De bron raadt `TRIM()` en `UPPER()` specifiek voor dit doel aan.

</details>

<details>
<summary>Systeemoverstijgende opvraag</summary>

**Doel:** haal de bijbehorende hoeveelheid op uit een brontabel nadat de SKU is gestandaardiseerd.

```excel
=XLOOKUP(
    Normalized_SKU,
    Source_SKU_Column,
    Source_Quantity_Column,
    0
)
```

De architectuur staat `XLOOKUP` of `INDEX + MATCH` toe als kruistabel-opvraagmechanisme.

Het belangrijke ontwerpprincipe is niet de specifieke opvraagfunctie. Het is dat **de SKU-identiteit, en niet de rijpositie, de reconciliatie aanstuurt**.

</details>

<details>
<summary>Variantieberekening</summary>

**Doel:** kwantificeer het verschil tussen vergelijkbare voorraadposities.

```text
Absolute Variance
= Source Quantity - Reference Quantity
```

De implementatie moet het teken behouden wanneer directionele interpretatie nuttig is en absolute waarden gebruiken bij het rangschikken van de omvang van de discrepantie.

```text
Variance Magnitude
= ABS(Source Quantity - Reference Quantity)
```

Dit ondersteunt beide:

* directionele reconciliatie;
* rangschikking van uitzonderingen.

</details>

<details>
<summary>Conversie naar financieel verlies</summary>

**Doel:** converteer voorraadvariantie naar een geschatte financiële blootstelling.

```text
Estimated Loss Value
= Variance Quantity × Unit Cost
```

De kostprijs wordt bijgehouden in `Config_Master`, waardoor dezelfde reconciliatie-engine hergebruikt kan worden wanneer productkosten veranderen.

De bron definieert de kostenmatrix expliciet als het mechanisme om voorraaddiscrepanties te vertalen naar financieel verlies.

</details>

<details>
<summary>Relatieve variantie en risicodrempel</summary>

**Doel:** onderscheid een kleine numerieke afwijking van een materiële operationele uitzondering.

Conceptueel:

```text
Discrepancy Rate
= Absolute Variance ÷ Reference Inventory
```

Het resulterende percentage kan worden vergeleken met de geconfigureerde waarschuwings- of tolerantiedrempel.

Het bronontwerp voorziet dat `Config_Master` de discrepantiedrempels bijhoudt en dat voorwaardelijke opmaak rijen markeert waarvan de hoeveelheid of het discrepantiepercentage de geconfigureerde limiet overschrijdt.

</details>

### Validatieregels

De reconciliatie-engine hangt af van een klein aantal controles die gerespecteerd moeten worden voordat de uitvoer als besliskwaliteit kan worden behandeld.

| Veld / Controle                  | Regel                                                                                                           | Foutgedrag                                                                                                            |
| -------------------------------- | -------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| **SKU**                          | Moet gestandaardiseerd en consistent identificeerbaar zijn over de bronbestanden heen.                                        | Niet-matchende of misvormde records moeten worden behandeld als datakwaliteitsuitzonderingen in plaats van stilzwijgend als shrinkage te worden geclassificeerd. |
| **SKU-uniekheid**               | Eén fysiek product moet naar één standaard SKU-identiteit verwijzen.                                                  | Dubbele of conflicterende identificatoren vereisen stamdatacorrectie vóór betrouwbare reconciliatie.                       |
| **Kostprijs per eenheid**                    | Moet in `Config_Master` bestaan voor financiële waardering.                                                         | Hoeveelheidsvariantie kan zichtbaar blijven, maar financiële blootstelling kan zonder kosten niet betrouwbaar worden gewaardeerd.                    |
| **Snapshot-afsnijmoment**             | Shopify-, WMS- en 3PL-data moeten hetzelfde tijdstip vertegenwoordigen.                                               | Verschillende tijdstempels kunnen valse variantie creëren en vereisen herexport of aanpassing.                                       |
| **Geïmporteerde brongegevens**         | Ruwe exports moeten consistent in de aangewezen importzones worden geplakt.                                  | Structurele of bronformaat-anomalieën moeten worden gecorrigeerd voordat de resulterende uitzonderingen worden geïnterpreteerd.                   |
| **Discrepantiedrempel**        | Hoeveelheids-/percentage drempels moeten in de configuratie worden bijgehouden in plaats van hardgecodeerd in individuele uitvoeren. | Uitzonderingen die de drempel overschrijden worden voor onderzoek gemarkeerd.                                                      |
| **3PL-tolerantie / SLA**          | Contractuele verlostolerantie moet worden meegewogen bij de beslissing of een uitzondering claim-waardig is.              | De werkmap levert het bewijs; het management bepaalt of een contractuele claim wordt gestart.                    |
| **Retourtiming**               | Retourzendingen die door een 3PL worden geregistreerd en terugbetalingen in Shopify kunnen op verschillende momenten plaatsvinden.                        | Kortetermijnverschillen mogen niet automatisch als permanente shrinkage worden geïnterpreteerd.                                     |
| **Historische SKU-naamgeving**        | Verouderde naamgevingsinconsistenties moeten worden genormaliseerd of gemapt.                                                    | Niet-gemapte historische SKU's moeten zichtbaar blijven als datakwaliteitsuitzonderingen.                                                |
| **Synchronisatievertraging van systemen** | Tijdelijke Shopify/3PL-synchronisatieproblemen vallen buiten de reconciliatielogica van de spreadsheet.               | Beschouw dit als een systeemintegratieprobleem in plaats van een VBA-werkoplossing te forceren.                               |

De bron onderscheidt expliciet tussen problemen die Excel kan oplossen en problemen die operationele of systeemniveau-interventie vereisen. Gestandaardiseerde reconciliatie, verlieswaardering en uitzonderingsdashboards horen in de werkmap; cyclustellingsdiscipline, 3PL-claimbeheer, API-synchronisatie en GPS-tracking niet.



### Wat deze werkmap niet probeert op te lossen

De architectuur handhaaft bewust een duidelijke grens rond de Excel-laag.

**Operationele beheersproblemen:**

* inconsistente 3PL-cyclustellingsprocedures;
* onvoldoende frequentie van fysieke voorraadtellingen;
* het niet starten van claims wanneer contractuele verlieslimieten worden overschreden.

Deze vereisen managementactie in plaats van nog een formule.

**Systeemintegratieproblemen:**

* realtime Shopify ↔ 3PL-synchronisatievertragingen;
* API-communicatie;
* geautomatiseerde ERP-integratie.

De bron raadt specifiek af deze problemen via VBA in een lichtgewicht Excel-werkmap te forceren.

**Transportzichtbaarheidsproblemen:**

* realtime GPS-tracking van voorraad in transit;
* transportbeheerworkflows.

Deze vereisen een dedicated TMS in plaats van een voorraadreconciliatiespreadsheet.

Deze grens is opzettelijk. Het doel van de werkmap is het bieden van een **herhaalbare reconciliatie- en financieel-verliesanalyselaag**, niet de pretentie dat elk voorraadbeheersprobleem een Excel-probleem is.

### De werkmap verkrijgen

De tool is ontworpen voor terugkerende reconciliatie in plaats van eenmalige spreadsheetanalyse.

De beoogde operationele cyclus is:

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

De bronblauwdruk specificeert een wekelijkse of maandelijkse cadans, waarbij gebruikers de drie bronexports in hun respectieve invoerbladen plakken en actuele SKU-kosten en waarschuwingsdrempels in `Config_Master` bijhouden.

**Browserversie:** gebruik de HTML-versie voor een snelle operationele beoordeling.

**Excel-versie:** gebruik de werkmap wanneer de reconciliatie moet worden vernieuwd met echte Shopify-, WMS- en 3PL-exports.

De tool is bewust ontworpen zodat een niet-technische operations- of finance-gebruiker de terugkerende reconciliatie kan voltooien zonder elke keer het analytische model te herbouwen. Het brondoel is circa **10 minuten** voor het opschonen, reconciliëren en beoordelen van uitzonderingen.

### Beperkingen

Deze werkmap is een **reconciliatie- en verliesanalyse-laag**, geen voorraadbeheersplatform.

Zij kan niet:

* realtime Shopify ↔ WMS ↔ 3PL-synchronisatie garanderen;
* voorkomen dat een magazijnmedewerker fysiek een artikel verzendt wanneer de voorraad ontoereikend is;
* een WMS, ERP of voorraadbeheersysteem vervangen;
* 3PL-cyclustellingsprocedures afdwingen;
* automatisch bepalen of een discrepancy contractueel verhaalbaar is;
* realtime GPS-tracking van voorraad in transit bieden;
* historische SKU-stamdataproblemen oplossen zonder een passende mappingbeslissing.

Deze grenzen zijn expliciet in het bronontwerp. Gestandaardiseerde reconciliatie, discrepantiewaardering, uitzonderingsrangschikking en dashboardrapportage worden als geschikte Excel-problemen beschouwd. Cyclustellingsdiscipline en 3PL-claimbeheer vereisen managementcontroles; realtime API-synchronisatie hoort bij systeemintegratie; fysieke verzendtracking hoort bij een TMS.

Er zijn ook belangrijke interpretatiebeperkingen.

**Een hoeveelheidsverschil is niet automatisch shrinkage.** Retourzendingen kunnen door een 3PL op een ander moment worden geregistreerd dan de bijbehorende Shopify-terugbetaling, en inconsistente snapshottiming kan tijdelijke verschillen creëren. De operator moet de zakelijke context valideren voordat een discrepancy als permanent verlies wordt geclassificeerd.

**Het financiële verliescijfer is een schatting, geen boekhoudpost.** Het hangt af van de geconfigureerde SKU-kostprijs en de interpretatie van de onderliggende hoeveelheidsverschillen.

**Een schoon spreadsheetresultaat garandeert geen schone brongegevens.** Historische SKU-naamgevingsinconsistenties, onvolledige exports, dubbele records of onjuiste fysieke tellingen kunnen nog steeds misleidende conclusies opleveren.

De werkmap moet daarom worden gebruikt als een **feitenvaststellings- en prioriteringsmechanisme**, niet als een automatische oordeelsmachine.

</details>


## Andere tools in deze serie

Een collectie lichtgewicht Excel beslissingsondersteunende tools die operationele beheersing, reconciliatie, winstgevendheid, voorraad en financiële analyse dekken.

* **[inventory-planning-reorder-point-excel](https://github.com/HyVoid/inventory-planning-reorder-point-excel)** — Welke inkoopbeslissing moet vandaag worden genomen gegeven vraagtrends levertijden en kasbeperkingen? — Prognose voorraadbehoeften door vraagsignalen, levertijdrisico, inkoopadviezen en werkkapitaalexposure te combineren.
* **[Retail-SKU-Concentration-Assortment-Diagnostic-Console](https://github.com/HyVoid/Retail-SKU-Concentration-Assortment-Diagnostic-Console)** — Welke producten domineren voorraadrisico of verwateren assortimentkwaliteit? — Identificeer SKU-concentratierisico en assortimentefficiëntie in retailproductcatalogi.
* **[Retail-and-Maquila-Inventory-Ledger](https://github.com/HyVoid/Retail-and-Maquila-Inventory-Ledger)** — Waar beweegt voorraad zich tussen retail- en maquilaoperaties? — Volg voorraadbewegingen, verwerkingsverliezen en voorraadexposure over fabrieken, magazijnen en winkels.
* **[Universal-3D-Cargo-Loading-Optimization-Simulator](https://github.com/HyVoid/Universal-3D-Cargo-Loading-Optimization-Simulator)** — Hoe moet cargo worden geladen om verspilde ruimte en operationele wrijving te verminderen? — Simuleer 3D-laadconfiguraties om contain capaciteit en verzendefficiëntie te maximaliseren.
* **[Cross-Border-DTC-Inventory-Governance-Console](https://github.com/HyVoid/Cross-Border-DTC-Inventory-Governance-Console)** — Wat is de echte inkoopvraag na aftrek van pre-order verplichtingen en verwachte retouren? — Reconstrueer echte vraagsignalen door pre-order verplichtingen en retourgedrag te isoleren van ruwe verkoopdata.
* **[inventory-allocation-fulfillment-excel](https://github.com/HyVoid/inventory-allocation-fulfillment-excel)** — Kan elke klantorder daadwerkelijk op tijd worden geleverd gegeven fysieke voorraad, reserveringen, containers in transit en openstaande PO's op al onze locaties? — Bereken beschikbare-tot-te-beloven hoeveelheden en netto inkoopbehoeften door fysieke voorraad, orderreserveringen, voorraad in transit en open inkooporders over meerdere locaties te reconciliëren.

## Licentie

Dit project wordt uitgegeven onder de **Apache-licentie 2.0**.

Je mag het project gebruiken, wijzigen, distribueren en aanpassen onder de voorwaarden van de Apache-licentie 2.0.

Zie het licentiebestand in de repository voor de volledige licentietekst.

