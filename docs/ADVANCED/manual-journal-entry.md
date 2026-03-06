---
title: Manual journal entry
deprecated: false
hidden: true
metadata:
  robots: index
---
This guide provides a comprehensive walkthrough of the process for uploading a manual journal entry (JE) into the system. The process involves uploading a prepared file, specifying the posting details, and completing the review and approval workflow.  

Before you begin, please ensure your Manual JE file is ready. This file must be properly formatted and contain all the mandatory columns listed below. The file can have any additional columns based on the requirement.

* Subscription Number
* Subscription Line
* Account Type (Select one of the account type from the below list)
* Asset
* Liability
* Revenue
* COGS
* Deferred COGS
* Start Date (Can be blank)
* End Date (Can be blank)
* Dr Amount
* Cr Amount
* Account (Enter the account number along with segments)
* Auto Reversal (Can be yes or no, depending on the scenario)
* Currency
* Company Currency
* Ex-Rate
* Company Ex-rate

<br />

Step 1: Navigate and Initiate the Upload
Follow these steps to begin the upload process:
Navigate to Journals: From the main system menu, go to Import / Export > Journals. This will take you to the journal upload screen.

Add a New Journal Entry: Click on the + icon located on the screen. This action opens the interface for uploading a new manual JE.

Upload the File: Select and upload your prepared manual JE file from your computer.
Select Posting Details: After the file is attached, you must specify where and when the entry should be posted:
Books: From the dropdown menu, select the specific accounting books where this journal entry needs to be loaded.
Period: Choose the appropriate accounting period (e.g., Sep-25) for the journal entry. This is crucial for accurate financial reporting.
Save the Upload: Once you have selected the correct books and period, click the Save button.
Step 2: Review and Approval Workflow
After saving, the journal entry does not post immediately. It must go through a mandatory approval step.
Check the Status: After you click Save, the file's status will change to "Approval Pending". You will notice an arrow icon () appear next to the entry, indicating that a further action is required.

Go to the Revenue Workbench: Click on the arrow icon. This is a shortcut that will navigate you directly to the Revenue Workbench.
Review the Manual JE: In the Revenue Workbench, you can view the uploaded manual JE in a structured format. Carefully review all details:
Verify the accounts being debited and credited.
Confirm the amounts are correct.
Check descriptions and other relevant data for accuracy.
Approve or Reject the Entry: Based on your review, you have two options:
Approve: If the journal entry is accurate and ready to be posted, enter the comments and click the Approve button. Once approved, the entries will be permanently posted.

Reject: If you find any discrepancies or if the entry should not be posted, enter comments and click the Reject button. This will cancel the transaction and prevent it from affecting the books.

Once an entry is approved, the process is complete, and the transaction will be reflected in your reports for the selected period.
Here are explanations for the common manual journal entries and their impact on financial reports.
Example 1: Recognizing Revenue from Liability
This entry debits liability and credit revenue. Below is the screenshot of one such entry.
Journal Entry:
Debit Liability (Deferred Revenue): Decreases the deferred revenue account, showing you've fulfilled your obligation.
Credit Revenue: Increases the revenue account, reflecting the income you've earned.

Impact on Reports:
The increase in revenue will be displayed in the Revenue Waterfall Report.
The decrease in the liability balance will be shown in the Liability Balances Report.
Example 2: Recognizing Cost (COGS)
This entry is used to record the costs associated with the revenue. It is credited to the Deferred COGS account.
Journal Entry:
Debit COGS: the cost will be expensed
Credit Deferred COGS: Decreases the deferred cost account.

Impact on Reports:
The recognized cost will appear in the Cost Waterfall Report.
The updated deferred cost balance will be visible in the Cost Balances Report.
Example 3: Accruing Revenue with an Asset

This entry is created while recognizing revenue from the asset account. We debit assets and credit revenue.

Journal Entry:
Debit Asset (e.g., Accounts Receivable): Increases your assets, showing that a customer owes you money.
Credit Revenue: recognizes revenue for the period.
Impact on Reports:
The recognized revenue from this entry will be visible in the Revenue Waterfall Report. The asset part of the entry can be seen under the Asset Balances Report.
Important Considerations for Manual Journal Entries (MJE)
When preparing and uploading a Manual Journal Entry, it is crucial to understand that this process operates completely independently of the system's automated rules. Please review the following points carefully before posting:
Entries are Fully Manual: As the name implies, a manual JE requires every piece of information to be provided by you in the upload file. The system will not automatically apply or derive any details from existing system configurations, such as data rules or revenue recognition settings. The data will be posted exactly as you provide it.
All Segments Must Be Manually Input: The system will not automatically populate any financial dimensions or reporting segments (e.g., Department, Product Line, Region, Cost Centre).
If the start and end dates are blank in the file, the system will recognize the entire revenue in the period uploaded. If the start and end dates are filled in, you will be able to see the waterfall based on the start and end dates.
If the auto reversal is yes, the current period entry will be reversed in the next period.
In short, the MJE feature provides you with precise control, but it also means the responsibility for the accuracy and completeness of the data. Always double-check your file before uploading.
