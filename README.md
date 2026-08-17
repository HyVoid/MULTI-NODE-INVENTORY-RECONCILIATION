
# Stop Explaining Inventory Loss. Start Locating It.
# Multi-Node Inventory Reconciliation & Shrinkage Analysis

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](#license)
[![Platform: Browser + Excel](https://img.shields.io/badge/Platform-Browser%20%2B%20Excel-217346.svg)](#quick-start-workflow)
[![Tool Type: Decision Support](https://img.shields.io/badge/Tool%20Type-Decision%20Support-2251FF.svg)](#what-it-helps-you-track)

**A lightweight inventory reconciliation and shrinkage analysis tool for comparing Shopify, WMS, and 3PL inventory, locating discrepancies, and translating stock loss into financial impact — without rebuilding the analysis every reporting cycle.**

> **No signup. No installation. Free.**
>
> 🌐 **[Open in Browser](https://hyvoid.github.io/MULTI-NODE-INVENTORY-RECONCILIATION/)** — HTML live version
> 📥 **[Download Excel](https://alexhasgreatestuff.gumroad.com/l/ddongr)** — Excel version

## Screenshots

<!-- screenshot: browser version -->

**Browser version — operational reconciliation view**
Shows the standardized inventory comparison and exception analysis without requiring a local Excel workflow.

<!-- screenshot: Excel version -->

**Excel version — management dashboard**
Shows total inventory variance, estimated shrinkage value, node-level discrepancy rates, and the highest-risk SKUs for investigation.

## What It Helps You Track

* **Shopify vs. WMS vs. 3PL inventory differences** — see where system-reported quantities stop agreeing.
* **Total inventory variance and estimated shrinkage value** — understand the financial consequence rather than reviewing quantity differences alone.
* **3PL vs. internal warehouse discrepancy rates** — distinguish where the largest reconciliation problem is concentrated.
* **Top loss-value SKUs** — identify which products deserve investigation first.
* **High-risk exceptions** — surface SKUs whose quantity or discrepancy rate exceeds the configured warning threshold.
* **Potential 3PL claim exposure** — provide a fact base for internal process correction or contractual loss claims.

## Quick Start Workflow

1. **Set key parameters.**
   On `Config_Master`, maintain the standard SKU list, product information, unit cost, and the discrepancy or warning thresholds used by the business.

2. **Import existing data.**
   Paste the latest Shopify export into `Import_Shopify`, the WMS inventory export into `Import_WMS`, and the 3PL physical inventory export into `Import_3PL`. The intended workflow is to use the original exports directly rather than manually rebuilding a normalized reconciliation table.

3. **Get the results.**
   Move to the reconciliation output and `Dashboard`. The workbook cleans and aligns the imported records, compares inventory quantities across nodes, calculates discrepancies, and converts relevant differences into financial values.

4. **Maintain with periodic refresh.**
   Repeat the process weekly or monthly using a consistent inventory cut-off time. The workbook is intentionally lightweight: refresh the source data rather than rebuilding the analysis.

**Set the control parameters. Drop in the existing inventory exports. Get the reconciliation. Investigate the exceptions. Refresh when you need to.**

## Why I Built This

Multi-node inventory problems are rarely caused by the absence of a number. They are caused by **different systems presenting different versions of the same number**.

A Shopify inventory export may describe what the selling system believes is available. A WMS export may describe what the internal warehouse records as being in stock. A 3PL report may describe physical inventory held at an external fulfillment location. When these files are manually joined every week, the reconciliation process itself becomes another source of error.

The failure is especially costly because a variance is usually treated as a quantity problem:

> “SKU A is short by 18 units.”

That statement does not answer the management question.

The useful question is:

> **Where did those 18 units disappear, and what does that difference mean financially?**

This tool turns the reconciliation into a repeatable analytical workflow. Instead of manually comparing three spreadsheets, the user establishes a standard SKU reference, imports the three inventory snapshots, and lets the workbook align the records and calculate the differences.

For example, a 20-unit discrepancy on a $3 item and a 20-unit discrepancy on a $45 item should not receive the same management priority. Introducing the SKU cost matrix converts quantity variance into an estimated financial exposure. The dashboard can then rank the highest-value discrepancies rather than forcing the operator to inspect every row manually.

The result is **productized reasoning**: a reusable framework for answering the same operational question every week or month, rather than a one-off spreadsheet assembled around a single reconciliation event.

## Common Inventory Reconciliation Problems This Solves

| Problem                                      | Without This Tool                                                                                                  | With This Tool                                                                                                   |
| -------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------- |
| **Three systems disagree**                   | Shopify, WMS, and 3PL exports are manually compared, increasing the risk of missed rows and inconsistent matching. | A standardized reconciliation layer aligns records around the configured SKU reference.                          |
| **Messy exported data**                      | Blank rows, inconsistent formatting, spaces, and capitalization create false mismatches.                           | The calculation layer normalizes key fields before comparison.                                                   |
| **Variance is measured only in units**       | Management sees a stock difference but cannot immediately estimate its financial significance.                     | SKU unit cost converts relevant quantity differences into estimated loss value.                                  |
| **Large exceptions are buried in detail**    | Operators scan long reconciliation tables and can miss commercially important discrepancies.                       | Dashboard outputs highlight discrepancy rates, loss value, and Top 10 high-value SKUs.                           |
| **3PL losses are difficult to substantiate** | A suspected loss may remain an informal operational complaint.                                                     | A standardized reconciliation report provides a factual basis for investigation and potential claim preparation. |
| **Reconciliation happens too late**          | Inventory is reviewed reactively after discrepancies have accumulated.                                             | A weekly or monthly control cadence supports proactive reconciliation and exception follow-up.                   |

## Who This Is For

This tool is designed for **e-commerce and retail operators, supply-chain managers, finance teams, inventory controllers, and business owners** who receive inventory data from multiple operational nodes and need a repeatable way to reconcile it without introducing a full ERP or custom integration project.

It is particularly suited to businesses where Shopify, an internal WMS, and one or more 3PL inventory reports must be compared on a recurring basis.

It is **not** designed to replace an ERP, WMS, TMS, or real-time API integration. It does not provide GPS tracking, prevent physical overselling at transaction time, or resolve instantaneous system synchronization delays. Those are system-integration or operational-control problems rather than spreadsheet reconciliation problems.

**No spreadsheet expertise is required to understand the browser version. Open it, review the workflow, and determine whether the reconciliation model fits the operating process.**

## About

I build lightweight operational trackers and decision-support tools for situations where there are too many moving parts to hold in your head, but not enough complexity to justify another enterprise system.

The central question is simple: **What information needs to be in one place so the next operational decision can be made confidently?**

Multi-Node Inventory Reconciliation & Shrinkage Analysis is one example of that approach: turn recurring cross-system inventory comparison into a standardized analytical workflow that connects operational discrepancies to financial consequences.
## Technical Details

<details>
<summary>For technical reviewers, Excel practitioners, and collaborators</summary>

### Workbook Architecture

The workbook is deliberately structured as a **data-cleaning and reconciliation engine + financial-loss decision dashboard**, rather than as a permanent inventory database. Each reconciliation cycle can overwrite the previous import set or be saved as a separate workbook, keeping the file lightweight and avoiding unnecessary database or macro dependencies.

The architecture follows a simple:

**Input → Normalize → Reconcile → Quantify → Flag → Present**

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

The workbook is divided into six functional sheets:

| Sheet            | Layer         | Responsibility                                                            | Primary User           |
| ---------------- | ------------- | ------------------------------------------------------------------------- | ---------------------- |
| `Dashboard`      | Decision      | KPI summary, loss exposure, node comparison, Top 10 exceptions            | CEO / Management       |
| `Config_Master`  | Configuration | Standard SKU list, product information, unit cost, discrepancy thresholds | Operations / Finance   |
| `Import_Shopify` | Input         | Raw Shopify inventory export                                              | Operations             |
| `Import_WMS`     | Input         | Raw internal WMS inventory export                                         | Warehouse / Operations |
| `Import_3PL`     | Input         | Raw 3PL physical inventory export                                         | 3PL / Operations       |
| `Calc_Engine`    | Calculation   | Data normalization, SKU matching, variance calculations, financial impact | Hidden technical layer |

The three import sheets are intentionally kept as **paste zones**. The source specification allows users to paste the original exports directly, including compatibility with leading blank rows, instead of forcing them to manually reshape the files before reconciliation.

### Data Flow and Reconciliation Logic

The core calculation layer uses `Config_Master` as the reference point for standardized SKUs.

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

The design specifically addresses the problem of **messy data**. The source architecture calls for `TRIM()` to remove hidden or accidental spaces and `UPPER()` to normalize capitalization, followed by `XLOOKUP` or `INDEX + MATCH` for non-invasive cross-table retrieval.

This matters because a SKU such as:

```text
ABC-001
```

should not become a false exception simply because another export contains:

```text
 abc-001
```

The reconciliation engine therefore treats normalization as a prerequisite to comparison rather than trying to solve data-quality problems after the variance report has already been generated.

### Reconciliation Cut-Off Principle

Inventory snapshots must represent the **same business cut-off time**.

For example:

```text
Shopify Snapshot     → Sunday 23:59:59
WMS Snapshot         → Sunday 23:59:59
3PL Physical Count   → Sunday 23:59:59
```

If the snapshots are taken at materially different times, inventory movements, returns, or in-transit orders can create apparent differences that are not actual shrinkage.

The source architecture explicitly identifies consistent cut-off time as a core operating constraint and warns that mismatched snapshots can create “false differences.”

This is therefore a **business-control requirement**, not merely a spreadsheet formula requirement.

### SKU as the Single Reconciliation Key

The SKU is treated as the standard identity connecting the three source systems.

The configuration layer maintains:

* Standard SKU
* Product name
* Unit cost
* Discrepancy threshold
* Warning threshold

The calculation engine then uses that standard key to retrieve quantities from each source.

This prevents the reconciliation from depending on the row order of the imported files. Shopify can list SKUs in one sequence, WMS in another, and 3PL in a third; the calculation engine still compares the same product against the same product.

The source specification emphasizes SKU uniqueness and consistency as a fundamental constraint: one physical product should not be represented by multiple inconsistent identifiers.

### Dashboard Architecture

The Dashboard is intentionally designed for **exception-first management**, not for reproducing the raw source tables.

The primary KPI layer contains:

* Total quantity variance
* Total estimated financial loss
* 3PL discrepancy rate
* Internal warehouse discrepancy rate

The visual layer then provides:

* Loss-value distribution between 3PL and internal warehouse
* Top 10 SKUs ranked by loss value
* High-risk exception identification

These outputs are directly specified in the source architecture.

The intended management sequence is:

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

This is why the workbook is better understood as a **decision-support layer** than as a simple inventory comparison spreadsheet.

### Three Traps That Catch Even Experienced Inventory Operators

#### Trap 1 — Treating Every Quantity Difference as Shrinkage

**Decision:**
An operator sees that Shopify reports 1,000 units while the 3PL reports 970 and immediately records 30 units as lost.

**Faulty number:**
The comparison uses snapshots taken at different times.

**Why the recommendation changes:**
The 30-unit difference may represent shipments, returns, adjustments, or other movements occurring between the two snapshots.

**Correct approach:**
First establish a common cut-off time and compare like-for-like inventory snapshots.

| Approach                 | Result                                             |
| ------------------------ | -------------------------------------------------- |
| Different snapshot times | 30-unit difference treated as loss                 |
| Common cut-off           | Only residual unexplained variance is investigated |

The source specifically identifies cut-off inconsistency as a cause of false discrepancies.

The corrected decision is therefore **“investigate the residual variance”**, not **“claim the full variance as shrinkage.”**

<details>
<summary>Calculation logic</summary>

```text
Comparable Variance
= Quantity at Node A
- Quantity at Node B

Only when:
Snapshot_A_Time = Snapshot_B_Time
```

A discrepancy should not be interpreted as financial loss until the comparison basis itself is valid.

</details>

#### Trap 2 — Ranking Problems by Units Instead of Money

**Decision:**
The operator sorts the reconciliation report by the largest quantity discrepancy.

**Faulty metric:**
A 50-unit variance is ranked above a 10-unit variance simply because `50 > 10`.

**Why the recommendation is incomplete:**
Quantity does not represent economic significance.

Suppose:

| SKU   | Variance | Unit Cost | Estimated Exposure |
| ----- | -------: | --------: | -----------------: |
| SKU-A |       50 |        $2 |               $100 |
| SKU-B |       10 |       $40 |               $400 |

A quantity-only ranking would investigate SKU-A first. A financial-loss ranking would investigate SKU-B first.

The source architecture explicitly calls for introducing a SKU cost matrix so that quantity differences can be translated into financial loss.

**Correct decision:** prioritize exceptions using both **quantity variance and financial exposure**, rather than quantity alone.

<details>
<summary>Calculation logic</summary>

```text
Estimated Loss Value
= Variance Quantity × Unit Cost
```

For the example:

```text
SKU-A = 50 × $2  = $100
SKU-B = 10 × $40 = $400
```

The second exception has the smaller quantity but the larger financial consequence.

</details>

#### Trap 3 — Assuming a Clean SKU Match Means Clean Data

**Decision:**
The operator uses a direct lookup between the three exports and assumes unmatched records represent missing inventory.

**Faulty assumption:**
The SKU strings are presumed to be identical across systems.

**Why the recommendation changes:**
Exported data can contain leading/trailing spaces, inconsistent capitalization, special characters, blank rows, or historical SKU naming conventions. The source specifically identifies these as practical data-quality problems.

For example:

```text
Shopify → "sku-001"
WMS     → "SKU-001"
3PL     → " SKU-001 "
```

A naive exact match can interpret these as different products.

**Correct approach:** normalize the identifier before cross-system lookup.

<details>
<summary>Normalization logic</summary>

```excel
=UPPER(TRIM([@SKU]))
```

Then use the normalized key for cross-table retrieval.

Conceptually:

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

This reduces false exceptions caused by formatting rather than inventory movement.

</details>

### Example Scenario

Assume a weekly reconciliation is performed for a single SKU after all three systems have been captured at the same cut-off time.

The imported snapshots report:

| Source  | Quantity |
| ------- | -------: |
| Shopify |    1,000 |
| WMS     |      992 |
| 3PL     |      970 |

The SKU's configured unit cost is **$18**.

The first analytical step is not to declare 30 units lost. The system establishes the differences between each reported inventory position:

```text
Shopify vs. WMS
= 1,000 - 992
= 8 units

WMS vs. 3PL
= 992 - 970
= 22 units
```

This immediately provides a more useful operational question.

The total discrepancy is not simply “30 units missing.” The data suggests that the largest unexplained gap is concentrated between the WMS and 3PL node.

If the 22-unit 3PL variance remains unexplained after checking shipment timing, returns, adjustments, and other legitimate movements, the estimated financial exposure at the configured cost is:

```text
22 × $18 = $396
```

The management implication is therefore different from a generic inventory warning.

The next action is not to inspect every SKU equally. The operator should investigate the **3PL-side exception first**, verify whether the variance represents physical loss, damage, timing, or a reporting issue, and then determine whether the discrepancy exceeds the company's contractual or internal tolerance.

The dashboard is designed to make this prioritization visible: management can see the total financial exposure, the distribution of loss between nodes, and the highest-value SKU exceptions without manually scanning the raw exports.

The tool therefore supports a sequence of:

**reconciliation → exception isolation → financial quantification → operational investigation → potential claim or process correction.**

It does not itself determine whether a discrepancy is legally recoverable. That remains a management and contractual decision.

### Formula Reference

The formulas below describe the core calculation patterns specified for the reconciliation architecture. They are intended to make the workbook's reasoning auditable rather than to turn the README into a generic Excel formula catalog.

<details>
<summary>SKU Normalization</summary>

**Purpose:** standardize imported SKU strings before comparison.

```excel
=UPPER(TRIM([@SKU]))
```

**Logic:**

* `TRIM()` removes leading, trailing, and redundant spaces.
* `UPPER()` standardizes letter capitalization.
* The resulting normalized key becomes suitable for cross-system matching.

The source specifically recommends `TRIM()` and `UPPER()` for this purpose.

</details>

<details>
<summary>Cross-System Lookup</summary>

**Purpose:** retrieve the corresponding quantity from a source table after the SKU has been standardized.

```excel
=XLOOKUP(
    Normalized_SKU,
    Source_SKU_Column,
    Source_Quantity_Column,
    0
)
```

The architecture permits `XLOOKUP` or `INDEX + MATCH` as the cross-table retrieval mechanism.

The important design principle is not the specific lookup function. It is that **SKU identity, rather than row position, controls reconciliation**.

</details>

<details>
<summary>Variance Calculation</summary>

**Purpose:** quantify the difference between comparable inventory positions.

```text
Absolute Variance
= Source Quantity - Reference Quantity
```

The implementation should preserve the sign where directional interpretation is useful and use absolute values when ranking the magnitude of the discrepancy.

```text
Variance Magnitude
= ABS(Source Quantity - Reference Quantity)
```

This supports both:

* directional reconciliation;
* exception ranking.

</details>

<details>
<summary>Financial Loss Conversion</summary>

**Purpose:** convert inventory variance into an estimated financial exposure.

```text
Estimated Loss Value
= Variance Quantity × Unit Cost
```

The unit cost is maintained in `Config_Master`, allowing the same reconciliation engine to be reused when product costs change.

The source explicitly defines the cost matrix as the mechanism for translating stock discrepancies into financial loss.

</details>

<details>
<summary>Relative Variance and Risk Threshold</summary>

**Purpose:** distinguish a small numerical difference from a material operational exception.

Conceptually:

```text
Discrepancy Rate
= Absolute Variance ÷ Reference Inventory
```

The resulting rate can be compared against the configured warning or tolerance threshold.

The source design calls for `Config_Master` to maintain discrepancy thresholds and for conditional formatting to flag rows whose quantity or discrepancy rate crosses the configured limit.

</details>

### Validation Rules

The reconciliation engine depends on a small number of controls that must be respected before the output can be treated as decision-grade.

| Field / Control                  | Rule                                                                                                           | Error Behavior                                                                                                            |
| -------------------------------- | -------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| **SKU**                          | Must be standardized and consistently identifiable across source files.                                        | Unmatched or malformed records should be treated as data-quality exceptions rather than silently classified as shrinkage. |
| **SKU uniqueness**               | One physical product should map to one standard SKU identity.                                                  | Duplicate or conflicting identifiers require master-data correction before reliable reconciliation.                       |
| **Unit Cost**                    | Must exist in `Config_Master` for financial valuation.                                                         | Quantity variance may still be visible, but financial exposure cannot be reliably valued without cost.                    |
| **Snapshot Cut-off**             | Shopify, WMS, and 3PL data should represent the same time point.                                               | Different timestamps can create false variance and require re-export or adjustment.                                       |
| **Imported source data**         | Raw exports should be pasted consistently into their designated import zones.                                  | Structural or source-format anomalies should be corrected before interpreting the resulting exceptions.                   |
| **Discrepancy threshold**        | Quantity/rate thresholds should be maintained in configuration rather than hard-coded into individual outputs. | Exceptions crossing the threshold are highlighted for investigation.                                                      |
| **3PL tolerance / SLA**          | Contractual loss tolerance must be considered when deciding whether an exception is claim-worthy.              | The workbook provides evidence; management determines whether a contractual claim should be initiated.                    |
| **Returns timing**               | Returns recorded by a 3PL and refunds recorded in Shopify may occur at different times.                        | Short-term mismatches should not automatically be interpreted as permanent shrinkage.                                     |
| **Historical SKU naming**        | Legacy naming inconsistencies must be normalized or mapped.                                                    | Unmapped historical SKUs should remain visible as data-quality exceptions.                                                |
| **System synchronization delay** | Temporary Shopify/3PL synchronization issues are outside the spreadsheet's reconciliation logic.               | Treat as a system-integration issue rather than forcing a VBA-based spreadsheet workaround.                               |

The source explicitly distinguishes between problems Excel can solve and problems requiring operational or system-level intervention. Standardized reconciliation, loss valuation, and exception dashboards belong inside the workbook; cycle-count discipline, 3PL claim management, API synchronization, and GPS tracking do not.



### What This Workbook Does Not Attempt to Solve

The architecture deliberately maintains a clear boundary around the Excel layer.

**Operational management problems:**

* inconsistent 3PL cycle-count procedures;
* insufficient physical inventory-count frequency;
* failure to initiate claims when contractual loss limits are exceeded.

These require management action rather than another formula.

**System integration problems:**

* real-time Shopify ↔ 3PL synchronization delays;
* API communication;
* automated ERP integration.

The source specifically recommends not forcing these problems into a lightweight Excel workbook through VBA.

**Transportation visibility problems:**

* real-time GPS tracking of inventory in transit;
* transportation-management workflows.

These require a dedicated TMS rather than an inventory reconciliation spreadsheet.

This boundary is intentional. The purpose of the workbook is to provide a **repeatable reconciliation and financial-loss analysis layer**, not to pretend that every inventory-control problem is an Excel problem.

### Get The Workbook

The tool is designed for recurring reconciliation rather than one-time spreadsheet analysis.

The intended operating cycle is:

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

The source blueprint specifies a weekly or monthly cadence, with users pasting the three source exports into their respective input sheets and maintaining current SKU costs and warning thresholds in `Config_Master`.

**Browser version:** use the HTML version for a quick operational review.

**Excel version:** use the workbook when the reconciliation needs to be refreshed with actual Shopify, WMS, and 3PL exports.

The tool is intentionally designed so that a non-technical operations or finance user can complete the recurring reconciliation without rebuilding the analytical model each time. The source target is approximately **10 minutes** for cleaning, reconciling, and reviewing exceptions.

### Limitations

This workbook is a **reconciliation and loss-analysis layer**, not an inventory-control platform.

It cannot:

* guarantee real-time Shopify ↔ WMS ↔ 3PL synchronization;
* prevent a warehouse operator from physically shipping an item when stock is insufficient;
* replace a WMS, ERP, or inventory-management system;
* enforce 3PL cycle-count procedures;
* automatically determine whether a discrepancy is contractually recoverable;
* provide real-time GPS tracking of inventory in transit;
* resolve historical SKU master-data problems without an appropriate mapping decision.

These boundaries are explicit in the source design. Standardized reconciliation, discrepancy valuation, exception ranking, and dashboard reporting are considered appropriate Excel problems. Cycle-count discipline and 3PL claim management require management controls; real-time API synchronization belongs to system integration; physical shipment tracking belongs to a TMS.

There are also important interpretation constraints.

**A quantity difference is not automatically shrinkage.** Returns can be recorded by a 3PL at a different time from the corresponding Shopify refund, and inconsistent snapshot timing can create temporary differences. The operator must validate the business context before classifying a discrepancy as permanent loss.

**The financial-loss figure is an estimate, not an accounting entry.** It depends on the configured SKU unit cost and the interpretation of the underlying quantity difference.

**A clean spreadsheet result does not guarantee clean source data.** Historical SKU naming inconsistencies, incomplete exports, duplicate records, or incorrect physical counts can still produce misleading conclusions.

The workbook should therefore be used as a **fact-finding and prioritization mechanism**, not as an automatic judgment engine.

</details>


## Other Tools in This Series

A collection of lightweight Excel decision-support tools covering operational control, reconciliation, profitability, inventory, and financial analysis.

* **Inventory Planning & Reorder Control** — demand, replenishment, inventory exposure, and purchasing decisions.
* **Order-Level Profit Engine** — revenue, variable costs, shipping allocation, and order-level profitability.
* **Single-Project Construction Control** — project budget, commitments, job costs, and project profitability.
* **Contractor Operations & Profitability Management System** — Lead → Estimate → Job → Labor & Materials → Job Cost → Profit → Customer History workflow.

## License

This project is released under the **Apache License 2.0**.

You may use, modify, distribute, and adapt the project subject to the terms and conditions of the Apache License 2.0.

See the repository license file for the complete license text.

