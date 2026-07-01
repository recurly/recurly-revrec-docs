---
title: Automatic month end close
excerpt: >-
  Use the Period Close Checklist in Recurly RevRec to finalize data, transfer
  journals, reconcile balances, and automatically close each period.
deprecated: false
hidden: false
metadata:
  robots: index
---
<div class="rp-page">
  <div class="rp-overview">Automatic month end close walks you through a Period Close Checklist that finalizes your data before the books close. Recurly RevRec starts you with four system-defined tasks — data processing, staging checks, journal transfers, and report reconciliation — and lets you add your own custom tasks on top. Once every required task is complete, the system closes the current period and opens the next one for you.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Part of Recurly RevRec — <a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-advanced" target="_blank">learn more</a></div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#definition"><span class="rp-toc-num">1</span>Definition</a>
    <a class="rp-toc-pill" href="#the-period-close-checklist"><span class="rp-toc-num">2</span>The Period Close Checklist</a>
    <a class="rp-toc-pill" href="#how-to-close-the-period"><span class="rp-toc-num">3</span>How to close the period</a>
    <a class="rp-toc-pill" href="#faqs"><span class="rp-toc-num">4</span>FAQs</a>
  </div>
</div>

# Definition

<div class="rp-definition">The Period Close Checklist is a set of tasks — both system-defined and user-defined — required to finalize each open period in Recurly RevRec. Working through it ensures your data is complete, journals are transferred, and balances are reconciled before you close a period.</div>

# The Period Close Checklist

Recurly RevRec includes a Period Close Checklist to keep period closures accurate and efficient. It begins with four system-defined tasks and can be expanded with any custom tasks you need.


<Image src="https://files.readme.io/e5684605bed5eeb29626cfb74bddd32d2305b6e5a007bde21a9ea74563147aec-4._System_Defined_Tasks.png" align="center" width="40%" border={true} />


## System-defined tasks

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Data processed for the current open period</h4><p>Ensures all Recurly invoices, credits, and voids are transferred into RevRec, including data up to the period's end date. This task cannot be skipped.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Billing pending processing or stuck in stage</h4><p>Identifies transactions stuck in the Order or Doc Stage tables for the current open period, which you must investigate and resolve.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Transfer journals</h4><p>Ensures that all batches containing journals are approved and summarized for the current period. Open batches without journals can remain open.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Review the accounted reports</h4><p>Confirms the accuracy of journal entries and reconciles beginning and ending balances. Verifies that the liability balance plus asset balance matches the revenue workflow for the current open month.</p></div>
  </div>
</div>

## Creating user-defined tasks

You can create any number of user-defined tasks essential for period close.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open the period task screen</h4><p>Go to Setup → Period Task.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/d71ad5d26e258a599e71f5f7a2600a822edb5750c1e16c93c8f67036971c39b2-1._Period_Task.png" align="center" width="40%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Add a task</h4><p>Select the "+" button.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Name the task</h4><p>Enter a task name.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Set required or optional</h4><p>Choose whether the task is Required or Optional.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/fcb1c2c356433e70d4af97013f4f31d943576d776ad01c5310f29725a44c8699-2._New_Task.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">5</div>
    <div><h4>Define the activation period</h4><p>Set the activation period — tasks activate in the subsequent period.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">6</div>
    <div><h4>Save your changes</h4><p>Save the task to add it to the checklist.</p></div>
  </div>
</div>

If needed, reorder tasks by selecting the "⋮" icon on the bottom right.


<Image src="https://files.readme.io/645c32df97dbf8e54bb01e00817febf42e64b46a152a7492df8b52b94bb3fdb0-3._Hierarchy_change.png" align="center" width="75%" border={true} />


# How to close the period

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Navigate to period close</h4><p>Go to Import/Export → Period Close.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Initiate period close</h4><p>Select Initiate Period Close. Only do this after the open period has concluded.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/ab01604cf77a9c63e0213c6478101aa15ed2a6829c18f39c628164369e3eb7fd-Screenshot_2025-06-27_at_9.08.42_AM.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Confirm period close</h4><p>In the dialog box that appears, enter any necessary message or comment, then select Close Period to confirm and begin the automated close process.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/44a525a8455f53f840096291d8901fe552f8e3711a3cb1c71a3583e84545761b-6.Comments.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>System checks run automatically</h4><p>The system runs a "period close automated" job to verify your data before closing.</p></div>
  </div>
</div>

The automated job confirms that:

<ul class="rp-list">
  <li>All invoices from Recurly are transferred into RevRec.</li>
  <li>Data in contract stage, doc stage, and cost stage is fully processed.</li>
  <li>Transfer JEs are summarized.</li>
  <li>Accounted reports are reconciled with RevRec Essentials.</li>
</ul>

Refer to the <a href="#the-period-close-checklist">Period Close Checklist</a> for details on each automated check.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">5</div>
    <div><h4>Complete user-defined tasks</h4><p>Review each user-defined task and mark it Complete when finalized. Add comments or file attachments as an audit trail for future reference.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">6</div>
    <div><h4>Skip optional tasks if needed</h4><p>Set any optional tasks to Skipped if you don't need to complete them.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/5802364502736289fb780bb5f62e681e53e78a040c3d823d3d61080782258d8a-7._Perid_Close_-_Step_4.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">7</div>
    <div><h4>Automatic close and next period open</h4><p>Once all required tasks are complete, the system automatically closes the current period and opens the next one. The final screen shows the period as closed and all tasks as completed.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/d27624399376acf0cd8a8026d2f19a8d7a1c080bc953a79e5f16294dbeaee9c5-8._Point_6.png" align="center" width="75%" border={true} />


<div class="rp-callout rp-callout-important">
  <div><strong><i class="fa-solid fa-circle-exclamation" aria-hidden="true"></i> Important</strong>The system needs 30–60 minutes for data to synchronize. After making corrections, wait up to an hour before selecting Retry or contacting Support.</div>
</div>

With all tasks finalized, you'll close the period in Recurly RevRec — keeping your end-of-period process accurate and compliant.

# FAQs

## Period close process

<Accordion title="What is the checklist or process for the period close?">
  The Period Close checklist, in Administration, guides you through finalizing data and controls for the period. Follow the ordered system and user tasks to ensure compliance and a complete close.
</Accordion>

## General period close errors

<Accordion title="What does the error in the system task 'Data processed for the current open period' mean?">
  **Problem:** Recurly invoices for the current open period haven't been successfully transferred into RevRec.

  **Solution:** Initiate the billing integration job to synchronize the missing invoices. After the integration completes successfully, select Retry. The system won't allow the period close to proceed until all invoices are synced.
</Accordion>

<Accordion title="What does the error in the system task 'Billing pending processing or stuck in stage' mean?">
  **Problem:** Billing data or other uploaded transaction data for the current or a previous open period is stuck in the staging area and hasn't been processed.

  **Solution:**
  - Generate stage reports via Reports → Stage to find the specific transactions that are stuck.
  - Review and process the stuck data to resolve any underlying errors.
  - Once the data flows correctly into RevRec, select Retry on the period close task to continue.

  See the <a href="#contract-stage-errors">contract stage error FAQs</a> below to understand how to resolve stage data errors.
</Accordion>

<Accordion title="What does the error in the system task 'Transfer Journals' mean?">
  **Problem:** Transfer journal cards for the primary book haven't been approved or summarized.

  **Solution:**
  - Go to Import/Export → Transfer JE to locate journals that are still open.
  - Approve and summarize all open journals.
  - Select Retry. This ensures all journal entries are properly accounted for before closing the period.
</Accordion>

<Accordion title="What does the error in the system task 'Review the Accounted Reports' mean?">
  **Problem:** There are summarization issues or balance discrepancies in key financial reports.

  **Solution:**
  - Review the roll-forward reports (liability and asset balances) and verify that all Unaccounted columns show zero.
  - Confirm that the beginning balance for the current period matches the ending balance from the previous period.
  - Check that the revenue waterfall aligns with the scheduled balances.
  - If you can't identify the specific report causing the issue, contact Recurly Support for assistance.
</Accordion>

<Accordion title="Is it possible to reopen a closed period?">
  No — a period that has been closed cannot be reopened. As a workaround, any transactions that belong to a closed period can be loaded into the current open period.
</Accordion>

<Accordion title="Will the period close process allow closing the period if invoices haven't been integrated?">
  No. The period close process blocks closing until all relevant invoices have been integrated.
</Accordion>

<Accordion title="The data in the stage area isn't needed, but the system is preventing the period close. What can be done?">
  **Problem:** The system won't allow the period to close while there's still data in the staging area, even if that data is unnecessary.

  **Solution:** If the stage data isn't required, manually delete it (see <a href="https://docs.recurly.com/docs/imports-exports#how-to-view-and-delete-data-in-the-stage-area" target="_blank">how to view and delete data in the stage area</a>). The period close process continues once the stage is empty.
</Accordion>

<Accordion title="What does the system check during the validation step?">
  The system task verifies:
  - Unaccounted = 0 in the liability balance and asset balance reports.
  - Current beginning balance = prior ending balance for those reports.
  - Revenue waterfall total matches scheduled balances.
</Accordion>

<Accordion title="Can I skip a user-created task?">
  A user-created task can only be skipped if it was marked Optional when it was created. Mandatory tasks can't be skipped.
</Accordion>

<Accordion title="Can I add a new user task for the current period?">
  No. A user task added during the current period becomes visible and active starting next period. You can't add a new task to a period already in progress.
</Accordion>

<Accordion title="Can I delete a user task in the current period?">
  Yes, but the deletion takes effect next period. The task remains part of the current period's checklist.
</Accordion>

<Accordion title="Can I close a future period?">
  No. The period close process only allows closing periods prior to the current calendar month. You can't close the current month or any future months in advance.
</Accordion>

<Accordion title="Why, if I made corrections, can I still not close the period?">
  The system may require 30–60 minutes for data to synchronize. Wait up to an hour before retrying.
</Accordion>

## Contract stage errors

These errors occur during the initial contract processing stage.

<Accordion title="What does the 'Debit Account is Blank' or 'Credit Account is Blank' error mean?">
  **Reason:** A transaction line is missing its assigned debit or credit account.

  **Solution:** Review system configurations and assign the correct accounts to the relevant lines.
</Accordion>

<Accordion title="Why am I seeing the error 'Updated SO Amount is in a different sign than previous Billed Amount'?">
  **Reason:** An updated sales order (SO) uses a sign (positive or negative) different from the original SO.

  **Solution:** Ensure the updated SO amount uses the same sign as the original.
</Accordion>

<Accordion title="What causes the 'Error Processing SO update'?">
  **Reason:** For a Credit Memo Request (CMR), the updated SO amount is less than the amount already billed.

  **Solution:** Verify the SO update amount and ensure it isn't less than the billed amount.
</Accordion>

<Accordion title="What does 'Updated SO Amount is less than Billed Amount' mean?">
  **Reason:** The total billed amount for a line exceeds the SO amount.

  **Solution:** Increase the SO amount to match or exceed the billed amount.
</Accordion>

<Accordion title="Why am I getting the 'Bundle child updates are not allowed' error?">
  **Reason:** Direct updates to bundle child lines aren't permitted.

  **Solution:** Make updates on the parent bundle line.
</Accordion>

<Accordion title="How do I fix 'POB Rule setup is missing in the book' or 'POB setup missing for some lines in this contract in book'?">
  **Reason:** One or more contract lines don't have a Performance Obligation (POB) rule configured.

  **Solution:** Configure the appropriate POB rules for all missing lines. Note: if any line in the contract has no POB assigned, all lines will be stuck in stage.
</Accordion>

## Doc stage errors

These errors typically occur when processing documents like invoices and credit memos.

<Accordion title="What should I do about an 'Invalid References on INV' error?">
  **Reason:** The reference invoice number or reference invoice line number is incorrect.

  **Solution:** Correct the reference invoice details.
</Accordion>

<Accordion title="Why did I get the error 'Invalid INV. INV belongs to Material Right Contract'?">
  **Reason:** An invoice was associated with a Material Right contract line, and those invoices can't be collected.

  **Solution:** Remove the invoice information from the Material Right line.
</Accordion>

<Accordion title="How do I resolve a 'Bill Amount is incorrect' error?">
  **Reason:** The bill amount is incorrect.

  **Solution:** Validate and correct the bill amount.
</Accordion>

<Accordion title="What does 'Original Credit Memo does not exist or already Cancelled' mean?">
  **Reason:** You attempted to cancel a credit memo with reference details that don't match an existing, active credit memo.

  **Solution:** Re-upload the cancellation file with the correct reference details.
</Accordion>

<Accordion title="How do I fix 'Original Invoice does not exist or already Cancelled' or 'Original Invoice does not exist'?">
  **Reason:** A credit memo references an invoice that doesn't exist or is already cancelled.

  **Solution:** Correct the reference invoice details and re-process.
</Accordion>

<Accordion title="Why am I seeing 'Invalid INV. SO not present in System'?">
  **Reason:** An invoice references a sales order (SO) that isn't in the system.

  **Solution:** Re-process with a valid, existing SO number.
</Accordion>

<Accordion title="What should I do for an 'Error Loading SO Line'?">
  **Reason:** The associated SO line hasn't been successfully processed from the contract stage.

  **Solution:** Process the SO in the contract stage successfully before loading the invoice.
</Accordion>

<Accordion title="How do I resolve 'CM cannot be processed as INV is in error'?">
  **Reason:** A credit memo (CM) was submitted against an invoice that's currently in an error state in stage.

  **Solution:** Resolve the invoice error first, then process the CM.
</Accordion>

<Accordion title="What causes the 'Cumulative bill amount is over sell price' error?">
  **Reason:** The total invoice value for a subscription exceeds the sell price, and over-billing isn't allowed.

  **Solution:** Go to Profiles → Overage and enable the overage setting.
</Accordion>

## Cost stage errors

These errors occur during the processing of cost-related data.

<Accordion title="What does 'Invalid Cost, SO not present in System' mean?">
  **Reason:** The SO number in the cost file is incorrect or doesn't exist.

  **Solution:** Verify the SO number and re-upload.
</Accordion>

<Accordion title="Why am I seeing 'Bundle child updates are not allowed' in the Cost Stage?">
  **Reason:** Direct updates to bundle child lines aren't allowed for costs either.

  **Solution:** Update costs on the parent bundle line.
</Accordion>

<Accordion title="How do I fix 'Invalid Cost Type, Cost Type Setup is missing'?">
  **Reason:** The specified cost type hasn't been configured.

  **Solution:** Configure the cost type correctly, then re-process.
</Accordion>

<Accordion title="What does 'Allocated Commission lines cannot be updated' mean?">
  **Reason:** Once commission is allocated to a line, that line can't be updated.

  **Solution:** Avoid updating lines with allocated commission. Use a new transaction or reversal if needed.
</Accordion>

<br />
