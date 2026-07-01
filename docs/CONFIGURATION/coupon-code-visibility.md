---
title: Coupon code visibility
excerpt: >-
  RevRec surfaces coupon code data from Recurly Billing at the subscription and
  charge line level, including on credit events, to help your finance team trace
  discounts for ASC 606 and IFRS 15 reporting.
deprecated: false
hidden: false
metadata:
  robots: index
---
<div class="rp-page">
  <div class="rp-overview">RevRec pulls coupon code data directly from Recurly Billing and surfaces it in your RevRec views. Instead of cross-referencing billing records and revenue schedules manually, you can now see coupon codes at both the subscription and charge line level — including on credit events — to help your finance team trace discounts for ASC 606 and IFRS 15 reporting.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Available as part of Recurly RevRec</div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#key-details"><span class="rp-toc-num">1</span>Key details</a>
    <a class="rp-toc-pill" href="#faq"><span class="rp-toc-num">2</span>FAQ</a>
  </div>
</div>

<iframe src="https://fast.wistia.net/embed/iframe/mduu4gjqnz?web_component=true&seo=false&videoFoam=false" title="Coupon code visibility" allow="autoplay; fullscreen" allowtransparency="true" frameborder="0" scrolling="no" class="wistia_embed" name="wistia_embed" width="640px" height="360px"></iframe>
<script src="https://fast.wistia.net/player.js" async></script>

# Key details

## Where coupon codes appear

<table class="rp-params">
  <tr class="rp-thead-row"><td>Level</td><td>What you'll see</td><td>Format</td><td>Why it matters</td></tr>
  <tr><td>Subscription</td><td>A consolidated list of coupon codes associated with the subscription lifecycle.</td><td>A single concatenated string of active coupon codes.</td><td>Helps you understand the discount context for the subscription when reviewing contracts and forecasting revenue impact.</td></tr>
  <tr><td>Charge line</td><td>The specific coupon code or codes that discounted an individual invoice line item.</td><td>If multiple coupons apply, codes are separated by a comma.</td><td>Makes it clear which discounts affected which charge lines, so allocations and reconciliations are easier to validate.</td></tr>
  <tr><td>Credit events (refunds, voids, write-offs)</td><td>Coupon codes from the original invoiced charge being credited.</td><td>Mirrors the original charge line's coupon code list.</td><td>Preserves traceability for negative revenue events by tying the credit back to the original commercial terms.</td></tr>
</table>

## Data fields and attributes

Use the following attributes in the Workbench and in exports to report on coupon codes:

<table class="rp-params">
  <tr class="rp-thead-row"><td>Attribute</td><td>Type</td><td>Label</td><td>What it contains</td></tr>
  <tr><td><strong>F23</strong></td><td>Contract attribute</td><td><strong>Coupon Codes</strong></td><td>A concatenated string of all active coupon codes associated with the subscription lifecycle.</td></tr>
  <tr><td><strong>F9</strong></td><td>Billing attribute</td><td><strong>Invoice coupon codes</strong></td><td>The coupon code or codes applied to a specific invoice line item.</td></tr>
</table>

# FAQ

<Accordion title="I see multiple codes in one field. How do I separate them?">
  Coupon codes are stored as a concatenated string — for example, <code>CODE1, CODE2</code>. If you export to CSV or Excel, you can split the field using Excel's Text to Columns feature with a comma delimiter.
</Accordion>

<Accordion title="Why do I see a coupon code on a refund line?">
  That's expected. For refunds, voids, and write-offs, RevRec looks back to the original invoiced charge line and displays the coupon code or codes that applied there. This keeps the credit event tied to the original discount conditions for audit and reconciliation.
</Accordion>

<br />
