[ 🌐 عربي ](README.ar.md) | [ 🇩🇪 Deutsch ](README.de.md) | [ 🇫🇷 Français ](README.fr.md) | [ 🇳🇱 Nederlands ](README.nl.md) | [ 🇪🇸 Español ](README.sp.md) | [ 🇬🇧 English ](README.md)

# Multi-Node Inventory Reconciliation & Shrinkage Analysis | Shopify & 3PL Excel-sjabloon
<img width="1920" height="790" alt="image" src="https://github.com/user-attachments/assets/6689bffe-1aac-43d7-9f63-6e85a14470f0" />


[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](#licentie)
[![Platform: Browser + Excel](https://img.shields.io/badge/Platform-Browser%20%2B%20Excel-217346.svg)](#korte-handleiding-hoe-je-je-voorraadreconciliatie-automatiseert)
[![Tool Type: Decision Support](https://img.shields.io/badge/Tool%20Type-Decision%20Support-2251FF.svg)](#wat-het-je-laat-volgen-voorraadpijnpunten-vs-oplossingen)

**Een geautomatiseerde reconciliatiespreadsheet en sjabloon voor shrinkage-analyse, ontworpen voor multichannel e-commerce merken. Vergelijk direct de Shopify-voorraadniveaus, de registraties van je interne Warehouse Management System (WMS) en de fysieke tellingen van je Third-Party Logistics (3PL)-partner om discrepanties te lokaliseren en eenheidsverlies te vertalen naar directe financiële impact, zonder VLOOKUP-formules te schrijven of elke maand rapporten opnieuw te bouwen.**

**Geen registratie. Geen installatie. Gratis in je browser.**

Test je operationele data direct in de gratis browserversie. Voor terugkerende maandafsluitingen en offline gegevensbeveiliging upgrade je naar het volledig ontgrendelde Excel-sjabloon met een 30-daagse geld-terug-garantie zonder vragen.

> 🌐 **Open het interactieve dashboard**  
> [Probeer de gratis browsergebaseerde 3PL voorraadreconciliatie-simulator](https://hyvoid.github.io/MULTI-NODE-INVENTORY-RECONCILIATION/)
> 
> 📥 **Download de herbruikbare spreadsheet**  
> [Download het voorraadshrinkage- & audit Excel-sjabloon](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)

---

## Wat het je laat volgen: Voorraadpijnpunten vs. Oplossingen

In plaats van slechts te constateren dat "de cijfers niet kloppen", vertaalt deze toolkit ruime voorraadverschillen naar een financieel actieplan.

| E-commerce voorraadpijnpunt (Het "waarom") | Reconcilieoplossing (Het "hoe") |
| :--- | :--- |
| **Blind spots tussen systemen:** Niet weten welk systeem (Shopify vs. 3PL vs. WMS) de waarheid over de beschikbare voorraad bewaart. | **Multi-node triangulatie:** Legt de door systemen gerapporteerde hoeveelheden naast elkaar om precies te lokaliseren waar datasynchronisaties mislukken. |
| **Ongekwantificeerde financiële shrinkage:** Een afwijking van 20 stuks op een artikel van $5 gelijk behandelen aan die van een artikel van $50. | **COGS-gewogen variantieanalyse:** Vermenigvuldigt eenheidsdiscrepanties met de SKU-kostprijs om de werkelijke financiële afboekingsblootstelling te onthullen. |
| **Leckage bij derde-partij-logistiek (3PL):** Het vermoeden dat fulfillmentpartners voorraad verliezen, zonder hard bewijs voor SLA-claims. | **Volgen van discrepantietarieven:** Isoleert de variantietarieven van 3PL versus intern magazijn om een feitelijke basis op te bouwen voor contractuele verliesclaims. |
| **Analyseparalyse door ruwe data:** Duizenden rijen cyclustelling-spreadsheets doorscrollen om fouten te vinden. | **Uitzonderingsgestuurd dashboarden:** Rangschikt automatisch de "Top 10 SKU's naar verlieswaarde" om managementonderzoek te prioriteren. |

---

## Korte handleiding: Hoe je je voorraadreconciliatie automatiseert

Transformeer rommelige, multi-bron exports in een executive voorraadaudit in vier gestructureerde stappen.

### Stap 1: Configureer je SKU-stamgegevens (eenmalige setup)
Ga naar het `Config_Master`-werkblad. Definieer je standaard SKU-nomenclatuur, de kostprijs per eenheid (COGS) en de bedrijfsspecifieke waarschuwingsdrempels (bijv. markeer elke discrepantie > 5 stuks of > $100 waarde). Deze baseline zorgt ervoor dat alle inkomende data wordt gemeten tegen één enkele bron van waarheid.

### Stap 2: Importeer WMS-, 3PL- en Shopify-exports
Omzeil handmatige datanormalisatie. Plak je ruwe CSV-exports direct in de aangewezen tabbladen:
*   `Import_Shopify` (De beschikbaarheid van je webwinkel)
*   `Import_WMS` (De registraties van je interne magazijn)
*   `Import_3PL` (De fysieke tellingen van je externe fulfillmentpartner)
*Opmerking: Het systeem is ontworpen om ruwe exports direct te verwerken, zonder handmatig kolommen te verwijderen of te herbouwen.*

### Stap 3: Genereer het shrinkage-dashboard en bekijk de uitzonderingen
Ga naar de `Dashboard`-uitvoer. De geautomatiseerde reconciliatie-engine schoont direct de opmaak op, stemt SKU's af en berekent discrepanties. Bekijk je voorraadafwijkingen met de hoogste waarde, de totale shrinkage en de nauwkeurigheidstarieven per node zonder handmatig één enkele cel te berekenen.

### Stap 4: Bouw een routine op en download voor herhaald gebruik
Gebruik voor je eerste audit de browserversie om directe voorraadproblemen te identificeren. Om een robuuste maandelijkse voorraadbeheersritme op te bouwen, exporteer je het systeem voor langetermijngebruik.

👉 **Actie vereist:** Zodra je workflow is gevalideerd, **[download je hier de herbruikbare voorraadreconciliatie Excel-sjabloon](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)**. Volgende maand plak je simpelweg de nieuwe voorraadsnapshot over de oude data; de volledige variantieanalyse wordt automatisch vernieuwd.

---

## De bedrijfslogica & methodiek

Deze toolkit is ontworpen rond professionele auditprincipes en verschuift de focus van data-aggregatie naar proactieve activabescherming. Dit is de operationele methodiek die de werkmap aandrijft:

### 1. Methodiek: Drievoudige voorraadafstemming
*   **De methode:** Vergelijkbaar met financiële audits van schulden aan leveranciers (AP), hanteert dit raamwerk een **drievoudig afstemmingsprincipe** tussen digitale verkoop (Shopify), interne tracking (WMS) en fysieke opslag (3PL).
*   **De zakelijke impact:** Het stopt het «schuldenspel». Door data te trianguleren kunnen operations managers vaststellen of een probleem een storefront-synchronisatiefout is (API-vertraging) of een fysiek fulfilmentverlies (shrinkage), wat de oplostijd drastisch verkort.

### 2. Methodiek: Prioritering op financieel waarde-at-risk (VaR)
*   **De methode:** Discrepanties worden inherent gewogen op basis van de kosten van verkochte goederen (COGS). De rekenlaag transformeert `Stuksafwijking` in `Financiële afboekingsblootstelling`.
*   **De zakelijke impact:** Het optimaliseert de arbeidsallocatie. In plaats van dat magazijnmedewerkers 4 uur besteden aan het onderzoeken van een afwijking van 50 stuks in poly-mailers, stuurt het dashboard ze naar een afwijking van 3 stuks in elektronica met hoge marge.

### 3. Methodiek: Uitzonderingsgestuurde rapportage
*   **De methode:** De toolkit filtert duizenden matchende SKU's naar een gecondenseerde lijst operationele uitzonderingen op basis van door de gebruiker gedefinieerde tolerantiedrempels (bijv. acceptabele shrinkage < 0,5%).
*   **De zakelijke impact:** Het creëert **geproduceerd redeneren**. De supply chain-directeur kijkt niet naar een datastort; hij kijkt naar een actiebare takenlijst voor interne procescorrectie of het indienen van 3PL-claims.

---

## Scenario's uit de praktijk: Wanneer gebruik je dit voorraadaudit-sjabloon

Dit systeem is specifiek gebouwd voor kritieke knooppunten in de supply chain waar fysieke voorraadnauwkeurigheid de financiële gezondheid bepaalt.

*   **Scenario A: Financiële maandafsluiting.** Financeteams hebben een exact COGS-afboekingscijfer nodig voor de boekhouding. Gebruik dit sjabloon om de exacte dollarwaarde van verloren voorraad over alle magazijnen op de laatste dag van de maand te berekenen.
*   **Scenario B: 3PL SLA-contractgeschillen.** Je vermoedt dat je fulfilmentpartner merchandising verliest boven de shrinkage-tolerantie van 1,5%. Gebruik de multi-node vergelijking om een gedocumenteerd claimrapport te genereren voor ontbrekende high-ticket SKU's.
*   **Scenario C: Voorkomen van voorraaduitval in het hoogseizoen (Q4/Black Friday).** Shopify toont 100 stuks, maar de 3PL heeft er slechts 20. Voer deze reconciliatie wekelijks uit tijdens Q4 om «spookvoorraad» te vangen voordat klanten voorraad kopen die je fysiek niet bezit; zo voorkom je massale restituties en supporttickets.

---

## Veelvoorkomende problemen in voorraadoperaties die dit oplost

| Probleem in voorraadoperaties | Handmatig spreadsheetproces | Geautomatiseerde sjabloonoplossing |
| :--- | :--- | :--- |
| **Drie uiteenlopende systemen zijn het oneens** | Operator draait handmatig `INDEX/MATCH` over Shopify-, WMS- en 3PL-bestanden, met risico op kapotte verwijzingen. | Een gestandaardiseerde reconciliatielaag stemt alle stock keeping units (SKU's) automatisch af. |
| **Rommlige opmaak van geëxporteerde data** | Lege rijen, spaties aan het einde en hoofdlettergevoelige SKU's veroorzaken valse mismatch-fouten. | De rekenlaag normaliseert strings en datatypen vóór de variantiecontrole. |
| **Shrinkage wordt alleen in stuks gemeten** | Het management ziet een stukstekort maar kan de COGS-impact niet nauwkeurig inschatten. | De ingebouwde SKU-kostenmatrix zet hoeveelheidstekorten om in geschatte financiële afboekingen. |
| **Grote uitzonderingen verdwijnen in het detail** | Controllers scannen duizenden rijen en missen commercieel fatale voorraaddiscrepanties. | Het executive dashboard belicht 3PL-fouttarieven, dode voorraad en de top 10 artikelen met verlieswaarde. |
| **3PL-verliezen zijn moeilijk te onderbouwen** | Ontbrekende voorraad blijft een informele magazijnklacht zonder documentatie. | Genereert een feitelijke variantieledger ter ondersteuning van formele 3PL SLA-claims en terugbetalingen. |

---

## Voor wie is dit: Rollen & use cases

Deze tool overbrugt de kloof tussen fysieke magazijnvoering en financiële rapportage. Hij is doelbewust ontworpen voor:

*   **E-commerce operations managers** die een *Shopify voorraadreconciliatiesjabloon* nodig hebben om digitale storefronts te synchroniseren met fysieke fulfilmentcentra.
*   **Supply chain-directeuren** die een *alternatief voor 3PL-auditsoftware* zoeken om externe partners verantwoordelijk te houden voor contractuele shrinkagetarieven.
*   **Voorraadcontrollers & magazijnmanagers** die maandelijkse *cyclustellingreconciliaties* uitvoeren over meerdere interne nodes.
*   **Fractionele CFO's & financiële managers** die een nauwkeurige methode nodig hebben om *voorraadshrinkage en COGS-impact* te berekenen voor maandafsluitingen.
*   **DTC-oprichters** die een executive overzicht van de voorraadgezondheid willen zonder te investeren in complexe ERP-integraties van zes cijfers.

*Opmerking: Deze toolkit is **niet** ontworpen om realtime API's, ERP-systemen of live WMS-barcodescanning te vervangen. Het is een periodiek beslissingsondersteuningsraamwerk dat gebruikt wordt om die systemen te auditen.*

---

## Over de maker

Ik bouw lichtgewicht operationele trackers en beslissingsondersteunende tools voor situaties waarin te veel bewegende delen zijn om in je hoofd te houden, maar te weinig complexiteit om nog een enterprisesysteem te rechtvaardigen.

De centrale vraag is eenvoudig: **Welke informatie moet op één gecentraliseerde plek staan voordat de volgende strategische supply chain-beslissing met vertrouwen genomen kan worden?**

Deze Multi-Node Inventory Reconciliation-werkmap is één voorbeeld van die aanpak: terugkerende systeemoverstijgende voorraadvergelijkingen omzetten in een gestandaardiseerde analytische workflow die operationele discrepanties verbindt met financiële gevolgen.


## Technische details

<details>
<summary>Voor technische reviewers, Excel-beoefenaars en medewerkers</summary>

### Werkmaparchitectuur

De werkmap is bewust gestructureerd als een **data-schoonmaak- en reconciliatie-engine + beslissingsdashboard voor financieel verlies**, en niet als een permanente voorraaddatabase. Elke reconciliecyclus kan de vorige importset overschrijven of als aparte werkmap worden opgeslagen, waardoor het bestand lichtgewicht blijft en onnodige database- of macro-afhankelijkheden worden vermeden.

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
| `Dashboard`      | Beslissing    | KPI-samenvatting, verliesblootstelling, nodevergelijking, Top 10 uitzonderingen | CEO / Management        |
| `Config_Master`  | Configuratie  | Standaard SKU-lijst, productinformatie, kostprijs, discrepantiedrempels   | Operations / Finance    |
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

niet een valse uitzondering mag worden simpelweg omdat een andere export bevat:

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
* 3PL-discrepantietarief
* Intern magazijn-discrepantietarief

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

Een discrepantie mag pas als financieel verlies worden geïnterpreteerd wanneer de vergelijkingsbasis zelf geldig is.

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
| Shopify |    1.000 |
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

De volgende actie is niet om elke SKU gelijk te inspecteren. De operator moet eerst de **3PL-zijuitzondering onderzoeken**, verifiëren of de variantie fysiek verlies, schade, timing of een rapportageprobleem vertegenwoordigt, en vervolgens bepalen of de discrepantie de contractuele of interne tolerantie van het bedrijf overschrijdt.

Het dashboard is ontworpen om deze prioritering zichtbaar te maken: het management kan de totale financiële blootstelling, de verliesverdeling tussen nodes en de SKU-uitzonderingen met de hoogste waarde zien zonder handmatig de ruwe exports te doorzoeken.

De tool ondersteunt daarom een reeks van:

**reconciliatie → uitzonderingsisolatie → financiële kwantificering → operationeel onderzoek → mogelijke claim of procescorrectie.**

De tool zelf bepaalt niet of een discrepantie juridisch verhaalbaar is. Dat blijft een management- en contractbeslissing.

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

Het resulterende tarief kan worden vergeleken met de geconfigureerde waarschuwings- of tolerantiedrempel.

Het bronontwerp voorziet dat `Config_Master` de discrepantiedrempels bijhoudt en dat voorwaardelijke opmaak rijen markeert waarvan de hoeveelheid of het discrepantietarief de geconfigureerde limiet overschrijdt.

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
| **Discrepantiedrempel**        | Hoeveelheids-/tariefdrempels moeten in de configuratie worden bijgehouden in plaats van hardgecodeerd in individuele uitvoeren. | Uitzonderingen die de drempel overschrijden worden voor onderzoek gemarkeerd.                                                      |
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
* automatisch bepalen of een discrepantie contractueel verhaalbaar is;
* realtime GPS-tracking van voorraad in transit bieden;
* historische SKU-stamdataproblemen oplossen zonder een passende mappingbeslissing.

Deze grenzen zijn expliciet in het bronontwerp. Gestandaardiseerde reconciliatie, discrepantiewaardering, uitzonderingsrangschikking en dashboardrapportage worden als geschikte Excel-problemen beschouwd. Cyclustellingsdiscipline en 3PL-claimbeheer vereisen managementcontroles; realtime API-synchronisatie hoort bij systeemintegratie; fysieke verzendtracking hoort bij een TMS.

Er zijn ook belangrijke interpretatiebeperkingen.

**Een hoeveelheidsverschil is niet automatisch shrinkage.** Retourzendingen kunnen door een 3PL op een ander moment worden geregistreerd dan de bijbehorende Shopify-terugbetaling, en inconsistente snapshottiming kan tijdelijke verschillen creëren. De operator moet de zakelijke context valideren voordat een discrepantie als permanent verlies wordt geclassificeerd.

**Het financiële verliescijfer is een schatting, geen boekhoudpost.** Het hangt af van de geconfigureerde SKU-kostprijs en de interpretatie van de onderliggende hoeveelheidsverschillen.

**Een schoon spreadsheetresultaat garandeert geen schone brongegevens.** Historische SKU-naamgevingsinconsistenties, onvolledige exports, dubbele records of onjuiste fysieke tellingen kunnen nog steeds misleidende conclusies opleveren.

De werkmap moet daarom worden gebruikt als een **feitenvaststellings- en prioriteringsmechanisme**, niet als een automatische oordeelsmachine.

</details>


## Andere tools in deze serie

Een collectie lichtgewicht Excel beslissingsondersteunende tools die operationele beheersing, reconciliatie, winstgevendheid, voorraad en financiële analyse dekken.

* **Inventory Planning & Reorder Control** — vraag, aanvulling, voorraadblootstelling en inkoopbeslissingen.
* **Order-Level Profit Engine** — omzet, variabele kosten, verzendallocatie en winstgevendheid per order.
* **Single-Project Construction Control** — projectbudget, verbintenissen, projectkosten en projectwinstgevendheid.
* **Contractor Operations & Profitability Management System** — Lead → Offerte → Project → Arbeid & Materialen → Projectkosten → Winst → Klantgeschiedenis workflow.

## Licentie

Dit project wordt uitgegeven onder de **Apache-licentie 2.0**.

Je mag het project gebruiken, wijzigen, distribueren en aanpassen onder de voorwaarden van de Apache-licentie 2.0.

Zie het licentiebestand in de repository voor de volledige licentietekst.
