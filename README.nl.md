[ 🌐 عربي ](README.ar.md) | [ 🇩🇪 Deutsch ](README.de.md) | [ 🇳🇱 Nederlands ](README.nl.md) | [ 🇪🇸 Español ](README.sp.md) | [ 🇬🇧 English ](README.md)

# Stop met het uitleggen van voorraadverlies. Begin het te lokaliseren.
# Voorraadaansluiting over meerdere vestigingen en analyse van voorraadverlies

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](#license)
[![Platform: Browser + Excel](https://img.shields.io/badge/Platform-Browser%20%2B%20Excel-217346.svg)](#quick-start-workflow)
[![Tool Type: Decision Support](https://img.shields.io/badge/Tool%20Type-Decision%20Support-2251FF.svg)](#what-it-helps-you-track)

**Een lichtgewicht tool voor voorraadaansluiting en analyse van voorraadverlies, waarmee u de voorraad van Shopify, WMS en 3PL kunt vergelijken, afwijkingen kunt lokaliseren en voorraadverlies kunt omzetten in financiële impact—zonder de analyse elke rapportagecyclus opnieuw op te bouwen.**

**Geen aanmelding. Geen installatie. Gratis in uw browser.**

Probeer de browserversie gratis. Hebt u de Excel-versie nodig, dan kunt u die kopen met een niet-goed-geld-terug-garantie van 30 dagen.
>
> 🌐 **[Openen in de browser](https://hyvoid.github.io/MULTI-NODE-INVENTORY-RECONCILIATION/)** — HTML live versie
> 📥 **[Excel downloaden](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)** — Excel-versie

## Wat u hiermee kunt bijhouden

* **Verschillen tussen Shopify, WMS en 3PL** — zie waar de door systemen gerapporteerde hoeveelheden niet meer overeenkomen.
* **Totale voorraadafwijking en geschatte waarde van voorraadverlies** — begrijp de financiële consequentie in plaats van alleen naar hoeveelheidsverschillen te kijken.
* **Afwijkingspercentages van 3PL versus intern magazijn** — onderscheid waar het grootste aansluitingsprobleem geconcentreerd is.
* **SKU's met de hoogste verlieswaarde** — identificeer welke producten eerst onderzoek verdienen.
* **Uitzonderingen met hoog risico** — maak SKU's zichtbaar waarvan de hoeveelheid of het afwijkingspercentage de geconfigureerde waarschuwingsdrempel overschrijdt.
* **Potentiële blootstelling voor claims op de 3PL** — lever een feitelijke basis voor correctie van interne processen of contractuele claims wegens verlies.

## Snelstartworkflow

1. **Stel de belangrijkste parameters in.**
   Onderhoud op `Config_Master` de standaard-SKU-lijst, productinformatie, kostprijs per eenheid en de afwijkings- of waarschuwingsdrempels die het bedrijf gebruikt.

2. **Importeer bestaande gegevens.**
   Plak de nieuwste Shopify-export in `Import_Shopify`, de WMS-voorraadexport in `Import_WMS` en de fysieke 3PL-voorraadexport in `Import_3PL`. De bedoelde workflow is om de oorspronkelijke exports rechtstreeks te gebruiken in plaats van handmatig een genormaliseerde aansluitingstabel opnieuw op te bouwen.

3. **Haal de resultaten op.**
   Ga naar de aansluitingsuitvoer en het `Dashboard`. De werkmap schoont de geïmporteerde records op, lijnt ze uit, vergelijkt voorraadhoeveelheden tussen de vestigingen, berekent afwijkingen en zet relevante verschillen om in financiële waarden.

4. **Onderhoud met periodieke verversing.**
   Herhaal het proces wekelijks of maandelijks met een consistent afsluitmoment voor de voorraad. De werkmap is bewust lichtgewicht: ververs de brongegevens in plaats van de analyse opnieuw op te bouwen.

**Stel de besturingsparameters in. Laad de bestaande voorraadexports. Haal de aansluiting op. Onderzoek de uitzonderingen. Ververs wanneer nodig.**

## Waarom ik dit heb gebouwd

Problemen met voorraad over meerdere vestigingen worden zelden veroorzaakt door het ontbreken van een getal. Ze worden veroorzaakt doordat **verschillende systemen verschillende versies van hetzelfde getal presenteren**.

Een Shopify-voorraadexport kan beschrijven wat het verkoopsysteem denkt dat beschikbaar is. Een WMS-export kan beschrijven wat het interne magazijn als op voorraad geregistreerd heeft. Een 3PL-rapport kan de fysieke voorraad bij een externe fulfilmentlocatie beschrijven. Wanneer deze bestanden wekelijks handmatig worden samengevoegd, wordt het aansluitingsproces zelf een extra bron van fouten.

De fout is extra kostbaar omdat een afwijking meestal als een hoeveelheidsprobleem wordt behandeld:

> "SKU A komt 18 eenheden tekort."

Die uitspraak beantwoordt de managementvraag niet.

De nuttige vraag is:

> **Waar zijn die 18 eenheden verdwenen, en wat betekent dat verschil financieel?**

Deze tool verandert de aansluiting in een herhaalbare analytische workflow. In plaats van drie spreadsheets handmatig te vergelijken, stelt de gebruiker een standaard SKU-referentie vast, importeert de drie voorraadmomentopnamen en laat de werkmap de records uitlijnen en de verschillen berekenen.

Een afwijking van 20 eenheden op een artikel van $3 en een afwijking van 20 eenheden op een artikel van $45 zouden bijvoorbeeld niet dezelfde managementprioriteit moeten krijgen. Het introduceren van de SKU-kostenmatrix zet hoeveelheidsafwijking om in een geschatte financiële blootstelling. Het dashboard kan vervolgens de afwijkingen met de hoogste waarde rangschikken, in plaats van de medewerker elke regel handmatig te laten inspecteren.

Het resultaat is **geproductiseerd redeneren**: een herbruikbaar kader om elke week of maand dezelfde operationele vraag te beantwoorden, in plaats van een eenmalig spreadsheet rond één aansluitingsgebeurtenis.

## Veelvoorkomende aansluitingsproblemen die dit oplost

| Probleem                                      | Zonder deze tool                                                                                                  | Met deze tool                                                                                                   |
| -------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------- |
| **Drie systemen komen niet overeen**                   | Shopify-, WMS- en 3PL-exports worden handmatig vergeleken, met meer risico op gemiste regels en inconsistente koppelingen. | Een gestandaardiseerde aansluitingslaag lijnt records uit rond de geconfigureerde SKU-referentie.                          |
| **Rommelige exportgegevens**                      | Lege regels, inconsistente opmaak, spaties en hoofdlettergebruik veroorzaken valse afwijkingen.                           | De berekeningslaag normaliseert de belangrijkste velden voordat wordt vergeleken.                                                   |
| **Afwijking wordt alleen in eenheden gemeten**       | Het management ziet een voorraadverschil maar kan de financiële betekenis niet direct inschatten.                     | De kostprijs per SKU zet relevante hoeveelheidsverschillen om in een geschatte verlieswaarde.                                  |
| **Grote uitzonderingen verdwijnen in details**    | Medewerkers doorlopen lange aansluitingstabellen en kunnen commercieel belangrijke afwijkingen missen.                     | De dashboarduitvoer markeert afwijkingspercentages, verlieswaarde en de top 10 SKU's met hoge waarde.                           |
| **3PL-verliezen zijn moeilijk te onderbouwen** | Een vermoedelijk verlies blijft misschien een informele operationele klacht.                                                     | Een gestandaardiseerd aansluitingsrapport biedt een feitelijke basis voor onderzoek en mogelijke claimvoorbereiding. |
| **Aansluiting vindt te laat plaats**          | De voorraad wordt reactief herzien nadat afwijkingen zich hebben opgestapeld.                                             | Een wekelijkse of maandelijkse controlefrequentie ondersteunt proactieve aansluiting en opvolging van uitzonderingen.                   |

## Voor wie dit bedoeld is

Deze tool is ontworpen voor **e-commerce- en retailexploitanten, supply-chainmanagers, finance-teams, voorraadcontrollers en bedrijfseigenaren** die voorraadgegevens van meerdere operationele vestigingen ontvangen en een herhaalbare manier nodig hebben om die aan te sluiten zonder een volledig ERP of een custom integratieproject in te voeren.

De tool is bijzonder geschikt voor bedrijven waar Shopify, een intern WMS en een of meer 3PL-voorraadrapporten op terugkerende basis moeten worden vergeleken.

De tool is **niet** bedoeld om een ERP, WMS, TMS of realtime API-integratie te vervangen. Ze biedt geen GPS-tracking, voorkomt geen fysieke oververkoop op het moment van de transactie en lost geen momentane vertragingen in systeemsynchronisatie op. Dat zijn problemen van systeemintegratie of operationele beheersing, niet van spreadsheet-aansluiting.

**Er is geen spreadsheetkennis nodig om de browserversie te begrijpen. Open deze, bekijk de workflow en bepaal of het aansluitingsmodel bij het operationele proces past.**

## Over

Ik bouw lichtgewicht operationele trackers en tools voor besluitvormingsondersteuning in situaties waarin te veel bewegende delen zijn om in uw hoofd te houden, maar niet genoeg complexiteit om een extra enterprise-systeem te rechtvaardigen.

De centrale vraag is eenvoudig: **Welke informatie moet op één plek staan zodat de volgende operationele beslissing met vertrouwen kan worden genomen?**

Voorraadaansluiting over meerdere vestigingen en analyse van voorraadverlies is een voorbeeld van die aanpak: verander terugkerende voorraadvergelijking tussen systemen in een gestandaardiseerde analytische workflow die operationele afwijkingen verbindt met financiële consequenties.
## Technische details

<details>
<summary>Voor technische reviewers, Excel-professionals en medewerkers</summary>

### Architectuur van de werkmap

De werkmap is bewust opgebouwd als een **engine voor gegevensopschoning en aansluiting + dashboard voor besluitvorming over financieel verlies**, in plaats van als een permanente voorraaddatabase. Elke aansluitingscyclus kan de vorige importset overschrijven of als een aparte werkmap worden opgeslagen, waardoor het bestand lichtgewicht blijft en onnodige database- of macro-afhankelijkheden worden vermeden.

De architectuur volgt een eenvoudige reeks:

**Invoer → Normaliseren → Aansluiten → Kwantificeren → Markeren → Presenteren**

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

De werkmap is verdeeld in zes functionele bladen:

| Blad            | Laag         | Verantwoordelijkheid                                                            | Primaire gebruiker           |
| ---------------- | ------------- | ------------------------------------------------------------------------- | ---------------------- |
| `Dashboard`      | Beslissing      | KPI-overzicht, verliesblootstelling, vergelijking tussen vestigingen, top 10 uitzonderingen            | CEO / management       |
| `Config_Master`  | Configuratie | Standaard-SKU-lijst, productinformatie, kostprijs per eenheid, afwijkingsdrempels | Operaties / finance   |
| `Import_Shopify` | Invoer         | Ruwe Shopify-voorraadexport                                              | Operaties             |
| `Import_WMS`     | Invoer         | Ruwe interne WMS-voorraadexport                                         | Magazijn / operaties |
| `Import_3PL`     | Invoer         | Ruwe fysieke 3PL-voorraadexport                                         | 3PL / operaties       |
| `Calc_Engine`    | Berekening   | Normalisatie van gegevens, SKU-koppeling, afwijkingsberekeningen, financiële impact | Verborgen technische laag |

De drie importbladen zijn bewust **plakzones**. De bronspecificatie staat gebruikers toe de oorspronkelijke exports rechtstreeks te plakken, inclusief compatibiliteit met voorloopregels, in plaats van hen te dwingen de bestanden handmatig om te vormen voordat ze worden aangesloten.

### Gegevensstroom en aansluitingslogica

De kernberekeningslaag gebruikt `Config_Master` als referentiepunt voor gestandaardiseerde SKU's.

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

Het ontwerp pakt specifiek het probleem van **rommelige gegevens** aan. De bronarchitectuur schrijft `TRIM()` voor om verborgen of per ongeluk toegevoegde spaties te verwijderen en `UPPER()` om het gebruik van hoofdletters te normaliseren, gevolgd door `XLOOKUP` of `INDEX + MATCH` voor niet-invasieve gegevensopvraging tussen tabellen.

Dit is belangrijk omdat een SKU zoals:

```text
ABC-001
```

geen valse uitzondering mag worden alleen omdat een andere export het volgende bevat:

```text
 abc-001
```

De aansluitingsengine behandelt normalisatie daarom als een voorwaarde voor vergelijking, in plaats van problemen met gegevenskwaliteit op te lossen nadat het afwijkingsrapport al is gegenereerd.

### Principe van het afsluitmoment voor de aansluiting

Voorraadmomentopnamen moeten het **zelfde zakelijke afsluitmoment** vertegenwoordigen.

Bijvoorbeeld:

```text
Shopify Snapshot     → Sunday 23:59:59
WMS Snapshot         → Sunday 23:59:59
3PL Physical Count   → Sunday 23:59:59
```

Als de momentopnamen op wezenlijk verschillende momenten worden genomen, kunnen voorraadbewegingen, retouren of zendingen onderweg schijnbare verschillen veroorzaken die geen werkelijke voorraadverliezen zijn.

De bronarchitectuur identificeert een consistent afsluitmoment expliciet als een kernbeperking van de operatie en waarschuwt dat niet-overeenkomende momentopnamen "valse verschillen" kunnen veroorzaken.

Dit is dus een **vereiste voor bedrijfsbeheersing**, niet alleen een vereiste voor een spreadsheetformule.

### SKU als de enige aansluitingssleutel

De SKU wordt behandeld als de standaardidentiteit die de drie bronsystemen met elkaar verbindt.

De configuratielaag onderhoudt:

* Standaard-SKU
* Productnaam
* Kostprijs per eenheid
* Afwijkingsdrempel
* Waarschuwingsdrempel

De rekenengine gebruikt die standaardsleutel vervolgens om hoeveelheden uit elke bron op te halen.

Dit voorkomt dat de aansluiting afhankelijk is van de regelvolgorde van de geïmporteerde bestanden. Shopify kan SKU's in de ene volgorde vermelden, WMS in een andere en 3PL in een derde; de rekenengine vergelijkt nog steeds hetzelfde product met hetzelfde product.

De bronspecificatie benadrukt de uniciteit en consistentie van SKU's als fundamentele beperking: één fysiek product mag niet door meerdere inconsistente identificaties worden vertegenwoordigd.

### Architectuur van het dashboard

Het dashboard is bewust ontworpen voor **management op basis van uitzonderingen**, niet voor het reproduceren van de ruwe brontabellen.

De primaire KPI-laag bevat:

* Totale hoeveelheidsafwijking
* Totaal geschat financieel verlies
* Afwijkingspercentage van de 3PL
* Afwijkingspercentage van het interne magazijn

De visuele laag biedt vervolgens:

* Verdeling van de verlieswaarde tussen 3PL en intern magazijn
* Top 10 SKU's gerangschikt op verlieswaarde
* Identificatie van uitzonderingen met hoog risico

Deze uitvoer is rechtstreeks gespecificeerd in de bronarchitectuur.

De bedoelde managementreeks is:

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

Daarom kan de werkmap beter worden begrepen als een **laag voor besluitvormingsondersteuning** dan als een eenvoudig spreadsheet voor voorraadvergelijking.

### Drie valkuilen die zelfs ervaren voorraadmedewerkers treffen

#### Valkuil 1 — Elk hoeveelheidsverschil als voorraadverlies behandelen

**Beslissing:**
Een medewerker ziet dat Shopify 1.000 eenheden rapporteert terwijl de 3PL 970 rapporteert, en registreert onmiddellijk 30 eenheden als verloren.

**Foutief getal:**
De vergelijking gebruikt momentopnamen die op verschillende tijdstippen zijn genomen.

**Waarom de aanbeveling verandert:**
Het verschil van 30 eenheden kan zendingen, retouren, correcties of andere bewegingen vertegenwoordigen die zich tussen de twee momentopnamen hebben voorgedaan.

**Correcte aanpak:**
Stel eerst een gemeenschappelijk afsluitmoment vast en vergelijk vergelijkbare voorraadmomentopnamen.

| Aanpak                 | Resultaat                                             |
| ------------------------ | -------------------------------------------------- |
| Verschillende momentopnametijden | Verschil van 30 eenheden behandeld als verlies                 |
| Gemeenschappelijk afsluitmoment           | Alleen het resterende onverklaarde verschil wordt onderzocht |

De bron identificeert inconsistentie in het afsluitmoment specifiek als oorzaak van valse afwijkingen.

De gecorrigeerde beslissing is daarom **"onderzoek de resterende afwijking"**, niet **"claim de volledige afwijking als voorraadverlies."**

<details>
<summary>Berekeningslogica</summary>

```text
Comparable Variance
= Quantity at Node A
- Quantity at Node B

Only when:
Snapshot_A_Time = Snapshot_B_Time
```

Een afwijking mag niet als financieel verlies worden geïnterpreteerd voordat de vergelijkingsbasis zelf geldig is.

</details>

#### Valkuil 2 — Problemen rangschikken op eenheden in plaats van op geld

**Beslissing:**
De medewerker sorteert het aansluitingsrapport op de grootste hoeveelheidsafwijking.

**Foutief cijfer:**
Een afwijking van 50 eenheden wordt boven een afwijking van 10 eenheden gerangschikt, simpelweg omdat `50 > 10`.

**Waarom de aanbeveling onvolledig is:**
Hoeveelheid vertegenwoordigt geen economische betekenis.

Stel:

| SKU   | Afwijking | Kostprijs per eenheid | Geschatte blootstelling |
| ----- | -------: | --------: | -----------------: |
| SKU-A |       50 |        $2 |               $100 |
| SKU-B |       10 |       $40 |               $400 |

Een rangschikking op alleen hoeveelheid zou SKU-A eerst onderzoeken. Een rangschikking op financieel verlies zou SKU-B eerst onderzoeken.

De bronarchitectuur vraagt expliciet om het introduceren van een SKU-kostenmatrix, zodat hoeveelheidsverschillen kunnen worden omgezet in financieel verlies.

**Correcte beslissing:** prioriteer uitzonderingen op basis van zowel **hoeveelheidsafwijking als financiële blootstelling**, in plaats van alleen hoeveelheid.

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

#### Valkuil 3 — Aannemen dat een schone SKU-koppeling schone gegevens betekent

**Beslissing:**
De medewerker gebruikt een directe opzoeking tussen de drie exports en gaat ervan uit dat niet-gekoppelde records ontbrekende voorraad vertegenwoordigen.

**Foutieve aanname:**
Er wordt verondersteld dat de SKU-strings in alle systemen identiek zijn.

**Waarom de aanbeveling verandert:**
Geëxporteerde gegevens kunnen spaties aan het begin of einde, inconsistent hoofdlettergebruik, speciale tekens, lege regels of historische SKU-naamgevingsconventies bevatten. De bron identificeert deze specifiek als praktische problemen met de gegevenskwaliteit.

Bijvoorbeeld:

```text
Shopify → "sku-001"
WMS     → "SKU-001"
3PL     → " SKU-001 "
```

Een naïeve exacte koppeling kan deze als verschillende producten interpreteren.

**Correcte aanpak:** normaliseer de identificatie voordat u tussen systemen opzoekt.

<details>
<summary>Normalisatielogica</summary>

```excel
=UPPER(TRIM([@SKU]))
```

Gebruik vervolgens de genormaliseerde sleutel voor opvraging tussen tabellen.

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

Dit vermindert valse uitzonderingen die door opmaak worden veroorzaakt in plaats van door voorraadbewegingen.

</details>

### Voorbeeldscenario

Stel dat een wekelijkse aansluiting wordt uitgevoerd voor één SKU nadat alle drie systemen op hetzelfde afsluitmoment zijn vastgelegd.

De geïmporteerde momentopnamen rapporteren:

| Bron  | Hoeveelheid |
| ------- | -------: |
| Shopify |    1.000 |
| WMS     |      992 |
| 3PL     |      970 |

De geconfigureerde kostprijs per eenheid van de SKU is **$18**.

De eerste analytische stap is niet om 30 eenheden als verloren te verklaren. Het systeem stelt de verschillen vast tussen elke gerapporteerde voorraadpositie:

```text
Shopify vs. WMS
= 1,000 - 992
= 8 units

WMS vs. 3PL
= 992 - 970
= 22 units
```

Dit levert onmiddellijk een nuttiger operationele vraag op.

De totale afwijking is niet simpelweg "30 eenheden vermist". De gegevens suggereren dat het grootste onverklaarde gat geconcentreerd is tussen de WMS- en de 3PL-vestiging.

Als de afwijking van 22 eenheden bij de 3PL onverklaard blijft na controle van zendingsmomenten, retouren, correcties en andere legitieme bewegingen, is de geschatte financiële blootstelling tegen de geconfigureerde kostprijs:

```text
22 × $18 = $396
```

De managementimplicatie is daardoor anders dan bij een generieke voorraadwaarschuwing.

De volgende actie is niet om elke SKU in gelijke mate te inspecteren. De medewerker moet eerst de **uitzondering aan de 3PL-zijde** onderzoeken, nagaan of de afwijking fysiek verlies, schade, timing of een rapportageprobleem vertegenwoordigt, en vervolgens bepalen of de afwijking de contractuele of interne tolerantie van het bedrijf overschrijdt.

Het dashboard is ontworpen om deze prioritering zichtbaar te maken: het management kan de totale financiële blootstelling, de verdeling van het verlies tussen vestigingen en de SKU-uitzonderingen met de hoogste waarde zien zonder de ruwe exports handmatig te doorlopen.

De tool ondersteunt daarmee een reeks van:

**aansluiting → isolatie van uitzonderingen → financiële kwantificering → operationeel onderzoek → mogelijke claim of procescorrectie.**

De tool bepaalt zelf niet of een afwijking juridisch verhaalbaar is. Dat blijft een management- en contractuele beslissing.

### Formuleverwijzing

De onderstaande formules beschrijven de kernpatronen van de berekeningen die voor de aansluitingsarchitectuur zijn gespecificeerd. Ze zijn bedoeld om de redenering van de werkmap auditeerbaar te maken, niet om de README in een generieke Excel-formulecatalogus te veranderen.

<details>
<summary>Normalisatie van SKU</summary>

**Doel:** geïmporteerde SKU-strings standaardiseren voordat ze worden vergeleken.

```excel
=UPPER(TRIM([@SKU]))
```

**Logica:**

* `TRIM()` verwijdert spaties aan het begin, aan het einde en overbodige spaties.
* `UPPER()` standaardiseert het gebruik van hoofdletters.
* De resulterende genormaliseerde sleutel wordt geschikt voor koppeling tussen systemen.

De bron beveelt hiervoor specifiek `TRIM()` en `UPPER()` aan.

</details>

<details>
<summary>Opvraging tussen systemen</summary>

**Doel:** de bijbehorende hoeveelheid uit een brontabel ophalen nadat de SKU is gestandaardiseerd.

```excel
=XLOOKUP(
    Normalized_SKU,
    Source_SKU_Column,
    Source_Quantity_Column,
    0
)
```

De architectuur staat `XLOOKUP` of `INDEX + MATCH` toe als mechanisme voor opvraging tussen tabellen.

Het belangrijkste ontwerpprincipe is niet de specifieke opzoekfunctie. Het is dat **de SKU-identiteit, en niet de regelpositie, de aansluiting aanstuurt**.

</details>

<details>
<summary>Berekening van de afwijking</summary>

**Doel:** het verschil tussen vergelijkbare voorraadposities kwantificeren.

```text
Absolute Variance
= Source Quantity - Reference Quantity
```

De implementatie moet het teken behouden waar een directionele interpretatie nuttig is, en absolute waarden gebruiken bij het rangschikken van de omvang van de afwijking.

```text
Variance Magnitude
= ABS(Source Quantity - Reference Quantity)
```

Dit ondersteunt zowel:

* directionele aansluiting;
* rangschikking van uitzonderingen.

</details>

<details>
<summary>Omzetting naar financieel verlies</summary>

**Doel:** voorraadafwijking omzetten in een geschatte financiële blootstelling.

```text
Estimated Loss Value
= Variance Quantity × Unit Cost
```

De kostprijs per eenheid wordt onderhouden in `Config_Master`, zodat dezelfde aansluitingsengine kan worden hergebruikt wanneer de productkosten veranderen.

De bron definieert de kostenmatrix expliciet als het mechanisme om voorraadafwijkingen om te zetten in financieel verlies.

</details>

<details>
<summary>Relatieve afwijking en risicodrempel</summary>

**Doel:** een klein numeriek verschil onderscheiden van een materiële operationele uitzondering.

Conceptueel:

```text
Discrepancy Rate
= Absolute Variance ÷ Reference Inventory
```

Het resulterende percentage kan worden vergeleken met de geconfigureerde waarschuwings- of tolerantiedrempel.

Het bronontwerp vraagt dat `Config_Master` de afwijkingsdrempels onderhoudt en dat voorwaardelijke opmaak regels markeert waarvan de hoeveelheid of het afwijkingspercentage de geconfigureerde grens overschrijdt.

</details>

### Validatieregels

De aansluitingsengine is afhankelijk van een klein aantal controles die moeten worden gerespecteerd voordat de uitvoer als beslissingskwaliteit kan worden beschouwd.

| Veld / controle                  | Regel                                                                                                           | Foutgedrag                                                                                                            |
| -------------------------------- | -------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| **SKU**                          | Moet gestandaardiseerd en consistent identificeerbaar zijn in de bronbestanden.                                        | Niet-gekoppelde of misvormde records moeten als uitzonderingen op de gegevenskwaliteit worden behandeld en niet stilzwijgend als voorraadverlies worden geclassificeerd. |
| **Uniciteit van SKU**               | Eén fysiek product moet aan één standaard-SKU-identiteit zijn gekoppeld.                                                  | Dubbele of tegenstrijdige identificaties vereisen correctie van de stamgegevens voordat betrouwbaar kan worden aangesloten.                       |
| **Kostprijs per eenheid**                    | Moet bestaan in `Config_Master` voor financiële waardering.                                                         | Hoeveelheidsafwijking kan nog steeds zichtbaar zijn, maar financiële blootstelling kan zonder kostprijs niet betrouwbaar worden gewaardeerd.                    |
| **Afsluitmoment van momentopname**             | Shopify-, WMS- en 3PL-gegevens moeten hetzelfde tijdstip vertegenwoordigen.                                               | Verschillende tijdstempels kunnen valse afwijkingen veroorzaken en vereisen een nieuwe export of correctie.                                       |
| **Geïmporteerde brongegevens**         | Ruwe exports moeten consistent in hun aangewezen importzones worden geplakt.                                  | Structurele of bronformaat-afwijkingen moeten worden gecorrigeerd voordat de resulterende uitzonderingen worden geïnterpreteerd.                   |
| **Afwijkingsdrempel**        | Hoeveelheids- en percentagedrempels moeten in de configuratie worden onderhouden in plaats van hard gecodeerd in afzonderlijke uitvoer. | Uitzonderingen die de drempel overschrijden worden gemarkeerd voor onderzoek.                                                      |
| **3PL-tolerantie / SLA**          | Met de contractuele verliestolerantie moet rekening worden gehouden bij de beslissing of een uitzondering claimbaar is.              | De werkmap levert bewijs; het management bepaalt of een contractuele claim moet worden gestart.                    |
| **Timing van retouren**               | Retouren die door een 3PL worden geregistreerd en restituties die in Shopify worden geregistreerd, kunnen op verschillende momenten plaatsvinden.                        | Kortstondige afwijkingen mogen niet automatisch als permanent voorraadverlies worden geïnterpreteerd.                                     |
| **Historische SKU-naamgeving**        | Verouderde inconsistenties in naamgeving moeten worden genormaliseerd of gekoppeld.                                                    | Niet-gekoppelde historische SKU's moeten zichtbaar blijven als uitzonderingen op de gegevenskwaliteit.                                                |
| **Vertraging in systeemsynchronisatie** | Tijdelijke synchronisatieproblemen tussen Shopify en 3PL vallen buiten de aansluitingslogica van het spreadsheet.               | Behandel dit als een probleem van systeemintegratie in plaats van een VBA-oplossing in het spreadsheet te forceren.                               |

De bron maakt expliciet onderscheid tussen problemen die Excel kan oplossen en problemen die operationele of systeemgerichte interventie vereisen. Gestandaardiseerde aansluiting, waardering van verliezen en dashboards met uitzonderingen horen binnen de werkmap; discipline bij het tellen, beheer van 3PL-claims, API-synchronisatie en GPS-tracking niet.



### Wat deze werkmap niet probeert op te lossen

De architectuur handhaaft bewust een duidelijke grens rond de Excel-laag.

**Problemen met operationeel beheer:**

* inconsistente procedures voor voorraadtellingen bij de 3PL;
* onvoldoende frequentie van fysieke voorraadtellingen;
* het nalaten om claims te starten wanneer contractuele verlieslimieten worden overschreden.

Deze vereisen managementactie in plaats van nog een formule.

**Problemen met systeemintegratie:**

* vertragingen in realtime synchronisatie tussen Shopify en 3PL;
* API-communicatie;
* geautomatiseerde ERP-integratie.

De bron beveelt specifiek aan deze problemen niet via VBA in een lichtgewicht Excel-werkmap te forceren.

**Problemen met transportzichtbaarheid:**

* realtime GPS-tracking van voorraad onderweg;
* workflows voor transportmanagement.

Deze vereisen een speciaal TMS in plaats van een spreadsheet voor voorraadaansluiting.

Deze grens is opzettelijk. Het doel van de werkmap is om een **herhaalbare laag voor aansluiting en analyse van financieel verlies** te bieden, niet om te doen alsof elk voorraadbeheerprobleem een Excel-probleem is.

### De werkmap aanschaffen

De tool is ontworpen voor terugkerende aansluiting in plaats van eenmalige spreadsheetanalyse.

De bedoelde operationele cyclus is:

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

De bronblauwdruk specificeert een wekelijkse of maandelijkse frequentie, waarbij gebruikers de drie bronexports in hun respectieve invoerbladen plakken en de actuele SKU-kosten en waarschuwingsdrempels in `Config_Master` onderhouden.

**Browserversie:** gebruik de HTML-versie voor een snelle operationele beoordeling.

**Excel-versie:** gebruik de werkmap wanneer de aansluiting moet worden ververst met werkelijke Shopify-, WMS- en 3PL-exports.

De tool is bewust zo ontworpen dat een niet-technische operations- of finance-gebruiker de terugkerende aansluiting kan uitvoeren zonder het analytische model elke keer opnieuw op te bouwen. Het brondoel is ongeveer **10 minuten** voor het opschonen, aansluiten en beoordelen van uitzonderingen.

### Beperkingen

Deze werkmap is een **laag voor aansluiting en verliesanalyse**, geen platform voor voorraadbeheer.

Ze kan niet:

* realtime synchronisatie tussen Shopify ↔ WMS ↔ 3PL garanderen;
* voorkomen dat een magazijnmedewerker een artikel fysiek verzendt terwijl de voorraad ontoereikend is;
* een WMS, ERP of voorraadbeheersysteem vervangen;
* procedures voor voorraadtellingen bij de 3PL afdwingen;
* automatisch bepalen of een afwijking contractueel verhaalbaar is;
* realtime GPS-tracking van voorraad onderweg bieden;
* historische problemen met SKU-stamgegevens oplossen zonder een passende koppelingsbeslissing.

Deze grenzen zijn expliciet in het bronontwerp. Gestandaardiseerde aansluiting, waardering van afwijkingen, rangschikking van uitzonderingen en dashboardrapportage worden beschouwd als passende Excel-problemen. Discipline bij het tellen en beheer van 3PL-claims vereisen managementcontroles; realtime API-synchronisatie hoort bij systeemintegratie; fysieke zendingtracking hoort bij een TMS.

Er zijn ook belangrijke interpretatiebeperkingen.

**Een hoeveelheidsverschil is niet automatisch voorraadverlies.** Retouren kunnen door een 3PL op een ander moment worden geregistreerd dan de bijbehorende restitutie in Shopify, en een inconsistent moment van de momentopname kan tijdelijke verschillen veroorzaken. De medewerker moet de zakelijke context valideren voordat een afwijking als permanent verlies wordt geclassificeerd.

**Het cijfer voor financieel verlies is een schatting, geen boekhoudkundige boeking.** Het is afhankelijk van de geconfigureerde kostprijs per SKU en de interpretatie van het onderliggende hoeveelheidsverschil.

**Een schoon spreadsheetresultaat garandeert geen schone brongegevens.** Historische inconsistenties in SKU-naamgeving, onvolledige exports, dubbele records of onjuiste fysieke tellingen kunnen nog steeds misleidende conclusies opleveren.

De werkmap moet daarom worden gebruikt als een **mechanisme voor feitenonderzoek en prioritering**, niet als een automatische oordeelmachine.

</details>


## Andere tools in deze serie

Een verzameling lichtgewicht Excel-tools voor besluitvormingsondersteuning op het gebied van operationele beheersing, aansluiting, winstgevendheid, voorraad en financiële analyse.

* **Voorraadplanning en bestelbeheersing** — vraag, aanvulling, voorraadblootstelling en inkoopbeslissingen.
* **Winstengine op orderniveau** — omzet, variabele kosten, toewijzing van verzendkosten en winstgevendheid per order.
* **Bouwbeheersing van één project** — projectbudget, verplichtingen, opdrachtkosten en projectwinstgevendheid.
* **Operationeel en winstgevendheidsbeheersysteem voor aannemers** — workflow van lead → raming → opdracht → arbeid en materialen → opdrachtkosten → winst → klanthistorie.

## Licentie

Dit project is vrijgegeven onder de **Apache License 2.0**.

U mag het project gebruiken, wijzigen, distribueren en aanpassen volgens de voorwaarden van de Apache License 2.0.

Zie het licentiebestand in de repository voor de volledige licentietekst.
