
# Stop Explaining Inventory Loss. Start Locating It.

![Platform](https://img.shields.io/badge/platform-Excel%20%7C%20HTML-blue)
![Type](https://img.shields.io/badge/type-Decision%20Support-orange)

## **Turn inventory discrepancies into operational evidence before they become profit leakage.**

No ERP replacement. No macros. No consultants. No guessing.

---

## Navigation

* 🔍 **Live Demo:** `./demo/index.html`
* 📥 **Download:** `./Multi-Node-Inventory-Reconciliation.xlsx`
* 📚 **Methodology:** [`docs/methodology.md`](./docs/methodology.md)

---

## Hero

> **[ HERO IMAGE PLACEHOLDER ]**
>
> Dashboard showing:
>
> * Total Inventory Loss ($)
> * 3PL vs WMS discrepancy distribution
> * Top 10 shrinkage SKUs
> * Warehouse risk ranking
> * Claim candidate alerts

---

# What Decision Does This Help You Make?

Instead of producing another report, this workbook answers four operational questions.

### 1. Is inventory actually missing?

Distinguishes:

* system timing differences,
* data formatting problems,
* genuine physical shrinkage.

---

### 2. Where did the discrepancy originate?

Separates discrepancies across:

* Shopify,
* Internal warehouse,
* 3PL.

No more "everyone blames everyone."

---

### 3. Is the amount material?

Converts units into money.

```
Loss Amount = Quantity Difference × Unit Cost
```

Operational inconvenience becomes financial exposure.

---

### 4. Does this justify escalation?

Identifies:

* SKUs exceeding tolerance,
* warehouses exceeding SLA,
* cases suitable for 3PL claims.

Escalation becomes evidence-based.

---

# About The Builder

Business problems are often framed as software problems.

Most are not.

Many recurring operational failures arise from:

* inconsistent definitions,
* missing validation steps,
* invisible assumptions,
* broken decision workflows.

This project does not attempt to replace enterprise systems.

It productizes a proven analytical process.

The objective is simple:

> Transform repeated business analysis into lightweight decision tools that non-technical teams can execute consistently.

No platform migration.

No implementation project.

No reinvention of the same spreadsheet every month.

---

# Who This Is For

| Role                 | Typical Situation                                    | Decision Supported           |
| -------------------- | ---------------------------------------------------- | ---------------------------- |
| CEO                  | Gross margin deteriorates without clear cause        | Determine financial exposure |
| Operations Manager   | Weekly inventory reconciliation consumes days        | Prioritize investigations    |
| Finance Team         | Inventory adjustments lack evidence                  | Quantify losses              |
| Supply Chain Manager | 3PL accountability unclear                           | Initiate claims              |
| E-commerce Operator  | Shopify availability conflicts with warehouse counts | Identify source of mismatch  |
| Internal Auditor     | Reconciliation controls are undocumented             | Verify control effectiveness |

---

# Why Most Inventory Errors Aren't Judgment Errors

Most inventory failures happen before judgment.

The decision process itself breaks.

## System Failure Points

| Stage                 | Failure                             |
| --------------------- | ----------------------------------- |
| Data Export           | Different cut-off times             |
| Data Cleaning         | SKU inconsistencies                 |
| Data Matching         | Wrong lookup logic                  |
| Financial Translation | Quantity not converted into dollars |
| Exception Review      | No prioritization                   |
| Escalation            | No evidence package                 |

---

## Wrong Workflow

```text
Export CSVs
↓
VLOOKUP everything manually
↓
Spot obvious differences
↓
Discuss discrepancies
↓
Move on
```

---

## Verification Workflow

```text
Synchronize cut-off timestamp
↓
Normalize SKU structure
↓
Cross-system reconciliation
↓
Calculate discrepancy quantities
↓
Translate into financial exposure
↓
Apply SLA thresholds
↓
Generate investigation list
↓
Escalate with evidence
```

---

## Minimum Verification Rules

```text
✓ Same snapshot timestamp

✓ Unique SKU definitions

✓ Explicit discrepancy formulas

✓ Financial impact calculation

✓ Threshold-based alerts

✓ Investigation evidence retained
```

---

# Three Traps That Catch Even Experienced Operators

## Trap 1 — Comparing Different Moments

### Decision Made

"3PL inventory is inaccurate."

---

### Hidden Assumption

Exports occurred at different times.

| System  | Export Time  |
| ------- | ------------ |
| Shopify | Sunday 23:59 |
| WMS     | Monday 00:18 |
| 3PL     | Monday 00:35 |

Orders continued flowing.

---

### Decision Divergence

Wrong conclusion:

> Warehouse error.

Correct conclusion:

> Cut-off inconsistency.

---

### Why It's Wrong

Inventory snapshots represent states.

States must be comparable.

Different timestamps invalidate comparisons.

---

<details>

<summary>Correct Rule</summary>

```text
Only reconcile snapshots captured at identical cut-off times.
```

</details>

---

## Trap 2 — Treating SKU Text as Truth

### Decision Made

"System quantities don't match."

---

### Hidden Cause

SKU formatting differed.

| Shopify | WMS     |
| ------- | ------- |
| abc-001 | ABC-001 |
| SKU123  | SKU123  |
| SKU-55  | SKU-55  |

---

### Decision Divergence

Wrong conclusion:

> Missing inventory.

Correct conclusion:

> Dirty master data.

---

### Why It's Wrong

Identifiers define matching.

Broken identifiers create fake discrepancies.

---

<details>

<summary>Correct Formula</summary>

```excel
=UPPER(TRIM([SKU]))
```

Normalize before matching.

</details>

---

## Trap 3 — Measuring Units Instead of Dollars

### Decision Made

"Only 12 units are missing."

---

### Hidden Metric Error

Unit value ignored.

| SKU | Difference | Unit Cost |   Loss |
| --- | ---------: | --------: | -----: |
| A   |         12 |        $3 |    $36 |
| B   |         12 |       $95 | $1,140 |

---

### Decision Divergence

Wrong conclusion:

> Same severity.

Correct conclusion:

> Prioritize SKU B immediately.

---

### Why It's Wrong

Operational impact is financial.

Counts alone distort priorities.

---

<details>

<summary>Correct Formula</summary>

```excel
=ABS(Difference_Qty) * Unit_Cost
```

</details>

---

# Example Scenario

## Weekly Inventory Review

### Inputs

| SKU   | Shopify | WMS | 3PL | Unit Cost |
| ----- | ------: | --: | --: | --------: |
| SKU-A |     120 | 120 | 118 |        $5 |
| SKU-B |      75 |  73 |  73 |       $20 |
| SKU-C |      40 |  40 |  35 |       $50 |

---

## Calculations

| SKU   | 3PL Difference | WMS Difference | Financial Loss |
| ----- | -------------: | -------------: | -------------: |
| SKU-A |             -2 |              0 |            $10 |
| SKU-B |              0 |             -2 |            $40 |
| SKU-C |             -5 |              0 |           $250 |

---

## Result

| Investigation Priority | SKU   |
| ---------------------- | ----- |
| Critical               | SKU-C |
| Medium                 | SKU-B |
| Low                    | SKU-A |

---

## So What?

Without this process:

> All discrepancies appear equal.

With this process:

> Resources focus where money is actually disappearing.

---

# What The Workbook Actually Delivers (Not How It Calculates)

* Automated cross-system inventory reconciliation
* SKU normalization
* Financial loss quantification
* Top-risk SKU ranking
* Warehouse discrepancy attribution
* 3PL claim evidence preparation
* Threshold-based exception alerts
* Executive dashboard summaries
* Repeatable reconciliation workflow
* Historical reporting capability through saved snapshots

---

# Workbook Logic (For the Skeptical Reviewer)

## Sheet Architecture

```text
Dashboard
│
├─ Config_Master
│
├─ Import_Shopify
│
├─ Import_WMS
│
├─ Import_3PL
│
└─ Calc_Engine
```

---

| Sheet          | Purpose                       |
| -------------- | ----------------------------- |
| Dashboard      | Executive view                |
| Config_Master  | SKU master, costs, thresholds |
| Import_Shopify | Raw Shopify exports           |
| Import_WMS     | Raw WMS exports               |
| Import_3PL     | Raw 3PL exports               |
| Calc_Engine    | Hidden reconciliation logic   |

---

## Design Principles

```text
No VBA.

No external dependencies.

No database setup.

No dynamic-array fragility.

No black-box calculations.
```

---

# Implementation Notes (For Those Who Want to Look Under the Hood)

<details>

<summary>SKU Standardization</summary>

```excel
=UPPER(TRIM(A2))
```

</details>

<details>

<summary>Cross-System Matching</summary>

```excel
=XLOOKUP(
    Standardized_SKU,
    Source_SKU,
    Source_Qty,
    0
)
```

</details>

<details>

<summary>3PL Difference</summary>

```excel
=Shopify_Qty - 3PL_Qty
```

</details>

<details>

<summary>WMS Difference</summary>

```excel
=Shopify_Qty - WMS_Qty
```

</details>

<details>

<summary>Financial Exposure</summary>

```excel
=ABS(Difference_Qty) * Unit_Cost
```

</details>

<details>

<summary>Conditional Alert Logic</summary>

```excel
=OR(
    ABS(Difference_Qty)>=Threshold_Qty,
    ABS(Difference_Qty/Shopify_Qty)>=Threshold_Rate
)
```

</details>

---

# Get The Workbook

Inventory losses rarely begin with theft.

Most begin with uncertainty.

By the time certainty arrives, the claim window often closes.

Download the workbook.

Run the reconciliation.

Preserve the evidence.

```text
Input:
Shopify Export
+ WMS Export
+ 3PL Export

Output:
Operational Truth
```

---

# Limitations

This workbook is intentionally narrow.

It does not attempt to solve every inventory problem.

## What It Does Not Do

* Real-time API synchronization
* ERP integration
* Transportation tracking
* GPS shipment visibility
* Automated claim submission
* Workflow approvals
* Database storage
* Forecasting demand

---

## Dependencies It Assumes

* Consistent SKU definitions
* Shared cut-off timestamps
* Reliable export files
* Accurate unit costs
* Organizational willingness to investigate findings

---

# Other Decision Tools You Might Need

If the problem extends beyond reconciliation:

| Need                            | Appropriate Tool                  |
| ------------------------------- | --------------------------------- |
| Demand forecasting              | Inventory planning model          |
| Transport visibility            | TMS                               |
| Real-time synchronization       | ERP integration                   |
| Warehouse execution             | WMS                               |
| Financial close controls        | Accounting reconciliation toolkit |
| Customer profitability analysis | Margin analysis workbook          |
| Sales concentration risk        | Revenue concentration analysis    |
| Safety stock optimization       | Inventory optimization model      |

---

# License

MIT License.

Permission is granted to use, modify, and distribute this project with attribution.

No warranty is provided.

The workbook assists decision-making.

Responsibility for operational decisions remains with the organization.
