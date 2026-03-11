---
title: Dashboard
excerpt: >-
  Monitor revenue health, deferred balances, and audit-ready metrics in one
  view.
deprecated: false
hidden: false
metadata:
  robots: index
---
# Overview

The Revenue Recognition Dashboard gives finance teams a centralized, real-time view of revenue performance, deferred balances, and compliance-related metrics. It helps CFOs, Controllers, Analysts, and other finance stakeholders review revenue health, validate data integrity, and make informed decisions from a single interface.

# Key benefits

* **Real-time visibility**: Dashboard tiles update continuously to reflect the latest financial data.
* **Revenue waterfall insight:** Track beginning balances, new billings, recognized revenue, and ending balances for any selected period
* **Audit-ready validation**: Compare dashboard totals against supporting views, such as the Liability Balance Rollforward and General Ledger.

# Key details

## Open the dashboard

**Select** the dashboard icon in the Revenue Recognition menu bar.

<Image align="center" border={true} src="https://files.readme.io/392a120d1642141a30b0537dd9eba05a8cc52050d112d63391a44b363f01e1d5-Img_1.png" className="border" />

The Revenue Recognition Dashboard turns complex transactional data into a clear, audit-ready reporting interface. It helps your team:

| Strategic value              | Description                                                                                                                  |
| :--------------------------- | :--------------------------------------------------------------------------------------------------------------------------- |
| Unified financial visibility | Consolidates billings, recognized revenue, and deferred balances into one source of truth.                                   |
| Audit readiness              | Helps reconcile dashboard values with the Liability Balance Rollforward and the General Ledger, reducing month-end friction. |
| Lifecycle tracking           | Shows how revenue moves from initial billing through final recognition.                                                      |

## Dashboard components

The dashboard includes two main sections:

| Section                       | Description                                                                                                     |
| :---------------------------- | :-------------------------------------------------------------------------------------------------------------- |
| Revenue Metrics               | Interactive tiles that provide a high-level view of revenue performance for the selected timeframe.             |
| Liability Balance Rollforward | A detailed view of how deferred revenue moves from beginning balance to ending balance for the selected period. |

## Revenue metrics

The Revenue Metrics section provides a centralized view of revenue-related activity. Use the filters at the top of the dashboard to customize what you see.

<Image align="center" border={true} src="https://files.readme.io/b6dfefbfb1a626cbf74f58420adbdc589bc1fecedbef79e7f6cf0f2879d2e925-Img_2.png" className="border" />

### Revenue metrics filters

| Filter             | Description                                                                                                                                                                           |
| :----------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Accounting period  | Select a period, such as Jan-26 or Feb-25, to display data for that timeframe. The dashboard defaults to the current open period, and the latest period stays at the top of the list. |
| Currency type      | View data in Transactional, Entity (Company), or Reporting (Global) currency.                                                                                                         |
| Currency selection | Select a specific currency to review totals for that currency only.                                                                                                                   |
| Accounting book    | Choose the accounting book, such as ASC 606 or Non-GAAP, that should be used as the data source.                                                                                      |

> **Note:** Currency filters display raw totals for the selected currency only. The dashboard does not convert values or apply exchange rates.

### Drill down into a metric

Each metric tile supports drill-down reporting. **Select** the drill-down icon on a tile to open the detailed transaction lines behind that total, including supporting transaction data such as customer names and invoice IDs.

<Image align="center" border={true} src="https://files.readme.io/512204060f2406acf8f9c948d8a0b6fc65b034a7e8f2bf17495d94975b63d97f-Img_3.png" className="border" />

### Revenue metric tiles

| Tile                           | What it shows                                                                                                                                    | Example                                                                                                                                                          | Audit note                                                                                                                                                                           |
| :----------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Current Period Billings        | The gross invoice value for all invoices with a Bill Date in the selected period. This includes subscriptions, one-time charges, and setup fees. | A customer signs up on March 15 for a $1,200 annual plan. Even though only part of that amount is earned in March, the tile shows $1,200 for March.              | This should match the Billing Transaction Details Report.                                                                                                                            |
| Deferred Revenue Balance       | The ending deferred revenue liability as of the last day of the selected period.                                                                 | A customer pays $120 on December 31 for a 12-month subscription starting January 1. After $10 is recognized in January, the Deferred Revenue Balance shows $110. | This should match the Ending Balance in the Liability Balance Rollforward.                                                                                                           |
| Revenue from Unbilled Services | Revenue recognized for delivered services that have not yet been billed.                                                                         | A $1,200 subscription uses an Upon Booking release setup, but only $800 has been invoiced so far. The remaining $400 appears here.                               | This value is the sum of the Asset Balances Report and the Unbilled Balances Report. The unbilled balance appears only when the unbilled flag is set to Y for the subscription line. |
| Refunds and Adjustments        | Credit memos, voided invoices, refunds, and similar transactions that reduce billings or recognized revenue.                                     | A customer is overcharged $100 in February, and a credit memo is issued in March. The tile shows -$100 in March.                                                 | This metric reflects contra-revenue activity processed during the selected accounting period.                                                                                        |
| Current Billing Revenue        | Revenue from invoices created in the current period that is also recognized in the same period.                                                  | A monthly subscription for $30 is billed on April 1 and fully earned by April 30. The tile shows $30 for April.                                                  | This can be validated by reviewing Revenue Waterfall data where the Invoice Date and Invoice Start Date fall within the same reporting period.                                       |
| Deferred Revenue Recognized    | Revenue released in the current period from deferred balances created in prior periods.                                                          | A customer paid for an annual plan in January. In August, one monthly portion of that payment is recognized and appears in this tile.                            | This represents revenue released from previously recorded deferred revenue liability.                                                                                                |
| Total Revenue Recognized       | Total revenue earned during the selected period, regardless of when billing occurred.                                                            | In October, you recognize $100 from current billings, $500 from prior deferred revenue, and $400 from unbilled services. Total Revenue Recognized is $1,000.     | This should equal: Current Billing Revenue + Deferred Revenue Recognized + Revenue from Unbilled Services.                                                                           |

## Liability balance rollforward

The Liability Balance Rollforward is the audit engine of the dashboard. It shows how deferred revenue moves from the beginning to the end of a selected period, quarter, or year. This view helps confirm that every billed amount is either recognized as revenue or remains recorded as a liability.

<Image align="center" border={true} src="https://files.readme.io/5ce4c64f258bbd7dd90ad656f6b8a666e52539c4eb3ccbc98125c1ece04faf54-Img_4.png" className="border" />

### Rollforward filters

| Filter             | Description                                                                                |
| :----------------- | :----------------------------------------------------------------------------------------- |
| Year or period     | Select a year, such as 2024 or 2025, to display all closed and open periods for that year. |
| Summarization      | View balances by Period, Quarter, or Year.                                                 |
| Currency type      | Review values in Transactional, Company, or Reporting currency.                            |
| Currency selection | Select a specific currency to display totals for that currency only.                       |
| Accounting book    | Choose the accounting book used as the source for dashboard values.                        |

> **Note:** Currency filters display raw totals for the selected currency only. The system does not perform currency conversion in this view.

### How the rollforward works

The rollforward follows this accounting logic:

**Beginning Balance + New Billings - Revenue Recognized = Ending Balance**

This structure helps your team reconcile deferred revenue activity directly against the General Ledger and support compliance with ASC 606 and IFRS 15.

### Rollforward columns

| Column             | Description                                                                                                           | Example                                                                                                          |
| :----------------- | :-------------------------------------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------- |
| Beginning Balance  | Deferred revenue carried over from the previous period.                                                               | If December ends with $50,000 in deferred revenue, January begins with $50,000.                                  |
| New Billings       | New invoices and charges created during the selected period.                                                          | If ten annual contracts worth $120,000 are billed in Q1, that amount appears as New Billings.                    |
| Revenue Recognized | Revenue earned during the selected period and released from the balance sheet to the income statement.                | If $10,000 of deferred revenue is earned in January, that amount appears here.                                   |
| Ending Balance     | Deferred revenue remaining at the end of the selected period. This becomes the Beginning Balance for the next period. | Start with $50,000, add $20,000 in new billings, and subtract $15,000 in recognized revenue to end with $55,000. |
