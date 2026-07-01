---
title: Autobill for external data
excerpt: >-
  Auto Bill in Recurly RevRec generates invoice lines directly from uploaded
  sales orders, so you don't import separate billing files when subscription and
  billing terms align.
deprecated: false
hidden: false
metadata:
  robots: index
---
<div class="rp-page">
  <div class="rp-overview">Auto Bill lets Recurly RevRec generate your invoice lines directly from the sales orders you upload — no separate billing files required. When your subscription and billing terms align, the system creates the matching invoices for you, keeping billing and recognition in sync end to end. It's one less parallel import to maintain.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Part of Recurly RevRec — <a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-advanced" target="_blank">learn more</a></div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#definition"><span class="rp-toc-num">1</span>Definition</a>
    <a class="rp-toc-pill" href="#key-benefits"><span class="rp-toc-num">2</span>Key benefits</a>
    <a class="rp-toc-pill" href="#enabling-auto-bill"><span class="rp-toc-num">3</span>Enabling Auto Bill</a>
  </div>
</div>

### Limitations

<ul class="rp-list">
  <li>Upfront billing only — the sales order must reflect the full contract value at upload, and the billing cadence must match the subscription term.</li>
  <li>No post-generation edits — invoices created via Auto Bill can't be updated or canceled. Any revisions require manual invoice imports.</li>
</ul>

# Definition

<div class="rp-definition">Auto Bill generation reads your imported subscription or contract records and automatically creates the corresponding invoice lines. When subscription and billing terms align, it eliminates the need to upload separate billing files.</div>

# Key benefits

<div class="rp-benefits">
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-file-arrow-up" aria-hidden="true"></i></div>
    <strong>Simplified imports</strong>
    <span>Upload only your subscription records — the system crafts the matching invoices.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-arrows-to-circle" aria-hidden="true"></i></div>
    <strong>Unified revenue flow</strong>
    <span>Keep recognition and billing together in one process for cleaner financial reporting.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-gauge-simple-high" aria-hidden="true"></i></div>
    <strong>Reduced operational overhead</strong>
    <span>No more maintaining parallel invoice uploads — let Auto Bill handle it.</span>
  </div>
</div>

# Enabling Auto Bill

You can turn on Auto Bill in one of two ways: flag it directly in your upload file, or configure a data rule that applies it automatically. Both start from Setup → Attribute Labels.


<Image src="https://files.readme.io/a33ed901139845e5312c3b10eda7ba3b0335d36167f672e5aaff62f9d3aa2804-image.png" align="center" width="75%" border={true} />


## Method 1: Auto Bill attribute in your upload file

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Add an Auto Bill column</h4><p>Include a column named <code>Auto Bill</code> in your sales order upload.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Flag each line</h4><p>Enter <code>Yes</code> or <code>Y</code> for each line you want the system to generate an invoice for.</p></div>
  </div>
</div>

Once flagged, you don't need to import any separate invoice records for those lines — Auto Bill creates them automatically.

## Method 2: Configuring a data rule

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open Data Rules</h4><p>Go to Transformation → Data Rules.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Create a new rule</h4><p>Name your rule and select Order Line as the object.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Set the application attribute</h4><p>Under Application Attributes, choose <code>Auto Bill</code> and set the value to <code>Yes</code>.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Save the rule</h4><p>Save the rule to activate it.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/31abf4fc4251a0d1934f82f1bfe679415d11294178022045e07b78f2581ca654-image.png" align="center" width="75%" border={true} />


With this rule active, every uploaded line defaults to Auto Bill = `Y`, so the system generates invoices without any file-level flags.

<div class="rp-callout rp-callout-note">
  <div><strong><i class="fa-solid fa-circle-info" aria-hidden="true"></i> Note</strong>Auto Bill only works for full-term, upfront-billed subscriptions. If your billing cadence diverges from the subscription term, continue importing billing records manually.</div>
</div>

<br />
