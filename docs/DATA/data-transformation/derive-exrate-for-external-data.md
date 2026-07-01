---
title: Derive exchange rate for external data
excerpt: >-
  Recurly RevRec automatically derives the correct currency exchange rate for
  contracts, invoices, and costs created outside Recurly, based on their
  creation date.  <br />
deprecated: false
hidden: false
metadata:
  robots: index
---
<div class="rp-page">
  <div class="rp-overview">Recurly RevRec can derive the correct exchange rate for any contract, invoice, or cost created outside Recurly — based on its creation date. That means no more supplying manual rates when you import or reconcile multi-currency subscription data. Flag the lines you want, and the system fills in the historical rate that was in effect.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Part of Recurly RevRec — <a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-advanced" target="_blank">learn more</a></div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#definition"><span class="rp-toc-num">1</span>Definition</a>
    <a class="rp-toc-pill" href="#key-benefits"><span class="rp-toc-num">2</span>Key benefits</a>
    <a class="rp-toc-pill" href="#derive-exchange-rates-for-subscriptions"><span class="rp-toc-num">3</span>Subscriptions</a>
    <a class="rp-toc-pill" href="#derive-exchange-rates-for-costs"><span class="rp-toc-num">4</span>Costs</a>
  </div>
</div>

<div style={{position: "relative", paddingTop: "56.25%", marginBottom: "28px", borderRadius: "10px", overflow: "hidden"}}>
  <iframe src="https://fast.wistia.net/embed/iframe/fxw815ezfm"
    title="Derive exchange rate for external data"
    allow="autoplay; fullscreen"
    allowtransparency="true"
    frameBorder="0"
    scrolling="no"
    allowFullScreen
    style={{position: "absolute", top: 0, left: 0, width: "100%", height: "100%", border: "none"}}></iframe>
</div>

# Definition

<div class="rp-definition">The Derive ExRate feature automatically retrieves the appropriate currency exchange rate — by contract date for subscriptions and by invoice date for invoices — so you don't need to upload rates manually for external data feeds. You can derive rates for uploaded cost lines too.</div>

# Key benefits

<div class="rp-benefits">
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-bullseye" aria-hidden="true"></i></div>
    <strong>Automated accuracy</strong>
    <span>Each line uses the historical rate in effect on its creation date, for precise revenue recognition.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-file-arrow-up" aria-hidden="true"></i></div>
    <strong>Streamlined imports</strong>
    <span>Skip extra columns and manual effort — just flag Derive ExRate and let the system handle the rest.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-chart-column" aria-hidden="true"></i></div>
    <strong>Consistent reporting</strong>
    <span>Keeps multi-currency analytics in sync without rate discrepancies or human error.</span>
  </div>
</div>

<div class="rp-card">

### How derivation is controlled

RevRec derives exchange rates for subscriptions and invoices created outside of Recurly, and for uploaded cost lines — so you never have to upload exchange-rate files manually. The feature is controlled through two attribute labels:

- **Contracts:** `Derive ExRates` (under contract attributes)
- **Costs:** `Cost Derive ExRates` (under cost attributes)

</div>

# Derive exchange rates for subscriptions

For subscriptions and order lines, enable derivation from Setup → Attribute Labels.


<Image src="https://files.readme.io/6ca52efce3c2984bba6ad9e99c5c5b14bdd0b3c414f437bdac04c0d5f8894a07-1_Screenshot_.png" align="center" width="75%" border={true} />


You can enable this feature in either of the following ways.

## Method 1: Set Derive ExRate in your upload file

Use this method when you want to control derivation line by line in the file you upload.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Add a Derive ExRate column</h4><p>Add a column named <code>Derive ExRate</code> to your upload file.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Flag each line</h4><p>For each line where you want RevRec to derive the exchange rate, enter <code>Yes</code> or <code>Y</code> in the <code>Derive ExRate</code> column.</p></div>
  </div>
</div>

## Method 2: Configure a data rule

Use this method when you want RevRec to derive exchange rates for all uploaded order lines by default.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open Data Rule</h4><p>Go to Transformation → Data Rule.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Create a new data rule</h4><p>Enter a name and select Order Line as the object.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Set the attribute</h4><p>Under Application Attributes, select <code>Derive ExRate</code>, and under Value, enter <code>Yes</code>.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Save the data rule</h4><p>After you save, RevRec automatically populates <code>Derive ExRate = Yes</code> for all uploaded order lines.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/8fa01b20f0ee79565c0d3f695579d9fdbfd41893fde1e66b7a279ce06e35c327-2_Screenshot.png" align="center" width="75%" border={true} />


### Behavior and defaults

<ul class="rp-list">
  <li>If <code>Derive ExRate</code> is set to <code>Yes</code> or <code>Y</code>, you don't need to upload exchange rates for that line — RevRec derives them automatically.</li>
  <li>After collection, the sales order line shows <code>Derive ExRate = Y</code> when derivation is enabled.</li>
  <li>If the field isn't set, it defaults to <code>N</code> (or <code>No</code>).</li>
</ul>

# Derive exchange rates for costs

For cost lines, enable derivation from Setup → Attribute Labels → Cost.


<Image src="https://files.readme.io/d9b8d6246f11df3d17d506c13ad0d30f081964f0a6a4107409d46f55f60d26e8-3_Screenshot.png" align="center" width="75%" border={true} />


You can enable this feature in either of the following ways.

## Method 1: Set Cost Derive Ex Rates in your cost upload file

Use this method when you want to control derivation line by line for costs.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Add a Cost Derive Ex Rates column</h4><p>Add a column named <code>Cost Derive Ex Rates</code> to your cost upload file.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Flag each cost line</h4><p>For each cost line where you want RevRec to derive the exchange rate, enter <code>Yes</code> or <code>Y</code> in the <code>Cost Derive Ex Rates</code> column.</p></div>
  </div>
</div>

## Method 2: Configure a data rule

Use this method when you want RevRec to derive exchange rates for all uploaded cost lines by default.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open Data Rule</h4><p>Go to Transformation → Data Rule.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Create a new data rule</h4><p>Enter a name and select Cost as the object.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Set the attribute</h4><p>Under Application Attributes, select <code>Cost Derive Ex Rates</code>, and under Value, enter <code>Yes</code>.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Save the data rule</h4><p>After you save, RevRec automatically populates <code>Cost Derive Ex Rates = Yes</code> for all uploaded cost lines.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/5e5c7bccd34a812ec7479b150f2160ed53ced99cbfaf410bb165958904152db5-4_Screenshot.png" align="center" width="75%" border={true} />


### Behavior and defaults

<ul class="rp-list">
  <li>If <code>Cost Derive Ex Rates</code> is set to <code>Yes</code> or <code>Y</code>, you don't need to upload exchange rates for that cost line — RevRec derives them automatically.</li>
  <li>After collection, cost lines display the derive flag as <code>Y</code> when enabled.</li>
  <li>If the field isn't set, it defaults to <code>N</code> (or <code>No</code>).</li>
</ul>

<br />
