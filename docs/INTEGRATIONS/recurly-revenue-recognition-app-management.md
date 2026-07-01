---
title: App Management — RevRec
excerpt: >-
  Configure Recurly RevRec to handle App Store and Google Play Store
  subscription data through contract grouping, an exclusive POB, data rules, and
  the App Management integration.
deprecated: false
hidden: false
metadata:
  robots: index
---
<div class="rp-page">
  <div class="rp-overview">Recurly RevRec can handle subscription data from both the Apple App Store and the Google Play Store. A few straightforward configurations — contract grouping, an exclusive performance obligation, a set of data rules, and the App Management integration job — get your app store data flowing in and recognizing revenue correctly. This page walks through each one in order.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Part of Recurly RevRec — <a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-advanced" target="_blank">learn more</a></div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#definition"><span class="rp-toc-num">1</span>Definition</a>
    <a class="rp-toc-pill" href="#key-benefits"><span class="rp-toc-num">2</span>Key benefits</a>
    <a class="rp-toc-pill" href="#grouping-configuration"><span class="rp-toc-num">3</span>Grouping configuration</a>
    <a class="rp-toc-pill" href="#performance-obligation"><span class="rp-toc-num">4</span>Performance obligation</a>
    <a class="rp-toc-pill" href="#data-rule-configuration"><span class="rp-toc-num">5</span>Data rule configuration</a>
    <a class="rp-toc-pill" href="#app-management-integration"><span class="rp-toc-num">6</span>App Management integration</a>
  </div>
</div>

# Definition

<div class="rp-definition">Recurly RevRec can handle subscription data from both the Apple App Store and the Google Play Store. To manage app store data, you set up a handful of straightforward configurations in Recurly RevRec that group the data, assign a performance obligation, transform it with data rules, and pull it in through an integration job.</div>

# Key benefits

<div class="rp-benefits">
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-layer-group" aria-hidden="true"></i></div>
    <strong>Streamlined data management</strong>
    <span>Group app store data by subscription source for accurate, efficient handling.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-clock" aria-hidden="true"></i></div>
    <strong>Flexible revenue recognition</strong>
    <span>Define an exclusive POB for app store data, recognizing revenue on an over-time basis.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-gears" aria-hidden="true"></i></div>
    <strong>Enhanced data rules</strong>
    <span>Copy Google fees to the App Fees attribute and assign distinct account numbers for Apple and Google Store data.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-plug" aria-hidden="true"></i></div>
    <strong>Seamless integration</strong>
    <span>Flow app store data into Recurly RevRec with the App Management integration.</span>
  </div>
</div>

# Grouping configuration

Configure your system to group order lines based on the subscription's source — Apple App Store or Google Play Store.

App store data is organized by subscription, so you'll create two separate grouping rules using the contract grouping feature:

<ul class="rp-list">
  <li><strong>Apple Store grouping rule:</strong> set the grouping attribute to Source = Apple Store.</li>
  <li><strong>Play Store grouping rule:</strong> set the grouping attribute to Source = Play Store.</li>
</ul>

This setup ensures order lines are accurately grouped by subscription source.


<Image src="https://files.readme.io/c12a5169c1ba7c997669e14fa3e4ffa32b6a7b9bb9744cec662251558ae07f88-1_Grouping_Config.png" align="center" width="75%" border={true} />


# Performance obligation

Define an exclusive Performance Obligation (POB) for app store data, where revenue is recognized over time.

This POB — called App Subscription — is automatically assigned to any order line in a contract that meets the Recurly RevRec rules for either Play Store or Apple Store data.


<Image src="https://files.readme.io/e4b80b6217c0f05b40f6172ec21e405d0b1185473a5dcc1c5b23eee5e1f86555-2_POB.png" align="center" width="75%" border={true} />


The POB rules are based on the source of the data, ensuring that all order lines with the specified source are grouped under the App Subscription POB.


<Image src="https://files.readme.io/77f5d669bd2139deb12466c6119b28e9a3c272e9cc04094b0691334566d27e82-3_POB_Rules.png" align="center" width="75%" border={true} />


<div class="rp-callout rp-callout-important">
  <div><strong><i class="fa-solid fa-circle-exclamation" aria-hidden="true"></i> Important</strong>The hierarchy of these rules is critical to guaranteeing the correct obligation is applied.</div>
</div>

# Data rule configuration

To ensure accurate revenue recognition, configure data rules that transform your app store data correctly. You'll copy the sell price from Google Fees lines into the App Fees attribute and assign the proper account numbers for Play Store and Apple Store data. There are four data rules.

## Data rule 1 — Copy Google fees to App Fees

Copies the sell price from Google Fees lines into the App Fees attribute.

**Rule**

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Application attribute</td><td>Formula</td></tr>
  <tr><td>App Fees</td><td><code>Line.SellPrice</code></td></tr>
</table>

**Criteria**

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Field</td><td>Operator</td><td>Value</td></tr>
  <tr><td>Plan</td><td>=</td><td>Google Fees</td></tr>
</table>


<Image src="https://files.readme.io/6ce5c2ecf7e0343039efd0c9cf37d3b8f1151eaa89492acb3b69bc867052e0d6-4_Data_Rule.png" align="center" width="75%" border={true} />


## Data rule 2 — Zero out Google fees

Sets the sell price of the Google Fees plan to zero to avoid duplicative charges.

**Rule**

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Application attribute</td><td>Formula</td></tr>
  <tr><td>App Fees</td><td>0</td></tr>
</table>

**Criteria**

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Field</td><td>Operator</td><td>Value</td></tr>
  <tr><td>Plan</td><td>=</td><td>Google Fees</td></tr>
</table>


<Image src="https://files.readme.io/14ab1e62d857d59865b8ed09371367da4df6e629723f87c270bf4dd280cba05d-5_Data_Rule_2.png" align="center" width="75%" border={true} />


## Data rule 3 — Assign account numbers for Play Store data

Applies the appropriate account number for all order lines with a source of Play Store.

**Rule**

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Application attribute</td><td>Formula</td></tr>
  <tr><td>Liability Account</td><td>23100</td></tr>
  <tr><td>Revenue Account</td><td>33200</td></tr>
</table>

**Criteria**

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Field</td><td>Operator</td><td>Value</td></tr>
  <tr><td>Source</td><td>=</td><td>Play Store</td></tr>
</table>


<Image src="https://files.readme.io/c5a03f8b4bcde418d6fa12a7af132d68b46cde13f32bdf02081d59614114a26f-6_Data_Rule_3.png" align="center" width="75%" border={true} />


## Data rule 4 — Assign account numbers for Apple Store data

Applies the appropriate account number for all order lines with a source of Apple Store.

**Rule**

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Application attribute</td><td>Formula</td></tr>
  <tr><td>Liability Account</td><td>23000</td></tr>
  <tr><td>Revenue Account</td><td>33000</td></tr>
</table>

**Criteria**

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Field</td><td>Operator</td><td>Value</td></tr>
  <tr><td>Source</td><td>=</td><td>Apple Store</td></tr>
</table>


<Image src="https://files.readme.io/a2c2dcb2dd29f02108ad4743f7102558b5593742e85cad7ece22c67ea661afd3-7_Data_Rule_4.png" align="center" width="75%" border={true} />


# App Management integration

Once your data rules are configured, run the App Management integration job. This integration pushes all processed app store data into Recurly RevRec.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open the integration job</h4><p>Go to Import/Export → Scheduled Jobs → App Management Integration.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/4cacd6bf89fb34de50b38315f39b77e53c155f362ea72336094c9d6406bd2152-8_App_management_Integration.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Run the job</h4><p>Ensure the job is active, then select Run to execute the integration.</p></div>
  </div>
</div>

<br />
