---
title: Goodwill credit
excerpt: >-
  Learn how Goodwill credits work in Recurly RevRec — how they're issued,
  redeemed, voided, and tracked in revenue recognition reports using plan codes.
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
  <div class="rp-overview">Goodwill credit is a complimentary credit balance given to customers as a gesture of goodwill — to acknowledge loyalty, resolve issues, or offer compensation. It can be applied toward purchases, and flows directly into your revenue recognition reports and ERP system for accurate financial tracking.</div>
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
  <li>A cancellation and refund policy that supports account crediting.</li>
</ul>

### Limitations

<ul class="rp-list">
  <li>Goodwill credits are non-transferable and must be used within the issuing account.</li>
  <li>Credits may have expiration dates or usage conditions, depending on your business policy.</li>
</ul>

# Definition

<div class="rp-definition">Goodwill credit is a complimentary credit balance given to customers as a gesture of goodwill. It can be applied toward purchases, facilitating payment adjustments and enhancing customer loyalty. Goodwill credits integrate seamlessly into your ERP system or revenue recognition ecosystem, streamlining reporting and financial tracking.</div>

# Key benefits

<div class="rp-benefits">
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-chart-line" aria-hidden="true"></i></div>
    <strong>Streamlined revenue recognition</strong>
    <span>Incorporating goodwill credits into revenue reports enhances financial accuracy by reflecting real-time customer balances and potential sales.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-file-invoice-dollar" aria-hidden="true"></i></div>
    <strong>Enhanced financial reporting</strong>
    <span>Goodwill credits contribute to a more comprehensive view of financial health, enabling precise revenue tracking and forecasting.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-gears" aria-hidden="true"></i></div>
    <strong>Increased operational efficiency</strong>
    <span>Automated management of goodwill credits simplifies reconciliation and ensures credits are accurately reflected in financial statements.</span>
  </div>
</div>

# Key details

When goodwill credit is allocated, Recurly generates a credit invoice reflecting the credit balance, which can be adjusted against subsequent payments. Credits are recorded as a single line in revenue recognition reports, with redemptions detailed separately — giving you a clear picture of credit usage and its impact on financial health.


<Image src="https://files.readme.io/82c8766-Screenshot_1_2024-03-04_at_4.45.08_PM.png" align="center" width="80%" border={true} />


The following table outlines the identifiers for goodwill credit transactions:

<table class="rp-params">
  <tr class="rp-thead-row"><td>Origin</td><td>Activity</td><td>Plan code</td></tr>
  <tr><td>credit-event</td><td>Goodwill issued</td><td><code>credit-goodwill</code></td></tr>
  <tr><td>credit-event</td><td>Goodwill redeemed</td><td><code>credit-goodwill-redeemed</code></td></tr>
  <tr><td>credit-event</td><td>Goodwill voided</td><td><code>credit-goodwill-voided</code></td></tr>
</table>


<Image src="https://files.readme.io/19cd870-image.png" align="center" width="75%" border={true} />


If goodwill credit is issued erroneously or remains unused, it can be voided — removing the balance from the customer's account. This action, along with all other credit transactions, is recorded in RevRec for comprehensive financial oversight.


<Image src="https://files.readme.io/efb1208-image.png" align="center" width="75%" border={true} />


# FAQ

<Accordion title="How are Goodwill Credits and their usage tracked in RevRec?">
  Goodwill credits appear as distinct lines identified by plan code:

  - **Credit issued:** `credit-goodwill`
  - **Credit used/redeemed:** `credit-goodwill-redeemed`
  - **Credit canceled/voided:** `credit-goodwill-voided`

  Credit-related lines also show origin = credit-event.
</Accordion>

<Accordion title="What happens if a Goodwill Credit is given by mistake or is never used?">
  Void the credit. A voided credit is no longer available to the customer, and RevRec records a reversal line with plan code <code>credit-goodwill-voided</code>.
</Accordion>

<br />
