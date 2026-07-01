---
title: Manual journal entry
excerpt: >-
  Upload accounting adjustments directly into Recurly RevRec with full control
  over journal data, posting period, and approval workflow.
deprecated: false
hidden: false
metadata:
  robots: index
---
<div class="rp-page">
  <div class="rp-overview">Manual journal entries let you upload accounting adjustments directly into Recurly RevRec, with full control over the journal data, posting period, and approval workflow. Use them when an entry needs to be recorded outside the system's automated revenue recognition logic. Because the process is fully manual, you provide every required value — and RevRec posts exactly what your file contains.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Part of Recurly RevRec — <a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-advanced" target="_blank">learn more</a></div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#definition"><span class="rp-toc-num">1</span>Definition</a>
    <a class="rp-toc-pill" href="#key-benefits"><span class="rp-toc-num">2</span>Key benefits</a>
    <a class="rp-toc-pill" href="#prepare-the-upload-file"><span class="rp-toc-num">3</span>Prepare the upload file</a>
    <a class="rp-toc-pill" href="#upload-a-manual-journal-entry"><span class="rp-toc-num">4</span>Upload</a>
    <a class="rp-toc-pill" href="#review-and-approve-the-journal-entry"><span class="rp-toc-num">5</span>Review and approve</a>
    <a class="rp-toc-pill" href="#reporting-examples"><span class="rp-toc-num">6</span>Reporting examples</a>
    <a class="rp-toc-pill" href="#important-considerations"><span class="rp-toc-num">7</span>Important considerations</a>
    <a class="rp-toc-pill" href="#faqs"><span class="rp-toc-num">8</span>FAQs</a>
  </div>
</div>

### Prerequisites

Before you upload a manual journal entry file, make sure:

<ul class="rp-list">
  <li>Your file is complete and properly formatted.</li>
  <li>All mandatory columns are included.</li>
  <li>Posting details such as Books and Period are known in advance.</li>
  <li>The data has been reviewed for accuracy, including accounts, amounts, currency, and segment values.</li>
</ul>

### Limitations

<ul class="rp-list">
  <li>Manual journal entries operate independently from automated RevRec rules.</li>
  <li>RevRec doesn't derive or populate values from data rules, revenue schedules, or existing system logic.</li>
  <li>You must manually provide all required financial dimensions and segments in the upload file.</li>
  <li>If Start Date and End Date are blank, the full amount is recognized in the uploaded period.</li>
  <li>If Auto Reversal is set to Yes, the current-period entry is reversed in the next period.</li>
</ul>

# Definition

<div class="rp-definition">A manual journal entry is a journal entry you upload into RevRec using a prepared file. After upload, the entry moves through a review and approval workflow before it's posted to the selected books and period.</div>

# Key benefits

<div class="rp-benefits">
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-sliders" aria-hidden="true"></i></div>
    <strong>Precise control</strong>
    <span>Record accounting adjustments exactly as you need them.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-book" aria-hidden="true"></i></div>
    <strong>Targeted posting</strong>
    <span>Post entries to specific books and accounting periods.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-circle-check" aria-hidden="true"></i></div>
    <strong>Approval before posting</strong>
    <span>Review and approve each entry in the Revenue Workbench before it posts.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-chart-column" aria-hidden="true"></i></div>
    <strong>Reflected in reporting</strong>
    <span>See manual adjustments in RevRec reporting, including waterfall and balance reports.</span>
  </div>
</div>

# Prepare the upload file

Your manual journal entry file must include the mandatory columns below. You can add extra columns if your process needs them.

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Column</td><td>Requirement</td><td>Notes</td></tr>
  <tr><td>Subscription Number</td><td>Required</td><td>Enter the subscription identifier.</td></tr>
  <tr><td>Subscription Line</td><td>Required</td><td>Enter the subscription line.</td></tr>
  <tr><td>Account Type</td><td>Required</td><td>Use one supported value, such as Asset, Liability, Revenue, COGS, or Deferred COGS.</td></tr>
  <tr><td>Asset</td><td>Conditional</td><td>Use when the entry affects an asset account.</td></tr>
  <tr><td>Liability</td><td>Conditional</td><td>Use when the entry affects a liability account.</td></tr>
  <tr><td>Revenue</td><td>Conditional</td><td>Use when the entry affects a revenue account.</td></tr>
  <tr><td>COGS</td><td>Conditional</td><td>Use when the entry affects a cost of goods sold account.</td></tr>
  <tr><td>Deferred COGS</td><td>Conditional</td><td>Use when the entry affects deferred cost.</td></tr>
  <tr><td>Start Date</td><td>Optional</td><td>Can be blank.</td></tr>
  <tr><td>End Date</td><td>Optional</td><td>Can be blank.</td></tr>
  <tr><td>Dr Amount</td><td>Required</td><td>Enter the debit amount.</td></tr>
  <tr><td>Cr Amount</td><td>Required</td><td>Enter the credit amount.</td></tr>
  <tr><td>Account</td><td>Required</td><td>Enter the account number, including segments.</td></tr>
  <tr><td>Auto Reversal</td><td>Required</td><td>Enter Yes or No, depending on the scenario.</td></tr>
  <tr><td>Currency</td><td>Required</td><td>Enter the transaction currency.</td></tr>
  <tr><td>Company Currency</td><td>Required</td><td>Enter the company currency.</td></tr>
  <tr><td>Ex-Rate</td><td>Required</td><td>Enter the transaction exchange rate.</td></tr>
  <tr><td>Company Ex-rate</td><td>Required</td><td>Enter the company exchange rate.</td></tr>
</table>

# Upload a manual journal entry

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open Journals</h4><p>Go to Import/Export → Journals.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/21fca57289c04939c098a4534744c11c748f7517e55289d45d9351376c7168fb-Image_1.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Create a new entry</h4><p>Select the + icon to create a new manual journal entry.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/af44223b98a4b5ce3dd67c07407a4d4a4ca48068413ba89f065c5ee41494cf8d-Image_2.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Upload your file</h4><p>Upload your prepared manual journal entry file.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Select posting details</h4><p>Choose the Books where the entry should load, and the Period for the entry, such as Sep-25.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">5</div>
    <div><h4>Save</h4><p>Select Save.</p></div>
  </div>
</div>

<div class="rp-callout rp-callout-note">
  <div><strong><i class="fa-solid fa-circle-info" aria-hidden="true"></i> Note</strong>The entry doesn't post immediately. RevRec sets the status to Approval Pending and displays an arrow icon next to the entry.</div>
</div>

# Review and approve the journal entry

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open the pending entry</h4><p>Select the arrow icon next to the uploaded file.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/df3988a3d5aaf619bead3b756a0945843d6baa4262a7898a3bc703b2f6ad40b7-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Open in the Revenue Workbench</h4><p>Open the entry in the Revenue Workbench.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Review the entry</h4><p>Carefully review the debited and credited accounts, amounts, descriptions, and any other relevant values.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Enter review comments</h4><p>Add your review comments.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">5</div>
    <div><h4>Approve or reject</h4><p>Select Approve to post the entry permanently, or Reject to cancel the transaction and prevent it from affecting the books.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/dc468975e9f16752b4ef13e72b7bc7ac315c6104415c558297a6bcf07d2b5dd5-image.png" align="center" width="75%" border={true} />



<Image src="https://files.readme.io/8d357b7e8f1331c5d31e277e7d5b7e6454e005b84bad26100ab7b02e8f61dab3-Image_5.png" align="center" width="75%" border={true} />


Once approved, the process is complete and the transaction appears in reports for the selected period.

## How dates affect recognition

The values in Start Date and End Date determine how RevRec reflects the entry.

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Scenario</td><td>Result</td></tr>
  <tr><td>Start Date and End Date are blank</td><td>RevRec recognizes the full amount in the uploaded period.</td></tr>
  <tr><td>Start Date and End Date are populated</td><td>RevRec reflects the entry in the waterfall based on the provided dates.</td></tr>
</table>

## How auto reversal works

If Auto Reversal is set to Yes, RevRec reverses the current-period entry in the next accounting period.

# Reporting examples

These examples describe common manual journal entry scenarios and where their impact appears in RevRec reports.

## Recognize revenue from liability

Use this entry when revenue is recognized from a liability balance such as deferred revenue.

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Journal impact</td><td>Result</td></tr>
  <tr><td>Debit Liability (Deferred Revenue)</td><td>Decreases deferred revenue, reflecting that the obligation has been fulfilled.</td></tr>
  <tr><td>Credit Revenue</td><td>Increases recognized revenue for the period.</td></tr>
</table>


<Image src="https://files.readme.io/1cadfe15362ce063db69ed8e362893266942beb98287899901984a5b876c4970-Image_6.png" align="center" width="75%" border={true} />


Report impact:

<ul class="rp-list">
  <li>Revenue appears in the Revenue Waterfall Report.</li>
  <li>The reduced liability balance appears in the Liability Balances Report.</li>
</ul>

## Recognize cost (COGS)

Use this entry to recognize cost associated with revenue.

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Journal impact</td><td>Result</td></tr>
  <tr><td>Debit COGS</td><td>Recognizes cost as expense.</td></tr>
  <tr><td>Credit Deferred COGS</td><td>Decreases the deferred cost balance.</td></tr>
</table>


<Image src="https://files.readme.io/20df8138df17b216afa49ad0780111c1d0b562ce1d8097d413a3e1553eda8c4b-Image_7.png" align="center" width="75%" border={true} />


Report impact:

<ul class="rp-list">
  <li>Recognized cost appears in the Cost Waterfall Report.</li>
  <li>The updated deferred cost balance appears in the Cost Balances Report.</li>
</ul>

## Recognize revenue with an asset

Use this entry when revenue is recognized against an asset account, such as accounts receivable.

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Journal impact</td><td>Result</td></tr>
  <tr><td>Debit Asset</td><td>Increases assets, reflecting an amount owed to the company.</td></tr>
  <tr><td>Credit Revenue</td><td>Recognizes revenue for the period.</td></tr>
</table>


<Image src="https://files.readme.io/8dfe10dde3f805909f3b779062daf19c454c25af0e978e2e86bfbafd7e3f869b-Image_8.png" align="center" width="75%" border={true} />


Report impact:

<ul class="rp-list">
  <li>Revenue appears in the Revenue Waterfall Report.</li>
  <li>The asset balance appears in the Asset Balances Report.</li>
</ul>

# Important considerations

Manual journal entries give you precise control, but they also place full responsibility for the entry on the uploader. Keep these points in mind.

<table class="rp-gw-table">
  <tr class="rp-thead-row"><td>Consideration</td><td>Details</td></tr>
  <tr><td>Fully manual process</td><td>RevRec posts the data exactly as provided in the file.</td></tr>
  <tr><td>No automated derivation</td><td>The system doesn't apply revenue rules, data rules, or other configuration logic.</td></tr>
  <tr><td>Segment responsibility</td><td>You must manually enter all applicable segments and reporting dimensions, such as department, product line, region, or cost center.</td></tr>
  <tr><td>Accuracy matters</td><td>Always verify accounts, amounts, dates, currencies, and comments before upload and approval.</td></tr>
</table>

# FAQs

<Accordion title="Does RevRec derive values for a manual journal entry from system rules?">
  No. Manual journal entries are independent from RevRec's automated rules and configurations. You must provide all required values in the upload file.
</Accordion>

<Accordion title="What happens if I leave the start and end dates blank?">
  RevRec recognizes the full amount in the period you selected during upload.
</Accordion>

<Accordion title="What happens if I populate the start and end dates?">
  RevRec reflects the entry in the waterfall based on the dates you provide.
</Accordion>

<Accordion title="Can I reverse a manual journal entry automatically?">
  Yes. Set Auto Reversal to Yes in the upload file to reverse the current-period entry in the next period.
</Accordion>

<Accordion title="Does the journal entry post immediately after upload?">
  No. After upload, the file status changes to Approval Pending. The entry must be reviewed and approved in the Revenue Workbench before it's posted.
</Accordion>

<br />
