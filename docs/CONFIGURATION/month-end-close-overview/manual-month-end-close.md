---
title: Manual month end close
excerpt: >-
  Follow the ordered steps to verify data, reconcile reports, transfer journal
  entries, and manually close a period in Recurly RevRec.
deprecated: false
hidden: false
metadata:
  robots: index
---
<div class="rp-page">
  <div class="rp-overview">Manual month end close gives you full, hands-on control over ending a period in Recurly RevRec. You verify your staged data, clear exception reports, reconcile your balances, transfer journal entries, and then close the period yourself — checking each step before moving on. It's the right fit when you want to catch and resolve discrepancies before the numbers are final.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Part of Recurly RevRec — <a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-advanced" target="_blank">learn more</a></div>
  <div class="rp-cost">
    <strong>Additional cost</strong><br/>
    This feature requires an additional cost. Contact <a href="mailto:support@recurly.com">support@recurly.com</a> or your Recurly account manager for pricing details.
  </div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#definition"><span class="rp-toc-num">1</span>Definition</a>
    <a class="rp-toc-pill" href="#key-benefits"><span class="rp-toc-num">2</span>Key benefits</a>
    <a class="rp-toc-pill" href="#how-to-do-month-end-close"><span class="rp-toc-num">3</span>How to do month end close</a>
  </div>
</div>

# Definition

<div class="rp-definition">Month end close is a formal process that ensures all revenue-related transactions are accurately captured and reconciled before you close one period and open the next. It involves verifying data, checking for exceptions, reconciling reports, and transferring journal entries.</div>

# Key benefits

<div class="rp-benefits">
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-chart-line" aria-hidden="true"></i></div>
    <strong>Accurate financial reporting</strong>
    <span>Ensures your data is complete and consistent for each period.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-circle-check" aria-hidden="true"></i></div>
    <strong>Reduced errors</strong>
    <span>Identifies and resolves exceptions — like holds or missing allocations — before closing.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-diagram-project" aria-hidden="true"></i></div>
    <strong>Streamlined workflows</strong>
    <span>Simplifies reconciling revenue and transferring journal entries.</span>
  </div>
</div>

# How to do month end close

To properly close a month in Recurly RevRec, follow these steps in order. Don't open the next period until each step is complete.

<div class="rp-nav-grid">

<Cards>
  <Card title="1. Stage data verification" href="#stage-data-verification">
    Make sure there are no unprocessed transactions or errors in the contract stage and documents stage reports.
  </Card>
  <Card title="2. Verification of exception reports" href="#verification-of-exception-reports">
    Review SSP and hold exception reports and address any issues requiring allocation or hold removal.
  </Card>
  <Card title="3. Reconciliation of reports" href="#reconciliation-of-reports">
    Compare asset, liability, revenue waterfall, and revenue insight reports to ensure they match.
  </Card>
  <Card title="4. Transferring journal entry" href="#transferring-journal-entry">
    Approve and transfer journal entries to your GL, making sure unaccounted balances are zero.
  </Card>
  <Card title="5. Closing the period" href="#closing-the-period">
    Finalize the current period, open the next, and allow new transactions to flow into RevRec.
  </Card>
</Cards>

</div>

## Stage data verification

Start by confirming your staged data is clean for the open period.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Run the contract stage report</h4><p>Go to Reports → Contract Stage Report for the open period.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/87e66112d016da85db1425dac2c0ac9fcb7cf30aba6a396f5d3e5c3765ef624a-1.Contract_Stage_Details.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Run the documents stage report</h4><p>Go to Reports → Documents Stage Report for the open period.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/97117ef674d798eb66dfa6342a439d17d6b9d176f69c3c08a652e4823df1d48a-2.Doc_Stage_details.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Resolve any errors</h4><p>Verify there are no unprocessed transactions or errors for the current period.</p></div>
  </div>
</div>

Resolve errors before proceeding, or they won't be included in the closed period's numbers. For large datasets, download the reports to assist with troubleshooting.

## Verification of exception reports

Next, clear both exception reports so nothing is unintentionally left out or held back.

### SSP exception report

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open the SSP exception report</h4><p>Go to Reports → Exception Reports and select SSP Exception.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/ba90fdebf651af6f1bf6d75801de58cff58900bd70993d0b9de65ad51dabf11a-3.SSP_Exception_Report.png" align="center" width="75%" border={true} />


Ensure no contracts that require Standalone Selling Price (SSP) allocation are listed. If a contract needs allocation, create a new SSP with an active date preceding the contract date, then re-run allocation using the Revenue Workbench.

### Hold exception report

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Open the hold exception report</h4><p>Go to Reports → Exception Reports and select Hold Exception.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/f678cd64d5f85d4a1de45f5e816b37fad181a38f93261eff64862dd640ec9556-4.Hold_Exception_Report.png" align="center" width="75%" border={true} />


Confirm that any items on hold are meant to be on hold. If you need to remove a hold so revenue is recognized, open the contract in the Revenue Workbench and manually release the appropriate amount.

## Reconciliation of reports

Now confirm your key reports agree with one another before touching journal entries.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Run the balance and waterfall reports</h4><p>Run the asset report, liability report, and revenue waterfall report for the period.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/21a29e5ad17413c5553ef71524026df005eda591edc6fe001255f589f92a4c78-5.Scheduled_Reconcillation.png" align="center" width="75%" border={true} />


The sum of the scheduled columns in the asset and liability reports should match the total in the revenue waterfall for the period.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Run the revenue insight report</h4><p>The scheduled balance in the revenue insight report should also match the revenue waterfall total.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/2c2b5e7d9af9cb5e852dbdd3468716ca1a03b33b390e819e05e616e88187de1f-9.Revenue_Insight_Report.png" align="center" width="75%" border={true} />


Confirm these reports are aligned before proceeding.

## Transferring journal entry

With everything reconciled, approve and transfer your journal entries to the general ledger.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open Transfer JE</h4><p>Go to Import/Export → Transfer JE.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/ed967fb23929f3f05476e069c06f13d53ba90ebab399153bd527a37fd50d50f3-11.Transfer_JE.png" align="center" width="40%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Approve the primary book journal for transfer</h4><p>Select the journal card for the primary book, review the entries, and select Approve for Transfer. Then mark the journal as transferred.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/299a36179bef07272c8ad2e76b4f1598154c44af4fbac4c32f53fc7d1610ca69-12.Primary_book_-_trasnfer_JE.png" align="center" width="40%" border={true} />



<Image src="https://files.readme.io/292913e82c3ece3bca035d243f90a9437e71563e31eb00bc0cc8e85bed1a9b4c-13.Transfer_JE_-_Approve_for_Transfer.png" align="center" width="75%" border={true} />



<Image src="https://files.readme.io/6c9fe2bee1f74a222221b94f45a536046c836ff8afc943465fc4772e0b5a7418-14.Transfer_JE_-_Mark_as_Transferred.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Confirm the entries land in your accounting system</h4><p>If you're pulling data via API, confirm it populates in your accounting system. If manual, download the journal entry and upload it based on your internal process.</p></div>
  </div>
</div>

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Verify unaccounted balances are zero</h4><p>Wait for the reports to refresh — it may take up to an hour for large datasets — then re-run the asset and liability reports. The Unaccounted columns should be zero before proceeding.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/03ac05643b3584c4fe203f6adaac605ce04560660685bf0d21b6d4d483ee64ad-15.Unaccounted_Total.png" align="center" width="75%" border={true} />


## Closing the period

Finally, close the current period and open the next one.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open period close</h4><p>Go to Import/Export → Period Close.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/dcae5e6085c4bcc3e5c6bcac59e09bdfb2b2e36336411b18f570a8601888adb2-16.Period_Close_-_Imp_Export.png" align="center" width="40%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Open the new period</h4><p>Select Open New Period (top right) and follow the prompts until the next period is open. Once closed, the system triggers new-period transactions to flow into RevRec.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/6c29367a76fc2e663832c620697cf4c29664ccf10c630c9b44bc8872a253521c-17.Period_close_-_Open_next.png" align="center" width="75%" border={true} />


<div class="rp-callout rp-callout-note">
  <div><strong><i class="fa-solid fa-circle-info" aria-hidden="true"></i> Note</strong>Before opening the next period, ensure all unaccounted balances are zero. If you see any remaining items, investigate and resolve them first.</div>
</div>

<br />
