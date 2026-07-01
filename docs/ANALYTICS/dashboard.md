---
title: Dashboard
excerpt: >-
  The Revenue Recognition Dashboard gives finance teams a real-time view of
  revenue performance, deferred balances, and audit-ready compliance metrics in
  one place.
deprecated: false
hidden: false
metadata:
  robots: index
---
<div class="rp-page">
  <div class="rp-overview">The Revenue Recognition Dashboard gives finance teams a centralized, real-time view of revenue performance, deferred balances, and compliance metrics. CFOs, controllers, analysts, and other stakeholders can review revenue health, validate data integrity, and make informed decisions from a single interface — without stitching together separate reports.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Part of Recurly RevRec — <a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-advanced" target="_blank">learn more</a></div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#key-benefits"><span class="rp-toc-num">1</span>Key benefits</a>
    <a class="rp-toc-pill" href="#open-the-dashboard"><span class="rp-toc-num">2</span>Open the dashboard</a>
    <a class="rp-toc-pill" href="#dashboard-components"><span class="rp-toc-num">3</span>Dashboard components</a>
    <a class="rp-toc-pill" href="#revenue-metrics"><span class="rp-toc-num">4</span>Revenue metrics</a>
    <a class="rp-toc-pill" href="#liability-balance-rollforward"><span class="rp-toc-num">5</span>Liability Balance Rollforward</a>
  </div>
</div>

<div style={{position: "relative", paddingTop: "56.25%", marginBottom: "28px", borderRadius: "10px", overflow: "hidden"}}>
  <iframe src="https://fast.wistia.net/embed/iframe/113oukv0ec"
    title="Revenue Recognition Dashboard"
    allow="autoplay; fullscreen"
    allowtransparency="true"
    frameBorder="0"
    scrolling="no"
    allowFullScreen
    style={{position: "absolute", top: 0, left: 0, width: "100%", height: "100%", border: "none"}}></iframe>
</div>

# Key benefits

<div class="rp-benefits">
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-bolt" aria-hidden="true"></i></div>
    <strong>Real-time visibility</strong>
    <span>Dashboard tiles update continuously to reflect the latest financial data.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-water" aria-hidden="true"></i></div>
    <strong>Revenue waterfall insight</strong>
    <span>Track beginning balances, new billings, recognized revenue, and ending balances for any selected period.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-clipboard-check" aria-hidden="true"></i></div>
    <strong>Audit-ready validation</strong>
    <span>Compare dashboard totals against supporting views like the Liability Balance Rollforward and General Ledger.</span>
  </div>
</div>

# Open the dashboard

Select the dashboard icon in the Revenue Recognition menu bar.


<Image src="https://files.readme.io/392a120d1642141a30b0537dd9eba05a8cc52050d112d63391a44b363f01e1d5-Img_1.png" align="center" width="75%" border={true} />


The dashboard turns complex transactional data into a clear, audit-ready reporting interface that helps your team in three ways:

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Strategic value</td><td>Description</td></tr>
  <tr><td>Unified financial visibility</td><td>Consolidates billings, recognized revenue, and deferred balances into one source of truth.</td></tr>
  <tr><td>Audit readiness</td><td>Helps reconcile dashboard values with the Liability Balance Rollforward and the General Ledger, reducing month-end friction.</td></tr>
  <tr><td>Lifecycle tracking</td><td>Shows how revenue moves from initial billing through final recognition.</td></tr>
</table>

# Dashboard components

The dashboard has two main sections.

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Section</td><td>Description</td></tr>
  <tr><td>Revenue Metrics</td><td>Interactive tiles that provide a high-level view of revenue performance for the selected timeframe.</td></tr>
  <tr><td>Liability Balance Rollforward</td><td>A detailed view of how deferred revenue moves from beginning balance to ending balance for the selected period.</td></tr>
</table>

# Revenue metrics

The Revenue Metrics section provides a centralized view of revenue-related activity. Use the filters at the top of the dashboard to customize what you see.


<Image src="https://files.readme.io/b6dfefbfb1a626cbf74f58420adbdc589bc1fecedbef79e7f6cf0f2879d2e925-Img_2.png" align="center" width="75%" border={true} />


## Revenue metrics filters

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Filter</td><td>Description</td></tr>
  <tr><td>Accounting period</td><td>Select a period, such as Jan-26 or Feb-25, to display data for that timeframe. The dashboard defaults to the current open period, and the latest period stays at the top of the list.</td></tr>
  <tr><td>Currency type</td><td>View data in Transactional, Entity (Company), or Reporting (Global) currency.</td></tr>
  <tr><td>Currency selection</td><td>Select a specific currency to review totals for that currency only.</td></tr>
  <tr><td>Accounting book</td><td>Choose the accounting book, such as ASC 606 or Non-GAAP, that should be used as the data source.</td></tr>
</table>

<div class="rp-callout rp-callout-note">
  <div><strong><i class="fa-solid fa-circle-info" aria-hidden="true"></i> Note</strong>Currency filters display raw totals for the selected currency only. The dashboard doesn't convert values or apply exchange rates.</div>
</div>

## Drill down into a metric

Each metric tile supports drill-down reporting. Select the drill-down icon on a tile to open the detailed transaction lines behind that total, including supporting data such as customer names and invoice IDs.


<Image src="https://files.readme.io/512204060f2406acf8f9c948d8a0b6fc65b034a7e8f2bf17495d94975b63d97f-Img_3.png" align="center" width="75%" border={true} />


## Revenue metric tiles

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Tile</td><td>What it shows</td><td>Example</td><td>Audit note</td></tr>
  <tr><td>Current Period Billings</td><td>The gross invoice value for all invoices with a bill date in the selected period, including subscriptions, one-time charges, and setup fees.</td><td>A customer signs up on March 15 for a $1,200 annual plan. Even though only part of that amount is earned in March, the tile shows $1,200 for March.</td><td>Should match the Billing Transaction Details Report.</td></tr>
  <tr><td>Deferred Revenue Balance</td><td>The ending deferred revenue liability as of the last day of the selected period.</td><td>A customer pays $120 on December 31 for a 12-month subscription starting January 1. After $10 is recognized in January, the balance shows $110.</td><td>Should match the ending balance in the Liability Balance Rollforward.</td></tr>
  <tr><td>Revenue from Unbilled Services</td><td>Revenue recognized for delivered services that haven't yet been billed.</td><td>A $1,200 subscription uses an Upon Booking release setup, but only $800 has been invoiced so far. The remaining $400 appears here.</td><td>This value is the sum of the Asset Balances Report and the Unbilled Balances Report. The unbilled balance appears only when the unbilled flag is set to Y for the subscription line.</td></tr>
  <tr><td>Refunds and Adjustments</td><td>Credit memos, voided invoices, refunds, and similar transactions that reduce billings or recognized revenue.</td><td>A customer is overcharged $100 in February, and a credit memo is issued in March. The tile shows -$100 in March.</td><td>Reflects contra-revenue activity processed during the selected accounting period.</td></tr>
  <tr><td>Current Billing Revenue</td><td>Revenue from invoices created in the current period that is also recognized in the same period.</td><td>A monthly subscription for $30 is billed on April 1 and fully earned by April 30. The tile shows $30 for April.</td><td>Validate by reviewing revenue waterfall data where the invoice date and invoice start date fall within the same reporting period.</td></tr>
  <tr><td>Deferred Revenue Recognized</td><td>Revenue released in the current period from deferred balances created in prior periods.</td><td>A customer paid for an annual plan in January. In August, one monthly portion of that payment is recognized and appears in this tile.</td><td>Represents revenue released from previously recorded deferred revenue liability.</td></tr>
  <tr><td>Total Revenue Recognized</td><td>Total revenue earned during the selected period, regardless of when billing occurred.</td><td>In October, you recognize $100 from current billings, $500 from prior deferred revenue, and $400 from unbilled services. Total Revenue Recognized is $1,000.</td><td>Should equal Current Billing Revenue + Deferred Revenue Recognized + Revenue from Unbilled Services.</td></tr>
</table>

# Liability Balance Rollforward

The Liability Balance Rollforward is the audit engine of the dashboard. It shows how deferred revenue moves from the beginning to the end of a selected period, quarter, or year — confirming that every billed amount is either recognized as revenue or remains recorded as a liability.


<Image src="https://files.readme.io/5ce4c64f258bbd7dd90ad656f6b8a666e52539c4eb3ccbc98125c1ece04faf54-Img_4.png" align="center" width="75%" border={true} />


## Rollforward filters

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Filter</td><td>Description</td></tr>
  <tr><td>Year or period</td><td>Select a year, such as 2024 or 2025, to display all closed and open periods for that year.</td></tr>
  <tr><td>Summarization</td><td>View balances by Period, Quarter, or Year.</td></tr>
  <tr><td>Currency type</td><td>Review values in Transactional, Company, or Reporting currency.</td></tr>
  <tr><td>Currency selection</td><td>Select a specific currency to display totals for that currency only.</td></tr>
  <tr><td>Accounting book</td><td>Choose the accounting book used as the source for dashboard values.</td></tr>
</table>

<div class="rp-callout rp-callout-note">
  <div><strong><i class="fa-solid fa-circle-info" aria-hidden="true"></i> Note</strong>Currency filters display raw totals for the selected currency only. The system doesn't perform currency conversion in this view.</div>
</div>

## How the rollforward works

The rollforward follows this accounting logic:

<div class="rp-callout rp-callout-tip">
  <div><strong><i class="fa-solid fa-lightbulb" aria-hidden="true"></i> Formula</strong>Beginning Balance + New Billings − Revenue Recognized = Ending Balance</div>
</div>

This structure helps your team reconcile deferred revenue activity directly against the General Ledger and supports compliance with ASC 606 and IFRS 15.

## Rollforward columns

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Column</td><td>Description</td><td>Example</td></tr>
  <tr><td>Beginning Balance</td><td>Deferred revenue carried over from the previous period.</td><td>If December ends with $50,000 in deferred revenue, January begins with $50,000.</td></tr>
  <tr><td>New Billings</td><td>New invoices and charges created during the selected period.</td><td>If ten annual contracts worth $120,000 are billed in Q1, that amount appears as New Billings.</td></tr>
  <tr><td>Revenue Recognized</td><td>Revenue earned during the selected period and released from the balance sheet to the income statement.</td><td>If $10,000 of deferred revenue is earned in January, that amount appears here.</td></tr>
  <tr><td>Ending Balance</td><td>Deferred revenue remaining at the end of the selected period. This becomes the beginning balance for the next period.</td><td>Start with $50,000, add $20,000 in new billings, and subtract $15,000 in recognized revenue to end with $55,000.</td></tr>
</table>

<br />
