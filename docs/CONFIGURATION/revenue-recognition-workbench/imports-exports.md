---
title: Imports and exports
excerpt: >-
  Use the Import/Export tool in Recurly RevRec to upload transactions, events,
  and cost files, manage the stage area, transfer journal entries, and close
  periods.
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
  <div class="rp-overview">The Import/Export feature in Recurly RevRec provides a structured platform to import and export data types including sales orders, billings, and cost files. Use it to upload transactions, process events, manage unprocessed files in the Stage Area, transfer journal entries, and close periods — keeping your financial data accurate and your month-end process on track. This feature is part of Recurly RevRec. <a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-advanced" target="_blank">Learn more</a>.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Available as part of Recurly RevRec</div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#key-benefits"><span class="rp-toc-num">1</span>Key benefits</a>
    <a class="rp-toc-pill" href="#transactions"><span class="rp-toc-num">2</span>Transactions</a>
    <a class="rp-toc-pill" href="#events"><span class="rp-toc-num">3</span>Events</a>
    <a class="rp-toc-pill" href="#stage-area"><span class="rp-toc-num">4</span>Stage area</a>
    <a class="rp-toc-pill" href="#transfer-je"><span class="rp-toc-num">5</span>Transfer JE</a>
    <a class="rp-toc-pill" href="#period-close"><span class="rp-toc-num">6</span>Period close</a>
  </div>
</div>

### Prerequisites

<ul class="rp-list">
  <li>An active Recurly account with administrative privileges.</li>
  <li>Familiarity with the data types and structures used in your business operations.</li>
  <li>Access to the source files intended for import or the destination directories for exports.</li>
</ul>

### Limitations

<ul class="rp-list">
  <li>The import/export tool may have file size restrictions to keep uploads and downloads efficient.</li>
  <li>Any changes you make apply to future transactions only.</li>
  <li>The system may require specific file formats for a successful data import.</li>
  <li>Real-time synchronization may not be available — data sync may occur at scheduled intervals.</li>
</ul>

# Key benefits

<div class="rp-benefits">
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-database" aria-hidden="true"></i></div>
    <strong>Data consistency</strong>
    <span>Keep your Recurly data consistent with other platforms or databases you use.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-clock" aria-hidden="true"></i></div>
    <strong>Time efficiency</strong>
    <span>Eliminate manual data entry to save time and reduce potential errors.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-chart-bar" aria-hidden="true"></i></div>
    <strong>Enhanced reporting</strong>
    <span>Import all necessary data to generate comprehensive reports with deeper insights into your operations.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-sliders" aria-hidden="true"></i></div>
    <strong>Flexibility</strong>
    <span>Export your data whenever needed, regardless of platform.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-rotate" aria-hidden="true"></i></div>
    <strong>Streamlined operations</strong>
    <span>Regular data synchronization keeps all departments working with the latest data.</span>
  </div>
</div>

# Transactions

In Recurly RevRec, you can upload sales orders, billings, and cost files. These files are the backbone of revenue recognition and integral to financial reporting.

<div class="rp-callout rp-callout-note">
  <div><strong><i class="fa-solid fa-circle-info" aria-hidden="true"></i> Note</strong>For a successful upload, column headings in your file must match the upload names specified in the attribute mapper of Recurly RevRec. Any discrepancies can prevent the file from loading.</div>
</div>

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open Transactions</h4><p>Access the Import/Export section and select "Transactions."</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Upload your file</h4><p>Select the "+" icon to add your transaction file. After uploading, save the file.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/d9290f3-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Verify column headings</h4><p>Confirm that the column headings in your file align with the system's attribute labels.</p></div>
  </div>
</div>

Once saved, transaction files appear as cards on the left side of the transaction import window.


<Image src="https://files.readme.io/98ebb91-image.png" align="center" width="75%" border={true} />


After a successful upload, transaction files can be accessed and reviewed in the Revenue Workbench for a comprehensive overview of your revenue data.

<div class="rp-callout rp-callout-note">
  <div><strong><i class="fa-solid fa-circle-info" aria-hidden="true"></i> Billing file details</strong>
    <ul>
      <li>Supported document types for billing file uploads are INV (invoice), IVC (invoice cancellation), CM (credit memo), and CMC (credit memo cancellation). Partial credit memos are allowed, but partial invoice cancellations are not permitted.</li>
      <li>The system collects transactions belonging to the current open period and previous periods. Transactions for future periods are placed in the Stage Area and processed once the corresponding period is opened.</li>
    </ul>
  </div>
</div>

# Events

Before uploading an event file in Recurly RevRec, ensure the file has been linked with a POB (Performance Obligation) template. This linkage is required for proper event mapping and accurate revenue recognition aligned with contractual obligations.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open Events</h4><p>Navigate to the Import/Export section and select "Events."</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Start a new upload</h4><p>Select the "+" button to initiate the upload process for a new event file.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/b5d085e-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Name the file and select the event</h4><p>Assign a name to the event file — by default the system uses the uploaded file's name. Then select the relevant event from the dropdown menu. These are predefined event templates established in the system.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Save</h4><p>Once all details are populated, save the file. The system processes the uploaded event file according to the configurations set for that event, ensuring accurate and compliant revenue recognition.</p></div>
  </div>
</div>

# Stage area

The Stage Area contains four tabs — Contracts, Documents, Cost, and Events. Unprocessed files appear under their respective tabs. Files may remain unprocessed for the following reasons:

<ul class="rp-list">
  <li><strong>Error in the file:</strong> If errors are encountered during upload, those files are placed in the Stage Area. The system displays error messages for each transaction indicating the issue to address.</li>
  <li><strong>Future transactions:</strong> Transactions with a future date or period are held in the Stage Area until the applicable period is opened in the system.</li>
  <li><strong>Scheduled processing:</strong> If the scheduled jobs for transaction or event import are inactive or not running, transactions may remain stuck in the Stage Area. Ensure scheduled jobs are active and properly configured.</li>
</ul>

## Viewing and deleting data in the Stage Area

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open the Stage Area</h4><p>Navigate to Import/Export to access the Stage Area.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Filter files</h4><p>Use the Status tab to filter and view files based on specific criteria.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Delete data</h4><p>To remove specific data, select the transaction under its respective tab, select the Delete icon, and confirm the deletion. Save your changes to finalize the removal.</p></div>
  </div>
</div>

# Transfer JE

<div class="rp-callout rp-callout-note">
  <div><strong><i class="fa-solid fa-circle-info" aria-hidden="true"></i> Note</strong>The month-end close process is a structured two-step approach. The first step involves transferring and verifying journal entries — laying the foundation for a confident period closure.</div>
</div>

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Navigate to Transfer JE</h4><p>Go to Import/Export → Transfer JE.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Open the journal card</h4><p>Select the journal card of the primary book to access its journal entries.</p></div>
  </div>
</div>

## Reconciliation checks

Before finalizing the transfer, run the following reports to verify all entries are accurate.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Run the Asset Report</h4><p>Generate the Asset Report for the period. Verify that the total of the scheduled column in the asset account matches the total in the revenue waterfall report.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Run the Liability Report</h4><p>Generate the Liability Report for the period. Confirm that the total of the scheduled column in the liability account matches the total in the revenue waterfall report.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Run the Revenue Waterfall Report</h4><p>Generate the Revenue Waterfall Report for the period. Validate that the total amount in the waterfall matches the combined total of the scheduled columns in both the asset and liability accounts.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Run the Revenue Insight Report</h4><p>Generate the Revenue Insight Report. Verify that the scheduled balance matches the total in the revenue waterfall report for the period.</p></div>
  </div>
</div>

## Finalizing the transfer

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Approve for Transfer</h4><p>Select "Approve for Transfer" for the journal card of the Primary book to indicate the entries have been reviewed and approved.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Mark as transferred</h4><p>Once approved, select "Mark as Transferred" to confirm the journal entries have been successfully transferred and recorded.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Wait for summarization</h4><p>Before proceeding, ensure the journal card is summarized. This consolidates the entries for accurate reporting. Don't move to the next step until summarization is complete.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/250214f-image.png" align="center" width="75%" border={true} />


# Period close

After transferring journal entries, the final step is to close the period.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open Period Close</h4><p>Access the Period Close option via Import/Export.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Open the next period</h4><p>Select "Open New Period."</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Confirm and proceed</h4><p>Confirm the action and allow the system to transition to the next period, ensuring continuity in your financial operations.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/993b248-image.png" align="center" width="75%" border={true} />


<br />
