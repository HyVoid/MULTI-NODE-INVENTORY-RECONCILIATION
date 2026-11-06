[ 🌐 عربي ](README.ar.md) | [ 🇩🇪 Deutsch ](README.de.md) | [ 🇫🇷 Français ](README.fr.md) | [ 🇳🇱 Nederlands ](README.nl.md) | [ 🇪🇸 Español ](README.sp.md) | [ 🇬🇧 English ](README.md)

# Shopify & 3PL Inventory Reconciliation Excel Template: Warehouse Stock Discrepancy, Cycle Count Variance & Shrinkage Cost Calculator
<img width="1102" height="790" alt="image" src="https://github.com/user-attachments/assets/3a637973-b460-4160-a098-eed931e2dc18" />



[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](#license)
[![Platform: Web Browser + Microsoft Excel (.xlsx)](https://img.shields.io/badge/Platform-Web%20Browser%20%2B%20Microsoft%20Excel%20(.xlsx)-217346.svg)](#quick-start-tutorial-how-to-reconcile-shopify-wms--3pl-inventory-in-4-steps)
[![Tool Type: Plug-and-Play Ecommerce Inventory Spreadsheet](https://img.shields.io/badge/Tool%20Type-Plug--and--Play%20Inventory%20Spreadsheet-2251FF.svg)](#what-it-helps-you-track-ecommerce-inventory-pain-points-vs-solutions)

**A ready-to-use Shopify & 3PL Inventory Reconciliation Excel Template (`.xlsx`) and Free Online Stock Discrepancy Calculator built for ecommerce brands, DTC operators, and warehouse managers who need to audit inventory counts without writing formulas.** Compare **Shopify storefront quantities**, internal **Warehouse Management System (WMS) records**, and **Third-Party Logistics (3PL) physical cycle counts** side by side, calculate **COGS-weighted inventory shrinkage ($)**, stop **ghost-inventory overselling**, and generate **documented 3PL reimbursement claims** in one pre-built spreadsheet.

**Test your SKU data free in your browser right now, or download the unlocked Excel file for monthly audits.**

Every SKU matching rule, text-cleaning formula, and dollar-variance calculation is already built in. Copy and paste your raw CSV exports from Shopify, your WMS, and your 3PL to see your exact stock discrepancies and financial loss exposure in seconds—backed by a 30-day, no-questions-asked money-back guarantee.

> 🌐 **Try the Online Reconciliation Calculator First**  
> [Launch the Free Interactive Shopify & 3PL Inventory Reconciliation Web Calculator (Browser Demo, Zero Setup Required)](https://hyvoid.github.io/multi-node-inventory-reconciliation/)
> 
> 📥 **Download the Ready-to-Use Excel Template**  
> [Get the Unlocked Multi-Node Inventory Reconciliation & Shrinkage Audit Excel Template (.xlsx with Auto-Updating Formulas)](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)
>
> *Both the free browser calculator and the downloadable Microsoft Excel workbook run on the exact same pre-configured 3-way SKU matching and COGS variance tables.*

---

## What It Helps You Track: Ecommerce Inventory Pain Points vs. Solutions

Finding out that your stock numbers do not match is only half the problem—you also need to know where the units went and how much money is at stake. This **plug-and-play inventory audit spreadsheet** solves the five most common stock control blind spots for multichannel ecommerce brands:

| High-Frequency Search Topic & Tracking Goal | The Daily Ecommerce Inventory Pain Point (Where Money Leaks) | How This Pre-Built Excel Template Fixes & Tracks It |
| :--- | :--- | :--- |
| **Shopify vs. 3PL vs. WMS Stock Discrepancies (`3-Way Inventory Matching`)** | Shopify says you have 120 units, your WMS says 100, and your 3PL says 85—leaving you unsure which system holds the real stock count. | Aligns **Shopify, WMS, and 3PL quantities side by side** per SKU so you can separate IT sync delays from actual physical warehouse losses. |
| **Inventory Shrinkage Cost & COGS Write-Off (`$` Impact vs. Unit Count)** | Treating a 20-unit missing count on a $2 packaging insert with the same urgency as a 20-unit loss on a $75 hero product. | Multiplies unit variances by each SKU's **Unit Cost (COGS)** to calculate exact **Dollar Shrinkage Exposure ($)** for accounting write-offs. |
| **3PL Lost Stock & SLA Reimbursement Claims (`Shrinkage Allowance` Audit)** | You know your fulfillment center is losing merchandise, but you lack the SKU-level variance proof required to file a contract claim. | Tracks **3PL vs. Internal Warehouse Discrepancy Rates (%)** against your contractual shrinkage cap to build a factual reimbursement ledger. |
| **Ghost Inventory & Peak-Season Overselling (`Stockout` Prevention)** | Shopify displays more available units than actually sit on 3PL shelves, causing paid ads to drive orders you have to cancel and refund. | Flags every SKU where **Digital Storefront Stock exceeds Physical 3PL Stock** so you can correct inventory levels before overselling. |
| **Cycle Count Analysis Paralysis (`Top 10 Loss-Value SKUs`)** | Scrolling through thousands of spreadsheet rows after a warehouse cycle count while missing the 5 SKUs driving 80% of your financial loss. | Automatically filters out matching rows and ranks the **Top 10 Highest Dollar-Loss SKUs** on one summary dashboard for immediate action. |

---

## Quick Start Tutorial: How to Reconcile Shopify, WMS & 3PL Inventory in 4 Steps

You do not need advanced Excel skills or manual `VLOOKUP` formulas to run a warehouse audit. Follow these four steps to turn raw CSV exports into a clear **Inventory Shrinkage & Discrepancy Report**:

### Step 1: Enter Your SKU Master List, Unit COGS & Alert Thresholds (`Config_Master`)
Open the `Config_Master` tab to set your baseline inventory rules:
- Paste your master **SKU List** and **Unit Cost of Goods Sold (COGS)**.
- Set your custom **Discrepancy Warning Thresholds** (for example, flag any SKU with more than a `5-unit` gap or more than `$100` in missing inventory value).

*Preview it live:* See how the master configuration table works right now in the [Free Online 3PL Inventory Reconciliation Browser Calculator](https://hyvoid.github.io/multi-node-inventory-reconciliation/).

---

### Step 2: Copy and Paste Your Raw Shopify, WMS & 3PL CSV Exports
Skip manual column formatting and text cleanup. Paste your raw inventory exports directly into the three input tabs:
- `Import_Shopify`: Your exported Shopify product inventory CSV (storefront stock levels).
- `Import_WMS`: Your internal warehouse management system or ERP stock report.
- `Import_3PL`: Your fulfillment partner's physical cycle count or ending inventory report (compatible with exports from ShipBob, ShipMonk, Flexport, Amazon MCF, and custom 3PL portals).
- **Zero manual formula dragging:** The pre-built tables clean extra spaces, align SKU codes, and expand automatically when you paste new rows.

---

### Step 3: Check Your Shrinkage Dashboard & Top 10 Loss-Value SKUs (`Dashboard`)
Switch to the `Dashboard` tab to view your completed audit results:
- See total **Inventory Shrinkage Value ($)**, **Net Unit Variance**, and **System-to-System Accuracy Rates (%)** calculated automatically.
- Review the **Top 10 Loss-Value SKUs** list to see which exact products need a physical recount in the warehouse or an urgent stock adjustment on Shopify.

---

### Step 4: Download the Unlocked Excel Template for One-Click Monthly Audits
Use the free browser tool to test your workflow and spot immediate stock gaps today. To save your SKU cost baselines locally, run recurring month-end accounting closes, and build historical 3PL claim logs, download the unlocked `.xlsx` spreadsheet.

> 💡 **Why Growing Ecommerce Brands Use This Excel Template Instead of Building From Scratch:**  
> Cleaning messy SKU strings across three different exports, aligning mismatched rows, and weighting stock variances by unit COGS involves tedious spreadsheet engineering. **In this Excel template, every 3-way matching rule, text normalizer, and auto-updating formula is already built for you.**  
> 
> You do not even need to double-click cell corners or drag formulas down. Download the workbook to your computer, paste your monthly Shopify and 3PL exports over last month's data, and get an updated financial shrinkage audit in one click. Even if you have zero technical spreadsheet background, you get instant visibility into your inventory health—freeing you to focus on marketing, restocking bestsellers, and closing sales during peak Q4 and Black Friday seasons while a simple copy-and-paste template handles the data reconciliation.  
> 
> 👉 **[Download the Unlocked Shopify & 3PL Inventory Reconciliation Excel Template (.xlsx) and Automate Your Stock Audits Today](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)**

---

## The Business Logic & Methodology: 4 Hidden Inventory Blind Spots This Excel Template Solves for You

Most ecommerce brands lose thousands of dollars to inventory shrinkage and overselling not because they forget to count stock, but because standard 2-way checks and basic unit spreadsheets hide where the real financial damage happens. Here is how this template protects your inventory and cash flow in plain terms:

### 1. Comparing Only Two Systems Hides Whether You Have an IT Bug or Warehouse Theft (3-Way Inventory Triangulation)
**The Objective Fact:** If you only compare Shopify (100 units) against your 3PL (80 units), you know 20 units are missing, but you do not know *why*. Those 20 units could be sitting in unfulfilled orders because an API webhook failed, or 20 physical boxes could have walked out the warehouse back door.  
**Your Direct Benefit:** By matching **Shopify (Digital Storefront) + WMS (Internal Ledger) + 3PL (Physical Shelf Count)** side by side in one row, the template isolates the exact break point:
- If `Shopify ≠ WMS`, but `WMS = 3PL`: You have a storefront syncing or unfulfilled-order lag. Fix your integration settings.
- If `Shopify = WMS`, but `3PL < WMS`: Physical stock was lost, damaged, or miscounted at the fulfillment center. File a 3PL claim.

### 2. Counting Missing Units Instead of Missing Dollars Wastes Warehouse Labor (COGS-Weighted Variance Ranking)
**The Objective Fact:** A standard cycle count sheet treats every unit equally. If your team sorts discrepancies by unit count alone, they will spend hours recounting cheap packaging supplies while ignoring high-cost products that quietly drain your profit margin. Look at how raw unit counts mislead warehouse teams compared to COGS-weighted shrinkage:

```text
SKU-A (Branded Poly-Mailer):   -50 Units Missing  ×  $0.20 Unit COGS  =   -$10.00 Financial Loss
SKU-B (Wireless Headphones):    -4 Units Missing  × $115.00 Unit COGS =  -$460.00 Financial Loss

```

In a basic unit-count spreadsheet, `SKU-A` (-50 units) looks like an emergency while `SKU-B` (-4 units) looks like a minor rounding error—even though `SKU-B` costs your business **46 times more money**.

**Your Direct Benefit:** The template multiplies every unit discrepancy by its unit COGS automatically and ranks your **Top 10 Loss-Value SKUs by dollar impact**. Your team investigates the $460 loss first instead of chasing $10 worth of mailers.

### 3. 3PL Fulfillment Contracts Have Strict Claim Deadlines and Shrinkage Caps (Documented SLA Claim Proof)

**The Objective Fact:** Almost all third-party logistics (3PL) contracts include a built-in "shrinkage allowance" (typically 0.5% to 2.0% of total units handled) and require merchants to submit SKU-by-SKU variance proof within 15 to 30 days of a cycle count to qualify for reimbursement. Complaints sent over email without structured variance logs are routinely rejected by 3PL account managers.

**Your Direct Benefit:** The template calculates exact **Node-to-Node Discrepancy Percentages** and generates a clean, SKU-level variance table showing expected stock, physical count, unit deficit, and COGS value—giving you ready-to-send documentation to recover cash from your 3PL.

### 4. "Ghost Inventory" on Shopify Burns Paid Ad Spend and Triggers Chargebacks (Phantom Stock Detection)

**The Objective Fact:** When your Shopify store thinks you have 50 units in stock, your Meta and Google shopping ads keep spending money to drive traffic to that product page. If your 3PL actually has 0 units on the shelf ("ghost inventory"), every new customer order results in a fulfillment delay, a manual cancellation, lost payment processing fees, and angry customer support tickets.

**Your Direct Benefit:** The template highlights every SKU where storefront availability exceeds physical warehouse stock so you can adjust Shopify inventory quantities before overselling during high-traffic sales events.

---

## Manual Inventory Spreadsheets (`VLOOKUP`) vs. This Automated Shopify & 3PL Reconciliation Template

| Warehouse & Accounting Comparison Factor | Manual Excel Sheets (`VLOOKUP` / `INDEX-MATCH` From Scratch) | Standardized Multi-Node Inventory Reconciliation Template (This Tool) |
| --- | --- | --- |
| **3-System Stock Alignment (`Shopify` + `WMS` + `3PL`)** | Staff manually stitch three separate CSV files together every month, risking broken cell references and skipped SKUs. | Pre-built **3-Way Matching Engine** aligns Shopify, WMS, and 3PL quantities automatically as soon as you paste your exports. |
| **Dirty CSV Formatting & SKU Mismatches** | Extra trailing spaces, leading zeros, and uppercase vs. lowercase SKU codes trigger false `#N/A` errors across thousands of rows. | Built-in **Text Normalization Layer** cleans whitespace and standardizes SKU strings before calculating stock differences. |
| **Financial Shrinkage Valuation (`COGS Write-Off`)** | Reports only show missing unit quantities, forcing bookkeepers to look up product costs manually at month-end close. | Embedded **SKU Cost Matrix** converts every unit shortage into exact **Dollar Shrinkage Exposure ($)** for accounting entries. |
| **Exception Filtering (`Top Loss SKUs`)** | Managers scroll through 5,000+ matching rows trying to spot which products have dangerous stock gaps. | **Automated Exception Dashboard** filters out normal rows and ranks the **Top 10 Highest Dollar-Loss SKUs** automatically. |
| **3PL SLA Reimbursement Documentation** | Missing warehouse units are argued informally over email without historical accuracy percentages or dollar totals. | Produces an audit-ready **3PL Variance & Discrepancy Rate Ledger** to substantiate formal SLA credit and reimbursement claims. |

---

## Who This Is For: Ecommerce Roles, Inventory Use Cases & Spreadsheet Workflows

This toolkit bridges the gap between physical warehouse shelves and ecommerce financial statements. It is built for **growing DTC brands, multichannel Shopify sellers, 3PL users, and ecommerce finance teams** who want reliable inventory control without paying $30,000+ per year for an enterprise ERP:

* **Shopify Store Owners & DTC Brand Founders (`Shopify Inventory Reconciliation Excel Template`):** Spot phantom stock and missing warehouse inventory in minutes without hiring a data analyst or learning complex spreadsheet formulas.
* **Ecommerce Operations & Fulfillment Managers (`3PL Stock Discrepancy & SLA Audit Spreadsheet`):** Hold external fulfillment centers (such as ShipBob, ShipMonk, or regional 3PLs) accountable by tracking monthly shrinkage rates against contractual SLA caps.
* **Warehouse Managers & Inventory Control Clerks (`Plug-and-Play Cycle Count Variance Calculator`):** Reconcile physical bin counts against WMS ledger records after weekly or monthly cycle counts, prioritizing recounts by highest dollar value at risk.
* **Ecommerce Bookkeepers & Fractional CFOs (`Inventory Shrinkage & COGS Write-Off Accounting Model`):** Calculate exact ending inventory valuation adjustments and month-end COGS shrinkage write-offs for QuickBooks Online, Xero, or NetSuite.
* **Multichannel Amazon, Walmart & Shopify Sellers (`Multi-Warehouse Stock Comparison Sheet`):** Audit stock distribution and unlinked SKU quantities across internal warehouses, 3PL nodes, and online sales channels from a single file.

*Note: This Excel workbook does not replace live barcode scanners, real-time API inventory sync apps, or your WMS. It acts as your independent **audit and reconciliation layer** to catch the sync failures and physical shrinkage that automated software misses.*

---

## Real-World Scenarios: How to Solve Common Shopify & 3PL Inventory Problems

If your operations or finance team runs into any of these recurring inventory headaches, this spreadsheet is structured to solve them out of the box:

* **How to Prevent Overselling During Black Friday / Cyber Monday (Q4 Peak Season):** Shopify shows 100 units available, but your 3PL only has 20 on the shelf. Run this reconciliation weekly during Q4 to catch "ghost inventory" and sync your storefront counts before customers buy out-of-stock items.
* **How to Prove 3PL Lost Inventory and Claim SLA Reimbursements:** Your fulfillment partner loses high-ticket SKUs beyond their 1.5% contractual shrinkage allowance. Paste your WMS shipment logs and the 3PL's physical count into the template to generate an itemized dollar-loss report for your reimbursement claim.
* **How to Calculate Month-End Inventory Shrinkage for Ecommerce Accounting:** Your bookkeeper needs an exact dollar figure for lost or damaged stock to close the monthly P&L. Use the COGS-weighted dashboard total to book accurate inventory write-off journal entries in minutes.
* **How to Reconcile Messy Warehouse CSV Exports Without Broken `VLOOKUP` Formulas:** Different systems export SKU codes with extra spaces or inconsistent formatting. Drop the raw exports into the import tabs and let the template align and compare every SKU automatically.

---

## About Theseus Workshop

**Theseus Workshop** builds plug-and-play Microsoft Excel models and browser-based decision tools for operators who need clear, reliable numbers today—without enterprise software bloat or complex spreadsheet programming.

Every tool is designed around one practical question:

> **"What exact operational and financial numbers need to sit in one pre-built table so your next business decision takes seconds instead of hours?"**

If you want to stop wrestling with broken `VLOOKUP` sheets, surprise stockouts, and uncompensated 3PL inventory losses, grab the full Excel template below or explore our complete library of operational spreadsheets:

* 📥 **Get This Inventory Reconciliation Template:** [Download the Unlocked Shopify & 3PL Inventory Reconciliation Excel Template (.xlsx)](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)
* 🌐 **Test the Free Web Calculator:** [Open the Interactive 3PL Inventory Reconciliation Browser Simulator](https://hyvoid.github.io/MULTI-NODE-INVENTORY-RECONCILIATION/)
* 🧰 **Explore All Ready-to-Use Excel Models & Business Toolkits:** [Visit the Official Theseus Workshop Store at TheseusWorkshop.com](https://www.google.com/search?q=https://www.theseusworkshop.com%3Futm_source%3Dgithub%26utm_medium%3DGitHub%2520README%26utm_campaign%3Dreadme%2520new%2520launch%26utm_content%3Dinventory-readme-store-link)

---


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

* **[inventory-planning-reorder-point-excel](https://github.com/HyVoid/inventory-planning-reorder-point-excel)** — What purchasing decision should be made today given demand trends lead times and cash constraints? — Forecast inventory requirements by combining demand signals lead-time risk purchasing recommendations and working capital exposure.
* **[Retail-SKU-Concentration-Assortment-Diagnostic-Console](https://github.com/HyVoid/Retail-SKU-Concentration-Assortment-Diagnostic-Console)** — Which products dominate inventory risk or dilute assortment quality? — Identify SKU concentration risk and assortment efficiency across retail product catalogs.
* **[Retail-and-Maquila-Inventory-Ledger](https://github.com/HyVoid/Retail-and-Maquila-Inventory-Ledger)** — Where is inventory moving across retail and maquila operations? — Track inventory movement processing loss and stock exposure across factories warehouses and stores.
* **[Universal-3D-Cargo-Loading-Optimization-Simulator](https://github.com/HyVoid/Universal-3D-Cargo-Loading-Optimization-Simulator)** — How should cargo be loaded to reduce wasted space and operational friction? — Simulate 3D cargo loading configurations to maximize container capacity and shipping efficiency.
* **[Cross-Border-DTC-Inventory-Governance-Console](https://github.com/HyVoid/Cross-Border-DTC-Inventory-Governance-Console)** — What is the real purchasing demand after removing pre-order liabilities and expected returns? — Reconstruct true demand signals by isolating pre-order obligations and return behavior from raw sales data.
* **[inventory-allocation-fulfillment-excel](https://github.com/HyVoid/inventory-allocation-fulfillment-excel)** — Can each customer order actually be delivered on time given physical stock, reservations, in-transit containers, and open POs across all our locations? — Calculate available-to-promise quantities and net procurement requirements by reconciling physical stock, order reservations, in-transit inventory, and open purchase orders across multiple locations.

## License

This project is released under the **Apache License 2.0**.

You may use, modify, distribute, and adapt the project subject to the terms and conditions of the Apache License 2.0.

See the repository license file for the complete license text.

