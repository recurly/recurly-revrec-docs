---
title: Payments
deprecated: false
hidden: false
metadata:
  robots: index
---
Title: Payments
Metadata description: How RevRec's Payment Integration syncs cash receipts, manual payments, and credits from RSM in real time, and how to set it up.

\---PASTE INTO EDITOR BELOW---

<div class="rp-page">
  <div class="rp-overview">This page walks you through Recurly's Payment Integration for Revenue Recognition (RevRec) — how it captures cash receipts, manual payments, and on-account credits in real time, and what changes once you turn it on. You'll find the setup steps, the new Payments tab in the Revenue Workbench, and a full reference for the journal entries the system generates automatically.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Available on all Recurly plans</div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#definition"><span class="rp-toc-num">1</span>Definition</a>
    <a class="rp-toc-pill" href="#key-benefits"><span class="rp-toc-num">2</span>Key benefits</a>
    <a class="rp-toc-pill" href="#how-it-works"><span class="rp-toc-num">3</span>How it works</a>
    <a class="rp-toc-pill" href="#setup"><span class="rp-toc-num">4</span>Setup</a>
    <a class="rp-toc-pill" href="#what-changes-after-activation"><span class="rp-toc-num">5</span>What changes after activation</a>
    <a class="rp-toc-pill" href="#data-flow-architecture"><span class="rp-toc-num">6</span>Data flow architecture</a>
    <a class="rp-toc-pill" href="#journal-entry-reference"><span class="rp-toc-num">7</span>Journal entry reference</a>
  </div>
</div>

# Definition

<div class="rp-definition">The RevRec Payment Integration automatically captures, records, and accounts for every cash receipt, manual payment, and on-account credit in Recurly RevRec. Before this integration, only billed and invoiced revenue synced to RevRec — cash events stayed outside the system, so finance teams built journal entries and reconciled everything by hand. This integration closes that gap by bringing cash event data into RevRec in real time.</div>

# Key benefits

<div class="rp-benefits">
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-clock" aria-hidden="true"></i></div>
    <strong>Reduced monthly close time</strong>
    <span>Skip the manual reconciliation — teams typically cut their monthly close cycle by 30–50%, freeing up time for higher-value work.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-bolt" aria-hidden="true"></i></div>
    <strong>Real-time journal entry creation</strong>
    <span>Journal entries generate within seconds of payment confirmation, so your financial records always reflect the latest transaction activity.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-shield-halved" aria-hidden="true"></i></div>
    <strong>Audit-ready, compliant records</strong>
    <span>Every journal entry and payment record follows ASC 606 and IFRS 15 standards, giving you reliable, audit-ready documentation at all times.</span>
  </div>
</div>

# How it works

Payment Integration builds a real-time data pipeline between Recurly Subscription Management (RSM) and RevRec, so payment events move between the two systems without manual intervention. When a payment event happens in RSM — a gateway charge, a manual payment, a credit application, or a refund — RevRec automatically runs through this sequence:

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Payment ingestion & association</h4><p>RevRec ingests the payment confirmation and links it to the invoice and charge lines it belongs to.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Validation & account mapping</h4><p>The transaction is validated and mapped to the correct chart-of-account codes for consistent GL categorization.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Journal entry generation</h4><p>Compliant double-entry journal entries post automatically, based on applicable accounting standards — no manual entry required.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>AR subledger & roll-forward update</h4><p>The Accounts Receivable (AR) subledger and roll-forward balances update immediately, keeping downstream reporting accurate and reconciled.</p></div>
  </div>
</div>

# Setup

## Activating Payment Integration

<div class="rp-callout rp-callout-note">
  <div><strong><i class="fa-solid fa-circle-info" aria-hidden="true"></i> Note</strong>Admin access required. Only users with RevRec admin permissions can enable this feature flag. Contact your system administrator if you don't have access to the RevRec Admin window.</div>
</div>

Payment Integration is a feature flag you enable from the RevRec Admin window.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open the RevRec Admin window</h4><p>Log in to RevRec and navigate to the RevRec Admin window.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Locate the feature flag</h4><p>Find Payment Integration in the feature settings section.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Enable the flag</h4><p>Toggle the feature flag to Enabled.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Save your changes</h4><p>Once you save, RevRec starts syncing payment events from RSM in real time.</p></div>
  </div>
</div>

Next, configure the two core components below to complete setup.

## Configure segmentation and your dataset

### A. Segmentation

Navigate to the RevRec segment configuration section. Payment Sync introduces two new segments you'll need to configure:

<div class="rp-card">

### Cash segment

Define the GL account code for cash receipts and outflows. This segment is debited when a payment is received and credited when a refund is issued.

</div>

<div class="rp-card">

### AR segment

Define the GL account code for accounts receivable. This segment is debited when an invoice is created and credited when a payment is received.

</div>


<Image src="https://files.readme.io/401d5e1a29d17b7153e98595dbff18996eb8c36b2380a9fc43a9ac731e2425da-image.png" align="center" width="75%" border={true} />


### B. Dataset configuration

Configure the dataset RevRec uses to ingest payment data from RSM. This includes mapping RSM payment fields to RevRec accounting fields — verify that every required payment data field is mapped correctly before moving on.

# What changes after activation

Once the Payment Integration flag is enabled, two things become visible in the system.

## Payment Integration scheduled job

A new job called "Payment Integration" appears under Scheduled Jobs (Import/Export → Scheduled Jobs). This job manages the ongoing sync of payment events from RSM into RevRec.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Go to Scheduled Jobs</h4><p>Navigate to Import/Export → Scheduled Jobs.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Run the Payment Integration job</h4><p>Existing invoices and payment events begin flowing into RevRec.</p></div>
  </div>
</div>

{/* TODO: Add screenshot of the Payment Integration scheduled job */}

## Payments tab — Revenue Workbench

A new Payments tab has been added to the Revenue Workbench, giving you invoice-level visibility into all payment activity. This tab consolidates key payment details into a single view, so you can quickly review how payments are being processed and recorded.


<Image src="https://files.readme.io/8912769957bb24ddf9e292dfed5525742ee0b99497ec827e5286d1d3982d837d-image.png" align="center" width="75%" border={true} />


<table class="rp-params">
  <tr class="rp-thead-row"><td>Field</td><td>Description</td></tr>
  <tr><td>Payment Type</td><td>Identifies the nature of the payment transaction — Credit Card (CR) for card payments, or Credit (CA) for payments made through a credit.</td></tr>
  <tr><td>Payment Method</td><td>Provides additional detail on how the payment was fulfilled — through a credit card transaction or a credit payment.</td></tr>
  <tr><td>Gateway Type</td><td>Indicates the payment gateway the transaction was routed through, useful for tracking which gateway was used when multiple are configured.</td></tr>
  <tr><td>Payment Date</td><td>Shows the date the payment was completed and recorded, so you can track timelines and reconcile against invoice due dates.</td></tr>
  <tr><td>Amount</td><td>Shows the total monetary value paid or credited for the invoice, reflecting the actual amount received for accurate revenue tracking.</td></tr>
</table>

# Data flow architecture

Here's how a payment event moves from RSM through RevRec to your General Ledger and ERP:

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Stage</td><td>Trigger</td><td>System</td><td>Action</td><td>Output</td></tr>
  <tr><td>1. Subscription event</td><td>New subscription, renewal, or upgrade</td><td>RSM</td><td>Creates and publishes invoice</td><td>Invoice sent to RevRec</td></tr>
  <tr><td>2. Payment initiated</td><td>Customer makes payment</td><td>Payment gateway</td><td>Processes and confirms the transaction</td><td>Payment confirmation sent to RSM</td></tr>
  <tr><td>3. Payment recorded</td><td>Gateway confirmation received</td><td>RSM</td><td>Records payment, updates invoice status to "Paid"</td><td>Status change published to RevRec</td></tr>
  <tr><td>4. Cash receipt entry</td><td>Invoice status = "Paid"</td><td>RevRec</td><td>Generates cash receipt journal entry instantly</td><td>Dr: Cash<br/>Cr: AR</td></tr>
  <tr><td>5. Revenue recognition</td><td>Performance obligation fulfilled</td><td>RevRec</td><td>Releases deferred revenue to recognized revenue</td><td>Dr: Deferred Revenue<br/>Cr: Revenue</td></tr>
  <tr><td>6. GL export</td><td>Journals posted in RevRec</td><td>RevRec → GL</td><td>Journals exported to the General Ledger</td><td>Entries reflected in financial statements</td></tr>
  <tr><td>7. ERP sync</td><td>GL updated</td><td>GL → ERP</td><td>GL data consumed by the merchant's external ERP</td><td>Full financial records updated (e.g., NetSuite, SAP)</td></tr>
</table>


<Image src="https://files.readme.io/9bbe8365de12b3d852b8e387f58b80084306230adf297ac154b3e772e66fc264-image.png" align="center" width="75%" border={true} />


<div class="rp-callout rp-callout-note">
  <div><strong><i class="fa-solid fa-circle-info" aria-hidden="true"></i> Note</strong>Stage 1 happens at invoice creation, before any cash moves. Stages 2–4 happen at payment confirmation, triggered by the "Paid" status change — not by invoice creation. Stage 5 is independent of cash timing; revenue is recognized when the obligation is fulfilled, not when payment arrives. Stages 6–7 are downstream of RevRec and occur after journals are posted.</div>
</div>

# Journal entry reference

This table shows the debit/credit pair RevRec posts for each payment event.

<table class="rp-params">
  <tr class="rp-thead-row"><td>Payment event</td><td>Debit</td><td>Credit</td><td>Description</td></tr>
  <tr><td>Invoice created</td><td>Accounts Receivable (AR)</td><td>Deferred Revenue</td><td>ASC 606 requires revenue to be deferred until the performance obligation is fulfilled. AR opens; revenue holds in deferred status.</td></tr>
  <tr><td>Obligation delivered</td><td>Deferred Revenue</td><td>Revenue</td><td>When the performance obligation is fulfilled, deferred revenue releases to the income statement as recognized revenue.</td></tr>
  <tr><td>Payment received</td><td>Cash</td><td>Accounts Receivable (AR)</td><td>When payment is confirmed and invoice status = Paid, cash is recognized and the outstanding AR balance reduces accordingly.</td></tr>
  <tr><td>Refund issued</td><td>Accounts Receivable (AR)</td><td>Cash</td><td>The original payment entry fully reverses. AR restores to reflect the outstanding balance; cash reduces by the refund amount.</td></tr>
  <tr><td>Refund / write-off (step 1)</td><td>Revenue</td><td>Deferred Revenue</td><td>Previously recognized revenue reverses back to deferred status in preparation for the AR credit.</td></tr>
  <tr><td>Refund / write-off (step 2)</td><td>Deferred Revenue</td><td>Accounts Receivable (AR)</td><td>Deferred revenue applies to clear the AR balance, closing the full cycle of invoice creation, recognition, and refund.</td></tr>
</table>

## Detailed journal entry explanations

<div class="rp-card">

### Cash receipt — payment received

**Trigger:** A payment is successfully applied to an invoice and the invoice status changes to "Paid" in RSM.

**Debit:** Cash (amount equal to payment received)
**Credit:** Accounts Receivable — AR (same amount)

**Effect on AR:** Reduces the open AR balance by the payment amount.
**Effect on Cash:** Increases the Cash account balance by the payment amount.

When a payment is confirmed, RevRec recognizes the incoming cash and reduces the outstanding AR balance accordingly. This entry closes the receivable for the amount paid and records the cash inflow. For a partial payment, only the paid portion clears from AR — the remainder stays open as a receivable.

</div>

<div class="rp-card">

### Refund — payment returned

**Trigger:** A refund is issued in RSM against a previously paid invoice.

**Debit:** Accounts Receivable — AR (amount equal to refund issued)
**Credit:** Cash (same amount)

**Effect on AR:** Restores the AR balance — the receivable reopens.
**Effect on Cash:** Reduces the Cash account balance by the refund amount.

When a refund is issued, RevRec reverses the original cash receipt entry. The AR balance restores to reflect the outstanding amount, and cash reduces. This entry always mirrors the original payment entry for the refunded amount.

</div>
