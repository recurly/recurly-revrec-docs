---
title: Performance obligation
excerpt: >-
  Configure performance obligations (POBs) in Recurly RevRec, including
  recognition rules, POB rules, and revenue forecasting for ASC 606 and IFRS 15
  compliance.
deprecated: false
hidden: false
metadata:
  robots: index
---
<div class="rp-page">
  <div class="rp-overview">Performance obligations are the second step of ASC 606 / IFRS 15 compliance in Recurly RevRec. Define each obligation, set up its recognition method, and establish the rules that link it to your transactions — so revenue recognizes accurately and consistently every time.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Available as part of Recurly RevRec</div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#adding-pobs"><span class="rp-toc-num">1</span>Adding POBs</a>
    <a class="rp-toc-pill" href="#adding-pob-rules"><span class="rp-toc-num">2</span>Adding POB rules</a>
    <a class="rp-toc-pill" href="#pob-forecasting"><span class="rp-toc-num">3</span>POB forecasting</a>
  </div>
</div>

# Adding POBs

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Navigate to POB</h4><p>Go to Rules → POB.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/9e57f37-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Add a new POB</h4><p>Select the "+" button to add a new performance obligation.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/4fd4296-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Name the POB</h4><p>Enter a unique name for the performance obligation.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/b21625b-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Set the active date</h4><p>Provide the active date for the new POB.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/f281b16-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">5</div>
    <div><h4>Select the waterfall type</h4><p>Choose the appropriate Waterfall Type (WF Type) from the dropdown.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/9c4764d-image.png" align="center" width="75%" border={true} />


<div class="rp-nav-grid">

<Cards>
  <Card title="PointInTime">
    Performance obligations are recognized at a single point in time.
  </Card>
  <Card title="OverTime">
    Performance obligations are recognized over the contract period.
  </Card>
  <Card title="OverTime Slide">
    Recognized over the contract period, with a delayed release date that extends revenue recognition.
  </Card>
  <Card title="OverTime Condense">
    Recognized based on the release date, with recognition adjusted according to event timing.
  </Card>
  <Card title="Manual">
    Revenue is realized based on manual input.
  </Card>
</Cards>

</div>

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">6</div>
    <div><h4>Choose the accounting method</h4><p>Select the accounting method for the new POB from the dropdown options.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/2b6ede8-image.png" align="center" width="75%" border={true} />


<div class="rp-nav-grid">

<Cards>
  <Card title="Daily">
    Revenue is recognized daily, based on the number of days in the contract.
  </Card>
  <Card title="FixedMonthly">
    Revenue is calculated in fixed amounts based on the number of months in the contract, with adjustments for the start date.
  </Card>
  <Card title="PartialMonthly">
    Revenue is calculated partially for the first and last months of the contract, with equal recognition for the remaining months.
  </Card>
  <Card title="Annually">
    Revenue is calculated annually.
  </Card>
</Cards>

</div>

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">7</div>
    <div><h4>Select the ratable method</h4><p>Choose the ratable method from the dropdown options.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/0bd9e92-image.png" align="center" width="75%" border={true} />


<div class="rp-nav-grid">

<Cards>
  <Card title="Sales Order Ratable">
    Revenue is amortized on a prorated basis, with catch-up applied in the current open period.
  </Card>
  <Card title="Sales Order Dates">
    Revenue is scheduled based on the start and end dates of the sales order lines.
  </Card>
  <Card title="Billing Dates">
    Revenue is scheduled based on the start and end dates of the billing or invoice.
  </Card>
</Cards>

</div>

After completing steps 1–6, save your changes. Your POB should look like this:


<Image src="https://files.readme.io/2a3d5ab-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">8</div>
    <div><h4>Choose how date changes affect the waterfall</h4><p>Select how a date change in a contract affects the revenue waterfall.</p></div>
  </div>
</div>

<ul class="rp-list">
  <li><strong>Default (Blank):</strong> The waterfall remains unchanged.</li>
  <li><strong>Cumulative Date Change:</strong> The entire waterfall is recalculated, considering both past and future payments, so the total amount is distributed accurately based on the new dates.</li>
  <li><strong>Prospective Date Change:</strong> Only future payments are adjusted to reflect the new dates. Past payments remain unaffected.</li>
</ul>

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">9</div>
    <div><h4>Open Revenue Release</h4><p>In the POB configuration screen, locate the Revenue Release section.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">10</div>
    <div><h4>Add a release event</h4><p>Select the "+" button in the Revenue Release section to add a new release event.</p></div>
  </div>
</div>

<ol>
  <li>Select the desired event from the dropdown menu.</li>
  <li>Enter the percentage of revenue release applicable for this event.</li>
</ol>


<Image src="https://files.readme.io/aad214f-image.png" align="center" width="75%" border={true} />


<div class="rp-callout rp-callout-note">
  <div><strong><i class="fa-solid fa-circle-info" aria-hidden="true"></i> Note</strong>You can add multiple release events to a single POB, which lets you recognize revenue accurately across different events and their corresponding release percentages. If the release event selected is Upon Booking or Upon Billing, the percentage must always be 100 — you can't combine multiple release events with either of these.</div>
</div>

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">11</div>
    <div><h4>Save</h4><p>Save all changes.</p></div>
  </div>
</div>

# Adding POB rules

You can access POB rules using one of two methods:

<Tabs>
  <Tab title="From the Rules menu">

1. Go to the Rules section in the navigation menu.
2. Select "Rules" under the Performance Obligation menu.

  </Tab>
  <Tab title="From a POB">

1. Open the desired POB.
2. Navigate to the "Rules" tab at the top.

  </Tab>
</Tabs>

<div class="rp-callout rp-callout-note">
  <div><strong><i class="fa-solid fa-circle-info" aria-hidden="true"></i> Note</strong>You can view a POB's rules by opening the POB and scrolling to the bottom of the page, but you won't find an edit or add rule option there. Use one of the two methods above to make changes.</div>
</div>

Once you're in the Rules section, follow these steps to add a POB rule:

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Start a new rule</h4><p>Select the "+" icon under the Rules section.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/165cf0c-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Select the POB</h4><p>Select the specific POB the rule should apply to.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/e247385-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Define the attribute</h4><p>Define the attribute value used for recognizing the POB — for example, "Item." If the value you need isn't available, select the window-shaped button, choose the attribute from the window that appears, then select "Save." In this example, "Account Code" is used as the attribute for POB recognition.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/8698dfd-image.png" align="center" width="75%" border={true} />



<Image src="https://files.readme.io/79bb6b3-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Enter the attribute value</h4><p>Once you've determined the attribute, enter the value that describes the POB and adjust the active date as needed.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/31a59de-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">5</div>
    <div><h4>Save</h4><p>Select the Save icon to save the rule.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/7388d8a-image.png" align="center" width="75%" border={true} />


<ul class="rp-list">
  <li>Avoid editing the default POBs, such as "Material right" and "Manual journal."</li>
  <li>Multiple release events can be associated with a single POB, but the total release percentage must equal 100%.</li>
  <li>Every POB requires an assigned rule to function properly.</li>
  <li>You can change the hierarchy of POB rules by dragging and rearranging them using the drag icon.</li>
  <li>Remember to save any changes you make to rules or hierarchy.</li>
  <li>To delete a POB rule, select the rule and select the Delete icon, then select Save to confirm the deletion.</li>
</ul>


<Image src="https://files.readme.io/d7091a2-image.png" align="center" width="75%" border={true} />


# POB forecasting

In most cases, revenue is recognized on the date a contract is booked or billed. For some contracts, though, revenue recognition is delayed until a specific external event occurs.

Forecast Management lets you forecast revenue based on both external events and billing dates. Even if the exact date of an external event — like a product release — is unknown, you can still factor it into your forecast by assuming it happens by the contract end date. This lets you plan revenue around a predictable contract end date.

## Configuring forecasting for a POB

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Navigate to the POB</h4><p>Go to the POB you want to configure.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Open Forecast</h4><p>Select Forecast to land on the forecast page.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Select the waterfall type</h4><p>Choose the waterfall type for the forecast: Point in Time, OverTime, OverTime Slide, or OverTime Condense.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Set the forecast percentage</h4><p>Enter the percentage of revenue to forecast based on this rule. The forecast release can never total more than 100% at any given point.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">5</div>
    <div><h4>Choose the forecast date</h4><p>Select the "forecast on" date — the date revenue should be forecasted against. Options include Book Date, Start Date, End Date, and Delivery Date.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">6</div>
    <div><h4>Set the forecast window</h4><p>Enter the number of days for the forecast to start or end, using the Start Day and End Day fields. For example, if "forecast on" is Book Date and you enter 30 as the start day, the system creates the forecast at Book Date + 30 days.</p></div>
  </div>
</div>

<br />
