---
title: Manual journal entry
excerpt: Upload, review, and approve manual journal entries in Recurly RevRec.
deprecated: false
hidden: false
metadata:
  robots: index
---
# Overview

Use manual journal entries to upload accounting adjustments directly into Recurly Revenue Recognition (RevRec). This process gives you full control over the journal data, posting period, and approval workflow, which is useful when an entry must be recorded outside the system’s automated revenue recognition logic.

### Prerequisites

Before you upload a manual journal entry file, make sure:

* Your file is complete and properly formatted.
* All mandatory columns are included.
* Posting details such as **Books** and **Period** are known in advance.
* The data has been reviewed for accuracy, including accounts, amounts, currency, and segment values.

### Limitations

* Manual journal entries operate independently from automated RevRec rules.
* RevRec does not derive or populate values from data rules, revenue schedules, or existing system logic.
* You must manually provide all required financial dimensions and segments in the upload file.
* If **Start Date** and **End Date** are blank, the full amount is recognized in the uploaded period.
* If **Auto Reversal** is set to **Yes**, the current-period entry is reversed in the next period.

## Definition

A manual journal entry is a journal entry that you upload into RevRec using a prepared file. After upload, the entry moves through a review and approval workflow before it is posted to the selected books and period.

## Key benefits

* Record accounting adjustments with precise control.
* Post entries to specific books and accounting periods.
* Support approval before posting.
* Reflect manual adjustments in RevRec reporting, including waterfall and balance reports.

## Prepare the upload file

Your manual journal entry file must include the mandatory columns listed below. You can also include additional columns if needed for your process.

| Column              | Requirement | Notes                                                                              |
| :------------------ | :---------- | :--------------------------------------------------------------------------------- |
| Subscription Number | Required    | Enter the subscription identifier.                                                 |
| Subscription Line   | Required    | Enter the subscription line.                                                       |
| Account Type        | Required    | Use one supported value such as Asset, Liability, Revenue, COGS, or Deferred COGS. |
| Asset               | Conditional | Use when the entry affects an asset account.                                       |
| Liability           | Conditional | Use when the entry affects a liability account.                                    |
| Revenue             | Conditional | Use when the entry affects a revenue account.                                      |
| COGS                | Conditional | Use when the entry affects a cost of goods sold account.                           |
| Deferred COGS       | Conditional | Use when the entry affects deferred cost.                                          |
| Start Date          | Optional    | Can be blank.                                                                      |
| End Date            | Optional    | Can be blank.                                                                      |
| Dr Amount           | Required    | Enter the debit amount.                                                            |
| Cr Amount           | Required    | Enter the credit amount.                                                           |
| Account             | Required    | Enter the account number, including segments.                                      |
| Auto Reversal       | Required    | Enter **Yes** or **No**, depending on the scenario.                                |
| Currency            | Required    | Enter the transaction currency.                                                    |
| Company Currency    | Required    | Enter the company currency.                                                        |
| Ex-Rate             | Required    | Enter the transaction exchange rate.                                               |
| Company Ex-rate     | Required    | Enter the company exchange rate.                                                   |

## Upload a manual journal entry

1. **Go to** **Import / Export > Journals**.

<Image align="center" border={true} src="https://files.readme.io/21fca57289c04939c098a4534744c11c748f7517e55289d45d9351376c7168fb-Image_1.png" className="border" />

2. **Select** the **+** icon to create a new manual journal entry.

<Image align="center" border={true} src="https://files.readme.io/af44223b98a4b5ce3dd67c07407a4d4a4ca48068413ba89f065c5ee41494cf8d-Image_2.png" className="border" />

3. **Upload** your prepared manual journal entry file.
4. **Select** the posting details:
   * **Books:** Choose the accounting books where the journal entry should be loaded.
   * **Period:** Choose the accounting period for the entry, such as **Sep-25**.
5. **Select** **Save**.

After you save the file, the entry does not post immediately. RevRec changes the status to **Approval Pending** and displays an arrow icon next to the entry.

## Review and approve the journal entry

1. **Select** the **arrow icon** next to the uploaded file.

<Image align="center" border={true} src="https://files.readme.io/df3988a3d5aaf619bead3b756a0945843d6baa4262a7898a3bc703b2f6ad40b7-image.png" className="border" />

2. **Open** the entry in the **Revenue Workbench**.
3. **Review** the uploaded journal entry carefully, including:
   * Debited and credited accounts
   * Amounts
   * Descriptions
   * Any additional relevant values
4. **Enter** review comments.
5. Choose one of the following actions:

**Approve** to post the journal entry permanently.

![](https://files.readme.io/dc468975e9f16752b4ef13e72b7bc7ac315c6104415c558297a6bcf07d2b5dd5-image.png)

**Reject** to cancel the transaction and prevent it from affecting the books.

<Image align="center" border={true} src="https://files.readme.io/8d357b7e8f1331c5d31e277e7d5b7e6454e005b84bad26100ab7b02e8f61dab3-Image_5.png" className="border" />

Once approved, the process is complete and the transaction is reflected in reports for the selected period.

## How dates affect recognition

The values in **Start Date** and **End Date** determine how RevRec reflects the entry:

| Scenario                              | Result                                                                  |
| :------------------------------------ | :---------------------------------------------------------------------- |
| Start Date and End Date are blank     | RevRec recognizes the full amount in the uploaded period.               |
| Start Date and End Date are populated | RevRec reflects the entry in the waterfall based on the provided dates. |

## How auto reversal works

If **Auto Reversal** is set to **Yes**, RevRec reverses the current-period entry in the next accounting period.

## Reporting examples

The following examples describe common manual journal entry scenarios and where their impact appears in RevRec reports.

### Recognize revenue from liability

Use this entry when revenue is recognized from a liability balance such as deferred revenue.

| Journal impact                     | Result                                                                         |
| :--------------------------------- | :----------------------------------------------------------------------------- |
| Debit Liability (Deferred Revenue) | Decreases deferred revenue, reflecting that the obligation has been fulfilled. |
| Credit Revenue                     | Increases recognized revenue for the period.                                   |

<Image align="center" border={true} src="https://files.readme.io/1cadfe15362ce063db69ed8e362893266942beb98287899901984a5b876c4970-Image_6.png" className="border" />

**Report impact**

* Revenue appears in the **Revenue Waterfall Report**.
* The reduced liability balance appears in the **Liability Balances Report**.

### Recognize cost (COGS)

Use this entry to recognize cost associated with revenue.

| Journal impact       | Result                               |
| :------------------- | :----------------------------------- |
| Debit COGS           | Recognizes cost as expense.          |
| Credit Deferred COGS | Decreases the deferred cost balance. |

<Image align="center" border={true} src="https://files.readme.io/20df8138df17b216afa49ad0780111c1d0b562ce1d8097d413a3e1553eda8c4b-Image_7.png" className="border" />

**Report impact**

* Recognized cost appears in the **Cost Waterfall Report**.
* The updated deferred cost balance appears in the **Cost Balances Report**.

### Recognize revenue with an asset

Use this entry when revenue is recognized against an asset account, such as accounts receivable.

| Journal impact | Result                                                      |
| :------------- | :---------------------------------------------------------- |
| Debit Asset    | Increases assets, reflecting an amount owed to the company. |
| Credit Revenue | Recognizes revenue for the period.                          |

<Image align="center" border={true} src="https://files.readme.io/8dfe10dde3f805909f3b779062daf19c454c25af0e978e2e86bfbafd7e3f869b-Image_8.png" className="border" />

**Report impact**

* Revenue appears in the **Revenue Waterfall Report**.
* The asset balance appears in the **Asset Balances Report**.

## Important considerations

Manual journal entries give you precise control, but they also place full responsibility for the entry on the uploader. Keep these points in mind:

| Consideration           | Details                                                                                                                             |
| :---------------------- | :---------------------------------------------------------------------------------------------------------------------------------- |
| Fully manual process    | RevRec posts the data exactly as provided in the file.                                                                              |
| No automated derivation | The system does not apply revenue rules, data rules, or other configuration logic.                                                  |
| Segment responsibility  | You must manually enter all applicable segments and reporting dimensions, such as department, product line, region, or cost center. |
| Accuracy matters        | Always verify accounts, amounts, dates, currencies, and comments before upload and approval.                                        |

## FAQs

**Q: Does RevRec derive values for a manual journal entry from system rules?**  
**A**: No. Manual journal entries are independent from RevRec’s automated rules and configurations. You must provide all required values in the upload file.

**Q: What happens if I leave the start and end dates blank?**  
**A**: RevRec recognizes the full amount in the period selected during upload.

**Q: What happens if I populate the start and end dates?**  
**A**: RevRec reflects the entry in the waterfall based on the dates you provide.

**Q: Can I reverse a manual journal entry automatically?**  
**A**: Yes. Set **Auto Reversal** to **Yes** in the upload file to reverse the current-period entry in the next period.

**Q: Does the journal entry post immediately after upload?**  
**A**: No. After upload, the file status changes to **Approval Pending**. The entry must be reviewed and approved in the **Revenue Workbench** before it is posted.
