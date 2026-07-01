---
title: Contract modification
excerpt: >-
  Understand the six types of contract modifications in Recurly RevRec, set
  contract revision levels, configure modification rules, and view changes in
  the Revenue Workbench.
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
  <div class="rp-overview">Contract modification in Recurly RevRec covers approved alterations to the price, term, or both of a contract — changes mutually agreed upon by the supplier and customer. The system automatically selects the appropriate modification sub-type based on the nature of the change, so revenue recognition stays accurate and compliant. This feature is part of Recurly RevRec. <a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-advanced" target="_blank">Learn more</a>.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Available as part of Recurly RevRec</div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#definition"><span class="rp-toc-num">1</span>Definition</a>
    <a class="rp-toc-pill" href="#key-benefits"><span class="rp-toc-num">2</span>Key benefits</a>
    <a class="rp-toc-pill" href="#key-details"><span class="rp-toc-num">3</span>Key details</a>
    <a class="rp-toc-pill" href="#faq"><span class="rp-toc-num">4</span>FAQ</a>
  </div>
</div>

### Prerequisites

<ul class="rp-list">
  <li>A valid Recurly account with appropriate permissions.</li>
  <li>Basic understanding of Recurly's revenue recognition processes.</li>
  <li>Familiarity with contract terms and conditions.</li>
</ul>

### Limitations

<ul class="rp-list">
  <li>Modifications must be approved by both parties.</li>
  <li>Not all types of modifications may be supported under certain conditions.</li>
  <li>Manual modifications using the Revenue Workbench may be treated differently.</li>
</ul>

# Definition

<div class="rp-definition">Contract modification in Recurly Revenue Recognition pertains to approved alterations in the price, term, or both of a contract. These changes are mutually agreed upon by both the supplier and customer, either in writing or through established practices.</div>

# Key benefits

<div class="rp-benefits">
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-sliders" aria-hidden="true"></i></div>
    <strong>Flexibility</strong>
    <span>Adjust contract terms easily to accommodate changing business needs.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-gears" aria-hidden="true"></i></div>
    <strong>Automation</strong>
    <span>The system automatically selects sub-types based on the nature of the modification.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-sitemap" aria-hidden="true"></i></div>
    <strong>Clarity</strong>
    <span>Clear categorization of modifications ensures accurate revenue recognition.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-bolt" aria-hidden="true"></i></div>
    <strong>Efficiency</strong>
    <span>Streamlined processes reduce manual intervention and errors.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-eye" aria-hidden="true"></i></div>
    <strong>Transparency</strong>
    <span>All modifications are traceable and viewable within the Revenue Workbench.</span>
  </div>
</div>


<Image src="https://files.readme.io/1c72453-image.png" align="center" width="60%" />


# Key details

## Types of modification supported

Recurly Revenue Recognition supports six primary types of contract modifications. Each primary type encompasses various sub-types. Depending on the nature of the change during the set Contract Revision Level, specific actions are triggered:

<div class="rp-nav-grid">

<Cards>
  <Card title="New Line/POB">
    The system selects an appropriate sub-type based on the modification.
  </Card>
  <Card title="Price Change">
    A sub-type is chosen based on the nature of the price alteration.
  </Card>
  <Card title="Quantity Change">
    The system determines a sub-type according to the modification.
  </Card>
  <Card title="Term Change">
    A sub-type is selected based on the term adjustment.
  </Card>
  <Card title="Cancellations / Returns">
    Activated when a contract amendment results from a cancellation or return.
  </Card>
  <Card title="All Others">
    Any alterations made to the contract using manual functions in the Revenue Workbench are treated as a Contract Modification.
  </Card>
</Cards>

</div>


<Image src="https://files.readme.io/1b83a1b-image.png" align="center" width="75%" border={true} />


## Key terminology

<ul class="rp-list">
  <li><strong>POB-related terminology:</strong> POBs are categorized as distinct or non-distinct based on term, quantity, or both.</li>
  <li><strong>SSP-related terminology:</strong> Terms such as "Within SSP Range" and "Outside SSP Range" describe the sell price of a new line relative to the SSP range.</li>
  <li><strong>Treatment-related terminology:</strong> Contract modifications can be treated as "Cumulative Catchup," "Prospective Catchup," or "No Allocation."</li>
</ul>

## Setting the Contract Revision Level

The Contract Revision Level defines how long after a change the system recognizes it as a modification.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Navigate to Contract Revision Level</h4><p>Go to Setup → Profiles → Contract Revision Level.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/a008b06-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Select the revision level</h4><p>In the value column, choose one of the following from the dropdown.</p></div>
  </div>
</div>

<ul class="rp-list">
  <li><strong>All:</strong> All changes to the contract are treated as modifications.</li>
  <li><strong>Period:</strong> Changes in the next and subsequent periods are recognized as modifications.</li>
  <li><strong>Quarter:</strong> Adjustments in the next and subsequent quarters are considered modifications.</li>
</ul>

## Changing treatment in modification rules

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Navigate to Contract Modification</h4><p>Go to Setup → Contract Modification.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Select the rule</h4><p>Choose the desired contract modification rule from the dropdown list.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/c5aaee1-image.png" align="center" width="75%" border={true} />


## Viewing modifications in the Workbench

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open the contract</h4><p>Access the Revenue Workbench and select the modified contract.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Review the Modifications tab</h4><p>Under the Modifications tab of the contract, all changes and revision levels are displayed.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/56a1b13-image.png" align="center" width="75%" border={true} />


# FAQ

<Accordion title="What is a Contract Modification in Recurly RevRec?">
  It's an approved change in the price, term, or both of a contract within Recurly's revenue recognition platform. Both the supplier and customer must agree on the modification.
</Accordion>

<Accordion title="How many types of modifications does Recurly RevRec support?">
  Recurly RevRec supports six primary types of modifications, each with its own sub-types: New Line/POB, Price Change, Quantity Change, Term Change, Cancellations/Returns, and All Others.
</Accordion>

<Accordion title="Can I manually modify a contract in Recurly RevRec?">
  Yes. You can make manual modifications using the Revenue Workbench. These changes are treated as the "All Others" type of Contract Modification.
</Accordion>

<Accordion title="How can I view the changes made to a contract?">
  Navigate to the Revenue Workbench and select the modified contract. Under the Modifications tab, you'll see all changes and revision levels.
</Accordion>

<Accordion title="What's the difference between Cumulative Catchup and Prospective Catchup treatments?">
  Cumulative Catchup uses a retrospective approach, recalculating amounts from the beginning of the contract. Prospective Catchup only considers changes from the moment they were made, excluding amounts posted in closed periods.
</Accordion>

<Accordion title="How do I set the Contract Revision Level?">
  Go to Setup → Profiles → Contract Revision Level. From there, select the desired revision level from the dropdown — All, Period, or Quarter.
</Accordion>

<Accordion title="What happens if a new line's sell price falls outside the SSP range?">
  It's described as "Outside SSP Range" — terminology used to indicate that the sell price of a new line falls outside the configured SSP range.
</Accordion>

<Accordion title="Are all modifications treated the same way in Recurly RevRec?">
  No. Modifications can be treated as Cumulative Catchup, Prospective Catchup, or No Allocation, depending on the nature of the change and the settings you choose.
</Accordion>

<Accordion title="What are Contract Modification Rules and how do they automate one-off scenarios?">
  Contract Modification Rules define how RevRec automates one-off contract changes such as upsells, downsells, or extensions. Configuration steps are detailed in the Application setup → Contract modification section. See the Contract Modification documentation for complete setup guidance.
</Accordion>

<br />
