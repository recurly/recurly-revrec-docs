---
title: Automatic month end close
excerpt: >-
  A succinct checklist to guide and streamline your period close process in
  Recurly RevRec, from system-defined tasks to custom, site-specific
  requirements.
deprecated: false
hidden: false
metadata:
  robots: index
---
# Overview

### Required plan

This feature is part of our product, Recurly RevRec. [<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-advanced" target="_blank">Learn more here</a>].

# Definition

**Period Close Checklist** refers to a set of tasks—both system-defined and user-defined—required to finalize each open period in Recurly RevRec. This ensures that data is complete, journals are transferred, and balances are reconciled before closing a period.

# Key details

## Period Close Checklist in Recurly Revenue Recognition

Recurly Revenue Recognition includes a **Period Close Checklist** to ensure accurate and efficient period closures. The checklist begins with **four system-defined tasks** and can be expanded with your own custom tasks.

<Image align="center" border={true} width="40% " src="https://files.readme.io/e5684605bed5eeb29626cfb74bddd32d2305b6e5a007bde21a9ea74563147aec-4._System_Defined_Tasks.png" className="border" />

### System-Defined Tasks

1. **Data processed for the current open period**: Ensures all Recurly invoices, credits, and voids are transferred into RevRec, including data up to the period’s end date. _(This task cannot be skipped.)_

2. **Billing Pending Processing or Stuck in Stage**: Identifies transactions stuck in the **Order** or **Doc Stage** tables for the current open period, which you must investigate and resolve.

3. **Transfer Journals**: Ensures that all batches containing journals are approved and summarized for the current period. Open batches without journals can remain open.

4. **Review the Accounted Reports**: Confirms the accuracy of journal entries and reconciles beginning and ending balances. Verifies that the **Liability Balance plus Asset Balance** matches the **Revenue Workflow** for the current open month.

### Creating User-Defined Tasks

You can create any number of user-defined tasks essential for period close:

1. Go to **Setup → Period Task**.

<Image align="center" border={true} width="30% " src="https://files.readme.io/d71ad5d26e258a599e71f5f7a2600a822edb5750c1e16c93c8f67036971c39b2-1._Period_Task.png" className="border" />

2. Click the **"+"** button.
3. Enter a **Task Name**.
4. Choose **Required** or **Optional**.

<Image align="center" border={true} width="80% " src="https://files.readme.io/fcb1c2c356433e70d4af97013f4f31d943576d776ad01c5310f29725a44c8699-2._New_Task.png" className="border" />

5. Define the **Activation Period** (tasks activate in the subsequent period).
6. **Save** your changes.

If needed, reorder tasks by clicking the "**⋮**" icon on the bottom right.

<Image align="center" border={true} width="70% " src="https://files.readme.io/645c32df97dbf8e54bb01e00817febf42e64b46a152a7492df8b52b94bb3fdb0-3._Hierarchy_change.png" className="border" />

<br />

***

# How to close the period

1. **Navigate to** **Import/Export → Period Close**.
2. **Click “Initiate Period Close.”**
   * Perform this step only after the open period has concluded.

<Image align="center" border={true} width="80% " src="https://files.readme.io/ab01604cf77a9c63e0213c6478101aa15ed2a6829c18f39c628164369e3eb7fd-Screenshot_2025-06-27_at_9.08.42_AM.png" className="border" />

3. **Confirm period close**
   * A dialogue box will appear.
   * Enter any necessary message/comment.
   * Click **“Close Period”** to confirm and begin the automated close process.

<Image align="center" border={true} width="70% " src="https://files.readme.io/44a525a8455f53f840096291d8901fe552f8e3711a3cb1c71a3583e84545761b-6.Comments.png" className="border" />

<br />

4. **System Checks**

* The system runs a **“period close automated”** job to verify:
* All invoices from Recurly are transferred into RevRec.
* Data in contract stage, doc stage, and cost stage are fully processed.
* Transfer JEs are summarized.
* Accounted reports are reconciled with RevRec Essentialss.
* Refer to the “Period Task” section for details on each automated check.

5. **Complete User-Defined Tasks**

* Review each user-defined task.
* Mark each task as **“Complete”** when finalized.
* Add comments or file attachments as an **audit trail** and for future reference.

6. **Optional tasks** may be set to **Skipped** if you do not need to complete them.

<Image align="center" border={true} width="70% " src="https://files.readme.io/5802364502736289fb780bb5f62e681e53e78a040c3d823d3d61080782258d8a-7._Perid_Close_-_Step_4.png" className="border" />

7. **Automatic Close & Next Period Open**
   * Once **all required tasks** are complete, the system automatically closes the **current period** and opens the **next one**.
   * The final screen will display the period as closed and all tasks as completed.

<Image align="center" border={true} src="https://files.readme.io/d27624399376acf0cd8a8026d2f19a8d7a1c080bc953a79e5f16294dbeaee9c5-8._Point_6.png" className="border" />

## **Important note on data synchronization**

* The system requires **30–60 minutes** for data to synchronize.
* After making any corrections, please wait up to an hour before clicking “Retry” or contacting Support.

With all tasks finalized, you’ll successfully close the period in Recurly RevRec, ensuring an accurate and compliant end-of-period process.

***

# FAQs

## Period close process

### What is the checklist or process for the period close?

**Answer:** The **Period Close** checklist (in **Administration**) guides you through finalizing data and controls for the period. Follow the ordered system and user tasks to ensure compliance and complete close.

***

## General period close errors

### What does the error in the system task "Data processed for the current open period" mean?

**Problem:** Recurly invoices for the current open period have not been successfully transferred into RevRec.
**Solution:** Initiate the billing integration job to synchronize the missing invoices. After the integration completes successfully, click **Retry**. The system will not allow the period close to proceed until all invoices are synced.

### What does the error in the system task “Billing pending processing or Stuck in Stage” mean?

**Problem:** Billing data or other uploaded transaction data for the current or a previous open period is stuck in the staging area and has not been processed.
**Solution:**

* Generate Stage Reports via **Reports → Stage** to find the specific transactions that are stuck.
* Review and process the stuck data to resolve any underlying errors.
* Once the data flows correctly into RevRec, click **Retry** on the period close task to continue.
  **Please note:** Refer to the [stage data error FAQs](period-close-checklist#contract-stage-errors) below for understanding how to resolve the stage data errors.

### What does the error in the system task “Transfer Journals” mean?

**Problem:** Transfer Journal Cards for the **primary book** have not been **approved** or **summarized**.
**Solution:**

* Go to **Import/Export → Transfer JE** to locate journals that are still open.
* **Approve and summarize** all open journals.
* Click **Retry**. This ensures all journal entries are properly accounted for before closing the period.

### What does the error in the system task “Review the Accounted Reports” mean?

**Problem:** There are summarization issues or balance discrepancies in key financial reports.
**Solution:**

* Review the roll-forward reports (**Liability** and **Asset Balances**) and verify that all **Unaccounted** columns show zero.
* Confirm that the **Beginning Balance** for the current period matches the **Ending Balance** from the previous period.
* Check that the **Revenue Waterfall** aligns with the scheduled balances.
* If you cannot identify the specific report causing the issue, contact **Recurly Support** for assistance.

### Is it possible to reopen a closed period?

**Answer:** **No**, a period that has been closed cannot be reopened.
**Workaround:** Any transactions that belong to a closed period can be loaded into the **current open period**.

### Will the new period close process allow closing the period if invoices haven't been integrated?

**Answer:** **No.** The period close process blocks closing until all relevant invoices have been integrated.

### The data in the stage area is not needed, but the system is preventing the period close. What can be done?

**Problem:** The system will not allow the period to be closed while there is still data in the staging area, even if that data is unnecessary.
**Solution:** If the stage data is not required, **manually delete it** (see directions [here](https://docs.recurly.com/docs/imports-exports#how-to-view-and-delete-data-in-the-stage-area)). The period close process will only continue once the stage is empty.

### What does the system check during the validation step?

**Answer:** The system task verifies:

* **Unaccounted = 0** in **Liability Balance** and **Asset Balance** reports.
* Current **Beginning Balance = Prior Ending Balance** for those reports.
* **Revenue Waterfall** total matches scheduled balances.

### Can I skip a user-created task?

**Answer:** A user-created task can only be skipped if it was marked as **optional** during its creation. Mandatory tasks cannot be skipped.

### Can I add a new user task for the current period?

**Answer:** **No.** A user task added during the current period becomes visible and active starting **next period**. You cannot add a new task to a period already in progress.

### Can I delete a user task in the current period?

**Answer:** **Yes**, but the deletion takes effect **next period**. The task remains part of the current period’s checklist.

### Can I close a future period?

**Answer:** **No.** The period close process only allows closing periods **prior to the current calendar month**. You cannot close the current month or any future months in advance.

### Why, if I made corrections, can I still not close the period?

**Answer:** The system may require **30–60 minutes** for data to synchronize.

***

## Contract stage errors

These errors occur during the initial contract processing stage.

### What does the "Debit Account is Blank" or "Credit Account is Blank" error mean?

**Reason:** A transaction line is missing its assigned debit or credit account.
**Solution:** Review system configurations and assign the correct accounts to the relevant lines.

### Why am I seeing the error "Updated SO Amount is in a different sign than previous Billed Amount"?

**Reason:** An updated Sales Order (SO) uses a sign (positive/negative) different from the original SO.
**Solution:** Ensure the updated SO amount uses the **same sign** as the original.

### What causes the "Error Processing SO update"?

**Reason:** For a Credit Memo Request (CMR), the updated SO amount is **less** than the amount already billed.
**Solution:** Verify the SO update amount and ensure it is **not less** than the billed amount.

### What does "Updated SO Amount is less than Billed Amount" mean?

**Reason:** The total billed amount for a line exceeds the SO amount.
**Solution:** Increase the SO amount to **match or exceed** the billed amount.

### Why am I getting the "Bundle child updates are not allowed" error?

**Reason:** Direct updates to bundle **child** lines aren’t permitted.
**Solution:** Make updates on the **parent bundle** line.

### How do I fix "POB Rule setup is missing in the book" or "POB setup missing for some lines in this contract in book"?

**Reason:** One or more contract lines do not have a **POB rule** configured.
**Solution:** Configure the appropriate **POB rules** for all missing lines.
**Please note:** If **any** line in the contract has no POB assigned, **all** lines will be stuck in Stage.

***

## Doc stage errors

These errors typically occur when processing documents like invoices and credit memos.

### What should I do about an "Invalid References on INV" error?

**Reason:** The reference invoice number or reference invoice line number is incorrect.
**Solution:** Correct the reference invoice details.

### Why did I get the error "Invalid INV. INV belongs to Material Right Contract"?

**Reason:** An invoice was associated with a **Material Right** contract line; those invoices can’t be collected.
**Solution:** Remove the invoice information from the **Material Right** line.

### How do I resolve a "Bill Amount is incorrect" error?

**Reason:** The bill amount is incorrect.
**Solution:** Validate and correct the bill amount.

### What does "Original Credit Memo does not exist or already Cancelled" mean?

**Reason:** You attempted to cancel a credit memo with reference details that don’t match an existing, active credit memo.
**Solution:** Re-upload the cancellation file with the **correct reference** details.

### How do I fix "Original Invoice does not exist or already Cancelled" or "Original Invoice does not exist"?

**Reason:** A credit memo references an invoice that doesn’t exist or is already cancelled.
**Solution:** Correct the **reference invoice** details and re-process.

### Why am I seeing "Invalid INV. SO not present in System"?

**Reason:** An invoice references a Sales Order (SO) that isn’t in the system.
**Solution:** Re-process with a **valid, existing SO** number.

### What should I do for an "Error Loading SO Line"?

**Reason:** The associated SO line hasn’t been successfully processed from the contract stage.
**Solution:** Process the SO in the **contract stage** successfully before loading the invoice.

### How do I resolve "CM cannot be processed as INV is in error"?

**Reason:** A Credit Memo (CM) was submitted against an invoice that’s currently in an **error** state in Stage.
**Solution:** Resolve the invoice error first, then process the CM.

### What causes the "Cumulative bill amount is over sell price" error?

**Reason:** Total invoice value for a subscription exceeds the sell price, and **over-billing** isn’t allowed.
**Solution:** Go to **Profiles → Overage** and enable the overage setting.

***

## Cost stage errors

These errors occur during the processing of cost-related data.

### What does "Invalid Cost, SO not present in System" mean?

**Reason:** The SO number in the cost file is incorrect or doesn’t exist.
**Solution:** Verify the SO number and re-upload.

### Why am I seeing "Bundle child updates are not allowed" in the Cost Stage?

**Reason:** Direct updates to bundle **child** lines are not allowed for costs either.
**Solution:** Update costs on the **parent bundle** line.

### How do I fix "Invalid Cost Type, Cost Type Setup is missing"?

**Reason:** The specified **Cost Type** hasn’t been configured.
**Solution:** Configure the Cost Type correctly, then re-process.

### What does "Allocated Commission lines cannot be updated" mean?

**Reason:** Once commission is allocated to a line, that line cannot be updated.
**Solution:** Avoid updating lines with allocated commission; use a new transaction or reversal if needed.
