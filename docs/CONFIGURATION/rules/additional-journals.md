---
title: Additional journals
excerpt: >-
  Configure Additional Journals in Recurly RevRec to generate journal entries
  for special-purpose requirements based on billing, revenue waterfall, or
  adjustment waterfall amounts.
deprecated: false
hidden: false
metadata:
  robots: index
---
<div class="rp-page">
  <div class="rp-overview">Additional Journals lets you generate journal entries for special-purpose requirements based on billed amounts, revenue waterfall values, or adjustment waterfall values. Navigate to Rules → Additional Journals to set up and manage your configurations.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Available as part of Recurly RevRec</div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#configuring-additional-journals"><span class="rp-toc-num">1</span>Configuring additional journals</a>
  </div>
</div>

# Configuring additional journals

Select the JE type that matches your requirement, then follow the steps for that type.

<Tabs>
  <Tab title="Billing">

1. **Name:** Enter a unique name for the additional journal.
2. **Books:** Choose the books in which the journal is to be posted — for example, Primary, Secondary, or All.
3. **JE Type:** Select Document. Use this type to create an additional journal based on the billed amount. You can also create journals based on any calculated columns in the document or billing record.
4. **POB Type:** Select the POB type the additional journals should apply to. Journals are only generated when a subscription belongs to the selected POB type. If additional journals are required for Cost or Expenses, select the cost type as well.
5. **Amount:** Select the data type for the amount in the journal entry. The dropdown displays all document attributes of data type "amount" defined in your instance. This field is only available when the JE type is Document.
6. **Debit and credit accounts:** Enter the debit and credit account information for the additional journals.
7. **Active date:** Set the start and end dates the JE should be active. Leave the end date blank to apply the JE indefinitely.
8. **Auto Reverse (optional):** Enable this option to automatically reverse the JE in the next period of the contract. Available only when the JE type is Document.
9. **Retirement (optional):** Available when additional journals are configured for a cost type. Enabling this creates additional journals at the end of the contract period.

<div class="rp-callout rp-callout-note">
  <div><strong><i class="fa-solid fa-circle-info" aria-hidden="true"></i> Note</strong>POB type and cost type are mutually exclusive — you can't select both at the same time.</div>
</div>

  </Tab>
  <Tab title="Revenue waterfall">

1. **Name:** Enter a unique name for the additional journal.
2. **Books:** Choose the books in which the journal is to be posted — for example, Primary, Secondary, or All.
3. **JE Type:** Select Revenue Waterfall. The JE is posted to the contract for the amounts in the revenue waterfall. To apply the additional journal to all contracts, leave the POB type blank.
4. **Debit and credit accounts:** Enter the debit and credit account information for the additional journals.
5. **Active date:** Set the start and end dates the JE should be active. Leave the end date blank to apply the JE indefinitely.

  </Tab>
  <Tab title="Adjustment waterfall">

1. **Name:** Enter a unique name for the additional journal.
2. **Books:** Choose the books in which the journal is to be posted — for example, Primary, Secondary, or All.
3. **JE Type:** Select Adjustment Waterfall. Entries are posted in the adjustment waterfall — the waterfall that arises from carve-ins and carve-outs at the time of allocation. This type is only applicable when the merchant has allocations.
4. **Debit and credit accounts:** Enter the debit and credit account values for the configured journals.
5. **Active date:** Set the start and end dates the JE should be active. Leave the end date blank to apply the JE indefinitely.

<div class="rp-callout rp-callout-note">
  <div><strong><i class="fa-solid fa-circle-info" aria-hidden="true"></i> Note</strong>Adjustment waterfall additional journals don't include a POB type selection and don't support auto reverse.</div>
</div>

  </Tab>
</Tabs>

<br />
