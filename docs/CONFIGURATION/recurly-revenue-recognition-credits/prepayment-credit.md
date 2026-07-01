---
title: Prepayment credit
excerpt: >-
  Learn how prepayment credits work in Recurly RevRec — how advance payments are
  tracked as a single SO line with two invoices, and how to identify prepayment
  credit activity by plan code.
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---
<div class="rp-page">
  <div class="rp-overview">Prepayment credit is an advance payment made by a customer for future purchases or subscriptions. The credit is stored in the customer's account and automatically applied to invoices as they're generated — simplifying payment and flowing accurately into RevRec for revenue tracking and forecasting.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Available as part of Recurly RevRec</div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#definition"><span class="rp-toc-num">1</span>Definition</a>
    <a class="rp-toc-pill" href="#key-benefits"><span class="rp-toc-num">2</span>Key benefits</a>
    <a class="rp-toc-pill" href="#key-details"><span class="rp-toc-num">3</span>Key details</a>
    <a class="rp-toc-pill" href="#faq"><span class="rp-toc-num">4</span>FAQ</a>
  </div>
</div>

<div class="rp-callout rp-callout-note">
  <div><strong><i class="fa-solid fa-circle-info" aria-hidden="true"></i> Additional cost</strong>To access this feature, you must have an active subscription to either Recurly RevRec or the Standard edition. Contact your Recurly account manager or <a href="mailto:support@recurly.com">support@recurly.com</a> for pricing details.</div>
</div>

### Prerequisites

<ul class="rp-list">
  <li>A cancellation and refund policy that supports prepayment crediting.</li>
</ul>

### Limitations

<ul class="rp-list">
  <li>Prepayment credits can only be used for purchases and can't be refunded.</li>
  <li>Specific configurations may restrict the use of prepayment credits for certain plans or products.</li>
</ul>

# Definition

<div class="rp-definition">Prepayment credit refers to an advance payment made by a customer for purchases or subscriptions. This credit is stored in the customer's account and automatically applied to invoices as they're generated, simplifying the payment process.</div>

# Key benefits

<div class="rp-benefits">
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-chart-line" aria-hidden="true"></i></div>
    <strong>Streamlined revenue recognition</strong>
    <span>Incorporating prepayment credits into revenue reports enhances financial accuracy by reflecting real-time customer balances and potential sales.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-file-invoice-dollar" aria-hidden="true"></i></div>
    <strong>Enhanced financial reporting</strong>
    <span>Prepayment credits contribute to a more comprehensive view of financial health, enabling precise revenue tracking and forecasting.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-gears" aria-hidden="true"></i></div>
    <strong>Increased operational efficiency</strong>
    <span>Automated management of prepayment credits simplifies reconciliation and ensures credits are accurately reflected in financial statements.</span>
  </div>
</div>

# Key details

When a customer makes a prepayment, Recurly issues two invoices: one acknowledging the payment and one representing the credit balance.

**Payment invoice**


<Image src="https://files.readme.io/41591a7-image.png" align="center" width="80%" border={true} />


**Credit invoice**


<Image src="https://files.readme.io/9ed19d1-image.png" align="center" width="80%" border={true} />


Prepayment credits appear in RevRec as a single Sales Order (SO) line with two invoices. Adjustments to the credit are recorded as new lines, identifiable by their origin and plan code.

<table class="rp-params">
  <tr class="rp-thead-row"><td>Origin</td><td>Activity</td><td>Plan code</td></tr>
  <tr><td>credit-event</td><td>Prepayment credit issued</td><td><code>credit-prepayment</code></td></tr>
  <tr><td>credit-event</td><td>Prepayment credit redeemed</td><td><code>credit-prepayment-redeemed</code></td></tr>
  <tr><td>credit-event</td><td>Prepayment credit voided</td><td><code>credit-prepayment-voided</code></td></tr>
</table>


<Image src="https://files.readme.io/00ce3ca-image.png" align="center" width="75%" border={true} />


Customers can view their total credit balance in Recurly — equal to the total sell price of the credit lines — in the customer information section.


<Image src="https://files.readme.io/0a9446b-image.png" align="center" width="45%" border={true} />


# FAQ

<Accordion title="What makes a prepayment credit different from the other two credit types?">
  A prepayment credit is funded by the customer. They pay in advance, and that amount is held as a credit balance to use on future subscriptions or purchases.
</Accordion>

<Accordion title="Why do I see two credit-event invoices in Recurly when a prepayment credit is issued?">
  Two invoices are created to make the accounting clear:

  - **Payment invoice:** Acknowledges receipt of the customer's advance payment.
  - **Credit invoice:** Converts that payment into a usable credit balance on the customer's account.
</Accordion>

<Accordion title="How are prepayment credits and their adjustments tracked in RevRec?">
  Filter for origin = credit-event and use these plan codes:

  - **Credit issued:** `credit-prepayment`
  - **Credit used/redeemed:** `credit-prepayment-redeemed`
  - **Credit canceled/voided:** `credit-prepayment-voided`
</Accordion>

<br />
