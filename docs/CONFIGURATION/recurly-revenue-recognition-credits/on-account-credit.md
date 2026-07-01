---
title: On-account credit
excerpt: >-
  Learn how on-account credits work in Recurly RevRec — how they're issued when
  subscriptions are canceled, redeemed, voided, and tracked in revenue
  recognition reports using plan codes.
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
  <div class="rp-overview">On-account credit is a balance credited to a customer's account instead of a direct refund — typically when a subscription is canceled and the customer is eligible for a refund. The credit can be applied toward future purchases and flows directly into Recurly RevRec reports for accurate financial tracking.</div>
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
  <li>On-account credits are non-transferable between accounts.</li>
  <li>Credits may be subject to expiration per your business's terms and conditions.</li>
</ul>

# Definition

<div class="rp-definition">On-account credit in Recurly refers to a balance credited to a customer's account instead of a direct refund. This occurs when a customer cancels a subscription and is eligible for a refund — rather than returning the money to the original source, Recurly credits the account, which can then be applied toward future purchases. These credits are accurately reflected in Recurly RevRec reports.</div>

# Key benefits

<div class="rp-benefits">
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-chart-line" aria-hidden="true"></i></div>
    <strong>Streamlined revenue recognition</strong>
    <span>Incorporating on-account credits into revenue reports enhances financial accuracy by reflecting real-time customer balances and potential sales.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-file-invoice-dollar" aria-hidden="true"></i></div>
    <strong>Enhanced financial reporting</strong>
    <span>On-account credits contribute to a more comprehensive view of financial health, enabling precise revenue tracking and forecasting.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-gears" aria-hidden="true"></i></div>
    <strong>Increased operational efficiency</strong>
    <span>Automated management of on-account credits simplifies reconciliation and ensures credits are accurately reflected in financial statements.</span>
  </div>
</div>

# Key details

When a customer's subscription is canceled and a refund is due, Recurly can credit the account instead of issuing a direct refund. That on-account credit can then be used for any purchases within Recurly's platform.

Upon issuing an on-account credit, Recurly generates a credit invoice reflecting the credited amount and any subsequent redemptions. The invoice updates to show the remaining balance over time, providing transparency for both the customer and your business.

Credits and their redemptions are recorded in RevRec as distinct entries, categorized by origin (`credit-event`) and identified by unique plan codes for easy reconciliation.


<Image src="https://files.readme.io/8ed64f5-image.png" align="center" width="80%" border={true} />


<table class="rp-params">
  <tr class="rp-thead-row"><td>Origin</td><td>Activity</td><td>Plan code</td></tr>
  <tr><td>credit-event</td><td>On-account credit issued</td><td><code>credit-on-account</code></td></tr>
  <tr><td>credit-event</td><td>On-account credit redeemed</td><td><code>credit-on-account-redeemed</code></td></tr>
  <tr><td>credit-event</td><td>On-account credit voided</td><td><code>credit-voided</code></td></tr>
  <tr><td>credit-event</td><td>On-account credit refunded</td><td><code>credit-paid</code></td></tr>
</table>


<Image src="https://files.readme.io/ccb7b62-image.png" align="center" width="75%" border={true} />


# FAQ

<Accordion title="How is an on-account credit created in the billing system?">
  When an on-account credit is issued, Recurly creates a credit invoice showing the initial credit amount. As the credit is redeemed, the invoice reflects the remaining balance over time.
</Accordion>

<Accordion title="How can I differentiate on-account credit activities in RevRec?">
  Filter by origin = credit-event and use these plan codes to identify each activity:

  - **Credit issued:** `credit-on-account`
  - **Credit used/redeemed:** `credit-on-account-redeemed`
  - **Credit canceled/voided:** `credit-voided`
  - **Credit refunded (paid out as cash):** `credit-paid`
</Accordion>

<br />
