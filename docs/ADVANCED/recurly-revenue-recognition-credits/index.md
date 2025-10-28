---
title: Credits
excerpt: >-
  Maximize customer satisfaction and financial flexibility with Recurly Revenue
  Recognition credits, including goodwill, on-account, and prepayment credits.
  Keep track of credits as they impact your revenue recognition.
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---
# Overview

### Additional cost

To access these features or settings, you must have an active subscription to either the Recurly Revenue Recognition Advanced or the Standard edition. For further information on pricing and how to enable this feature on your account, please contact your Recurly account manager directly, or reach out to us at [support@recurly.com](mailto:support@recurly.com).

export const PrerequisitesLimitations = ({ header }) => {
  return (
    <div className="flex justify-start">
      <div className="rounded-md p-6 m-4 max-w-lg shadow-md border border-gray-300 dark:bg-gray-800 dark:border-gray-600">
        <p className="text-lg font-bold">{header}</p>

        {/* Prerequisite */}
        <p>
          <i className="fa-solid fa-check mr-2" />
          Cancellation and refund policy that supports account crediting.
        </p>

        {/* Limitations */}
        <p>
          <i className="fa-solid fa-exclamation-triangle mr-4" />
          Prepayment credits can only be used for purchases and cannot be refunded.
        </p>
        <p>
          <i className="fa-solid fa-exclamation-triangle mr-4" />
          Goodwill credits are non-transferable and must be used within the issuing account.
        </p>
        <p>
          <i className="fa-solid fa-exclamation-triangle mr-4" />
          Credits may have expiration dates or usage conditions, depending on the business policy.
        </p>
      </div>
    </div>
  );
};

<PrerequisitesLimitations header="Prerequisites & limitations" />

# Definition

Recurly's Revenue Recognition Credits encompass three distinct types of credits that businesses can offer to their customers: Goodwill Credit, On-account Credit, and Prepayment Credit. Each serves a unique purpose, from enhancing revenue recognition to conducting new strategies based on your analysis.

## Incorporating credits in Recurly's Revenue Recognition

You have the flexibility to incorporate credits into your revenue recognition instance or not include them.

1. **Navigate** to Setup → Profiles
2. Under 'Ignore Credit Event Transactions' **select** 'Yes' or 'No'.

<Image align="center" border={true} width="50% " src="https://files.readme.io/5e90165b450dba809bb3614de2b2eba06b3b2d562d3ec5f1af57539d9f9909b4-Screenshot_2024-10-15_at_12.05.59_PM.png" className="border" />

## Key details

Visit our dedicated guides:

<Cards columns={3}>
  <Card title="Goodwill credit" href="goodwill-credit" icon="fa-handshake">
    Balance added to a customer’s account to acknowledge loyalty, resolve issues, or offer compensation. Integrated into revenue recognition reports.
  </Card>

  <Card title="On-account credit" href="on-account-credit" icon="fa-undo">
    Issued instead of refunds when subscriptions are canceled, helping retain customers and improve financial reporting accuracy.
  </Card>

  <Card title="Prepayment credit" href="prepayment-credit" icon="fa-credit-card">
    Customers pay in advance for services or products. Prepayments are tracked and reported in revenue recognition for better forecasting.
  </Card>
</Cards>

# FAQ 

**Q: What are the credit-event lines that appear in some contracts?**
A: When a credit transaction flows from Recurly into RevRec, a **credit-event** line is created to track that credit and to balance it once it’s fully used.

**Q: How are credit events shown in RevRec?**
A: Credits can arise in different ways, and RevRec treats them accordingly:

* **Goodwill credit:** A free, promotional credit (appears as a Credit Invoice in Recurly). It enters RevRec as one line; each redemption posts as a separate line. Identify via **origin = credit-event** and **plan code**.
* **On-account credit:** Typically issued instead of a cash refund (e.g., post-cancellation). It enters as one line; each redemption is a separate line. Identify via **origin = credit-event**.
* **Prepayment credit:** Customer-funded advance for future services. In RevRec it appears as **one SO line with two invoices**; any credit adjustment posts as a new line.

**Q: How can I see a customer’s total available credit balance?**
A: In Recurly, open the customer’s account page. The sum of the **Sell Price** for all **active credit lines** equals the customer’s total credit balance.

**Q: How can I identify credit-related transactions in RevRec?**
A: Filter by line-item **origin = credit-event**. The specific credit type or action (e.g., redemption, void) can be determined from the **plan code**.

<br />
