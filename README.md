[ 🌐 عربي ](README.ar.md) | [ 🇩🇪 Deutsch ](README.de.md) | [ 🇫🇷 Français ](README.fr.md) | [ 🇳🇱 Nederlands ](README.nl.md) | [ 🇪🇸 Español ](README.sp.md) | [ 🇬🇧 English ](README.md)

# Multi-Node Inventory Reconciliation & Shrinkage Analysis | Shopify & 3PL Excel Template
<img width="1920" height="790" alt="image" src="https://github.com/user-attachments/assets/6689bffe-1aac-43d7-9f63-6e85a14470f0" />


[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](#license)
[![Platform: Browser + Excel](https://img.shields.io/badge/Platform-Browser%20%2B%20Excel-217346.svg)](#quick-start-tutorial-how-to-automate-your-inventory-reconciliation)
[![Tool Type: Decision Support](https://img.shields.io/badge/Tool%20Type-Decision%20Support-2251FF.svg)](#what-it-helps-you-track-inventory-pain-points-vs-solutions)

**An automated inventory reconciliation spreadsheet and shrinkage analysis template designed for multichannel ecommerce brands. Instantly compare Shopify stock levels, internal Warehouse Management System (WMS) records, and Third-Party Logistics (3PL) physical counts to locate discrepancies and translate unit loss into direct financial impact—without writing VLOOKUP formulas or rebuilding reports every month.**

**No signup. No installation. Free in your browser.**

Test your operational data in the free browser version instantly. For ongoing monthly month-end closes and offline data security, upgrade to the fully unlocked Excel template with a 30-day, no-questions-asked money-back guarantee.

> 🌐 **Open Interactive Dashboard**  
> [Try the Free Browser-Based 3PL Inventory Reconciliation Simulator](https://hyvoid.github.io/MULTI-NODE-INVENTORY-RECONCILIATION/)
> 
> 📥 **Get the Reusable Spreadsheet**  
> [Download the Inventory Shrinkage & Audit Excel Template](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)

---

## What It Helps You Track: Inventory Pain Points vs. Solutions

Instead of merely identifying that "numbers don't match," this toolkit translates raw stock differences into a financial action plan.

| E-commerce Inventory Pain Point (The "Why") | Reconciliation Solution (The "How") |
| :--- | :--- |
| **Cross-System Blind Spots:** Unsure which system (Shopify vs. 3PL vs. WMS) holds the ground truth for available stock. | **Multi-Node Triangulation:** Aligns system-reported quantities side-by-side to pinpoint exactly where data syncs fail. |
| **Unquantified Financial Shrinkage:** Treating a 20-unit variance on a $5 item the same as a $50 item. | **COGS-Weighted Variance Analysis:** Multiplies unit discrepancies by SKU cost to reveal the true financial write-off exposure. |
| **Third-Party Logistics (3PL) Leakage:** Suspecting fulfillment partners are losing stock, but lacking hard proof for SLA claims. | **Discrepancy Rate Tracking:** Isolates 3PL vs. internal warehouse variance rates to build a factual basis for contractual loss claims. |
| **Analysis Paralysis via Raw Data:** Scrolling through thousands of rows of cycle count spreadsheets to find errors. | **Exception-Based Dashboarding:** Automatically ranks the "Top 10 Loss-Value SKUs" to prioritize management investigations. |

---

## Quick Start Tutorial: How to Automate Your Inventory Reconciliation

Transform messy, multi-source exports into an executive inventory audit in four structured steps.

### Step 1: Configure Your SKU Master Data (One-Time Setup)
Navigate to the `Config_Master` sheet. Define your standard SKU nomenclature, unit cost (COGS), and business-specific warning thresholds (e.g., flag any discrepancy > 5 units or > $100 value). This baseline ensures all incoming data is measured against a single source of truth.

### Step 2: Import WMS, 3PL, and Shopify Exports
Bypass manual data normalization. Paste your raw CSV exports directly into their designated tabs:
*   `Import_Shopify` (Your storefront availability)
*   `Import_WMS` (Your internal warehouse records)
*   `Import_3PL` (Your external fulfillment physical counts)
*Note: The system is engineered to ingest raw exports directly—no manual column deletion or rebuilding required.*

### Step 3: Generate the Shrinkage Dashboard & Review Exceptions
Navigate to the `Dashboard` output. The automated reconciliation engine instantly cleans formatting, aligns SKUs, and calculates discrepancies. Review your highest-value inventory variances, overall shrinkage value, and node-to-node accuracy rates without manually calculating a single cell.

### Step 4: Establish a Routine & Download for Repeated Use
For your first audit, use the browser version to identify immediate stock issues. To establish a robust monthly inventory control cadence, export the system for long-term use.

👉 **Action Required:** Once you've validated your workflow, **[Download the reusable Inventory Reconciliation Excel Template here](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)**. Next month, simply paste the new inventory snapshot over the old data—the entire variance analysis will refresh automatically.

---

## The Business Logic & Methodology

This toolkit is engineered around professional auditing principles, shifting the focus from data aggregation to proactive asset protection. Here is the operational methodology powering the workbook:

### 1. Methodology: 3-Way Inventory Matching
*   **The Method:** Similar to AP financial audits, this framework employs a **3-way matching principle** across digital sales (Shopify), internal tracking (WMS), and physical storage (3PL). 
*   **The Business Impact:** It stops the "blame game." By triangulating data, operations managers can identify if an issue is a storefront syncing error (API lag) or a physical fulfillment loss (shrinkage), dramatically reducing resolution time.

### 2. Methodology: Financial Value-at-Risk (VaR) Prioritization
*   **The Method:** Discrepancies are inherently weighted by Cost of Goods Sold (COGS). The calculation layer transforms `Unit Variance` into `Financial Write-off Exposure`.
*   **The Business Impact:** It optimizes labor allocation. Instead of warehouse staff spending 4 hours investigating a 50-unit variance on poly-mailers, they are redirected by the dashboard to investigate a 3-unit variance on high-margin electronics.

### 3. Methodology: Exception-Based Reporting
*   **The Method:** The toolkit filters thousands of matching SKUs into a condensed list of operational exceptions based on user-defined tolerance thresholds (e.g., acceptable shrinkage < 0.5%).
*   **The Business Impact:** It creates **productized reasoning**. The supply chain director isn't looking at a data dump; they are looking at an actionable punch list for internal process correction or 3PL claim filing.

---

## Real-World Scenarios: When to Use This Inventory Audit Template

This system is purpose-built for critical supply chain inflection points where physical stock accuracy dictates financial health.

*   **Scenario A: Month-End Financial Close.** Finance teams need an exact COGS write-off figure for accounting. Use this template to calculate the exact dollar value of lost inventory across all warehouses on the last day of the month.
*   **Scenario B: 3PL SLA Contract Disputes.** You suspect your fulfillment partner is losing merchandise beyond the 1.5% shrinkage allowance. Use the multi-node comparison to generate a documented claim report for missing high-ticket SKUs.
*   **Scenario C: Peak Season Stockout Prevention (Q4/Black Friday).** Shopify shows 100 units, but the 3PL only has 20. Run this reconciliation weekly during Q4 to catch "ghost inventory" before customers buy stock you don't physically possess, preventing massive refund rates and customer support tickets.

---

## Common Inventory Operations Problems This Solves

| Inventory Operations Problem | Manual Spreadsheet Process | Automated Template Solution |
| :--- | :--- | :--- |
| **Three disparate systems disagree** | Operators manually run `INDEX/MATCH` across Shopify, WMS, and 3PL files, increasing broken reference risks. | A standardized reconciliation layer aligns all stock keeping units (SKUs) automatically. |
| **Messy exported data formatting** | Blank rows, trailing spaces, and case-sensitive SKUs create false mismatch errors. | The calculation layer normalizes strings and data types prior to variance checking. |
| **Shrinkage is measured only in units** | Management sees a unit deficit but cannot accurately estimate the COGS impact. | The embedded SKU cost matrix converts quantity deficits into estimated financial write-offs. |
| **Large exceptions are buried in detail** | Controllers scan thousands of rows and miss commercially fatal stock discrepancies. | The executive dashboard highlights 3PL error rates, dead stock, and top 10 loss-value items. |
| **3PL losses are difficult to substantiate** | Missing inventory remains an informal warehouse complaint without documentation. | Generates a factual variance ledger to support formal 3PL SLA claims and reimbursements. |

---

## Who This Is For: Roles & Use Cases

This tool bridges the gap between physical warehousing and financial reporting. It is purposefully designed for:

*   **Ecommerce Operations Managers** needing a *Shopify inventory reconciliation template* to sync digital storefronts with physical fulfillment centers.
*   **Supply Chain Directors** looking for a *3PL audit software alternative* to hold external partners accountable for contractual shrinkage rates.
*   **Inventory Controllers & Warehouse Managers** conducting monthly *cycle count reconciliations* across multiple internal nodes.
*   **Fractional CFOs & Finance Managers** requiring an accurate method to calculate *inventory shrinkage and COGS impact* for month-end accounting closes.
*   **DTC Founders** who need an executive-level overview of inventory health without investing in complex, six-figure ERP integrations.

*Note: This toolkit is **not** designed to replace real-time APIs, ERP systems, or live WMS barcode scanning. It is a periodic decision-support framework used to audit those systems.*

---

## About the Creator

I build lightweight operational trackers and decision-support tools for situations where there are too many moving parts to hold in your head, but not enough complexity to justify another enterprise system.

The central question is simple: **What information needs to be in one centralized place before the next strategic supply-chain decision can be made confidently?**

This Multi-Node Inventory Reconciliation workbook is one example of that approach: turning recurring cross-system stock comparisons into a standardized analytical workflow that connects operational discrepancies to financial consequences.


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

