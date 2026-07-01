---
title: Datasets
excerpt: >-
  Datasets in Recurly RevRec are custom, user-defined tables of attributes that
  power your reports and analysis, refreshing nightly to keep insights current.
deprecated: false
hidden: false
metadata:
  robots: index
---
<div class="rp-page">
  <div class="rp-overview">Datasets are dynamic, user-defined tables of attributes — like item, account, region, or customer — that drive every report and analysis in Recurly RevRec. Pick the fields you care about, and the dataset becomes a reusable table for reporting. Once created, datasets refresh nightly, so your insights always reflect the latest sales and revenue data.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Part of Recurly RevRec — <a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-advanced" target="_blank">learn more</a></div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#definition"><span class="rp-toc-num">1</span>Definition</a>
    <a class="rp-toc-pill" href="#key-benefits"><span class="rp-toc-num">2</span>Key benefits</a>
    <a class="rp-toc-pill" href="#creating-a-dataset"><span class="rp-toc-num">3</span>Creating a dataset</a>
    <a class="rp-toc-pill" href="#faqs"><span class="rp-toc-num">4</span>FAQs</a>
  </div>
</div>

# Definition

<div class="rp-definition">A dataset is a custom collection of fields (attributes) from your sales orders and contracts, organized into a reusable table for reporting and analysis. Datasets can't be deleted — only inactivated — which preserves historical integrity while preventing future use.</div>

# Key benefits

<div class="rp-benefits">
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-table-cells" aria-hidden="true"></i></div>
    <strong>Tailored analytics</strong>
    <span>Pick exactly the attributes you need — item, liability account, region, customer — and build bespoke data tables.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-arrows-rotate" aria-hidden="true"></i></div>
    <strong>Always current</strong>
    <span>Datasets auto-refresh daily, so your dashboards and reports reflect the latest sales and revenue.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-clock-rotate-left" aria-hidden="true"></i></div>
    <strong>Safe versioning</strong>
    <span>Inactivate outdated datasets instead of deleting them, keeping audit trails intact while retiring superseded configurations.</span>
  </div>
</div>

# Creating a dataset

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open the dataset screen</h4><p>Go to Transformation → Dataset.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/bb61372-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Name the dataset</h4><p>Enter a unique dataset name.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Select the books</h4><p>Select the books (ledgers) this dataset applies to.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Choose attributes</h4><p>Choose the desired attributes and mark your primary attribute or attributes.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/04cf460-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">5</div>
    <div><h4>Save the configuration</h4><p>Select Save to finalize the dataset.</p></div>
  </div>
</div>

Once saved, any uploaded sales order with matching identifiers populates your new dataset. You'll see the data reflected in the Revenue Workbench and across all analytics reports, for consistent, accurate insights.


<Image src="https://files.readme.io/9cdca79-image.png" align="center" width="75%" border={true} />


<div class="rp-callout rp-callout-note">
  <div><strong><i class="fa-solid fa-circle-info" aria-hidden="true"></i> Note</strong>Datasets can't be permanently deleted. You can only toggle a dataset to Inactive to retire it from future use while retaining its historical records.</div>
</div>

# FAQs

<Accordion title="How do I manage and use datasets for custom data ingestion in the RevRec application?">
  Go to Application Setup → Data Sets to define schemas, map fields, and set validations. You can load data via the UI or API, then reference those datasets in Data Transformation rules and the Workbench.
</Accordion>

<br />
