---
title: Credits
excerpt: >-
  Overview of Recurly RevRec credit types — Goodwill, On-account, and Prepayment
  credits — including how to configure credit event inclusion in revenue
  recognition and how credits appear in RevRec.
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
  <div class="rp-overview">Recurly RevRec supports three types of credits — Goodwill, On-account, and Prepayment — each serving a distinct purpose in your revenue recognition workflows. Use this page to understand the credit types, configure whether credit event transactions flow into RevRec, and navigate to each dedicated guide.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Available as part of Recurly RevRec</div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#definition"><span class="rp-toc-num">1</span>Definition</a>
    <a class="rp-toc-pill" href="#key-details"><span class="rp-toc-num">2</span>Key details</a>
    <a class="rp-toc-pill" href="#faq"><span class="rp-toc-num">3</span>FAQ</a>
  </div>
</div>

<div class="rp-callout rp-callout-note">
  <div><strong><i class="fa-solid fa-circle-info" aria-hidden="true"></i> Additional cost</strong>To access these features, you must have an active subscription to either Recurly RevRec or the Standard edition. Contact your Recurly account manager or <a href="mailto:support@recurly.com">support@recurly.com</a> for pricing details.</div>
</div>

### Prerequisites

<ul class="rp-list">
  <li>A cancellation and refund policy that supports account crediting.</li>
</ul>

### Limitations

<ul class="rp-list">
  <li>Prepayment credits can only be used for purchases and can't be refunded.</li>
  <li>Goodwill credits are non-transferable and must be used within the issuing account.</li>
  <li>Credits may have expiration dates or usage conditions, depending on your business policy.</li>
</ul>

# Definition

<div class="rp-definition">Recurly RevRec supports three distinct credit types: Goodwill Credit, On-account Credit, and Prepayment Credit. Each serves a unique purpose — from enhancing revenue recognition to enabling customer retention strategies. You can choose whether to include credit event transactions in your revenue recognition instance.</div>

# Key details

## Incorporating credits in revenue recognition

You can choose whether to include credits in your RevRec instance.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Navigate to Profiles</h4><p>Go to Setup → Profiles.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Set the Ignore Credit Event Transactions option</h4><p>Under "Ignore Credit Event Transactions," select Yes to exclude credit events from RevRec, or No to include them.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/5e90165b450dba809bb3614de2b2eba06b3b2d562d3ec5f1af57539d9f9909b4-Screenshot_2024-10-15_at_12.05.59_PM.png" align="center" width="50%" border={true} />


## Credit types

<div class="rp-nav-grid">

<Cards>
  <Card title="Goodwill credit" href="https://docs.recurly.com/recurly-revrec/docs/goodwill-credit" target="_blank">
    Balance added to a customer's account to acknowledge loyalty, resolve issues, or offer compensation. Integrated into revenue recognition reports.
  </Card>
  <Card title="On-account credit" href="https://docs.recurly.com/recurly-revrec/docs/on-account-credit" target="_blank">
    Issued instead of refunds when subscriptions are canceled, helping retain customers and improve financial reporting accuracy.
  </Card>
  <Card title="Prepayment credit" href="https://docs.recurly.com/recurly-revrec/docs/prepayment-credit" target="_blank">
    Customers pay in advance for services or products. Prepayments are tracked and reported in revenue recognition for better forecasting.
  </Card>
</Cards>

</div>

# FAQ

<Accordion title="What are the credit-event lines that appear in some contracts?">
  When a credit transaction flows from Recurly into RevRec, a credit-event line is created to track that credit and to balance it once it's fully used.
</Accordion>

<Accordion title="How are credit events shown in RevRec?">
  Credits can arise in different ways, and RevRec treats them accordingly:

  - **Goodwill credit:** A free, promotional credit that appears as a Credit Invoice in Recurly. It enters RevRec as one line; each redemption posts as a separate line. Identify via origin = credit-event and plan code.
  - **On-account credit:** Typically issued instead of a cash refund — for example, post-cancellation. It enters as one line; each redemption is a separate line. Identify via origin = credit-event.
  - **Prepayment credit:** Customer-funded advance for future services. In RevRec it appears as one SO line with two invoices; any credit adjustment posts as a new line.
</Accordion>

<Accordion title="How can I see a customer's total available credit balance?">
  In Recurly, open the customer's account page. The sum of the Sell Price for all active credit lines equals the customer's total credit balance.
</Accordion>

<Accordion title="How can I identify credit-related transactions in RevRec?">
  Filter by line-item origin = credit-event. The specific credit type or action — such as redemption or void — can be determined from the plan code.
</Accordion>

<br />
