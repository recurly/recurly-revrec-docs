---
title: Prepayment credit
excerpt: >-
  Prepayment credit in Recurly allows customers to pay in advance for purchases,
  streamlining the subscription process and enhancing financial flexibility.
  This feature allows businesses to pull balance credits information, enhancing
  their revenue recognition experience.
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

To access this feature or setting, you must have an active subscription to either the Recurly RevRec or the Standard edition. For further information on pricing and how to enable this feature on your account, please contact your Recurly account manager directly, or reach out to us at [support@recurly.com](mailto:support@recurly.com).

### Prerequisites

* Cancellation and refund policy that supports prepayment crediting.

### Limitations

* Prepayment credits can only be used for purchases and cannot be refunded.
* Specific configurations may restrict the use of prepayment credits for certain plans or products.

# Definition

Prepayment credit refers to an advance payment made by a customer for purchases or subscriptions with a business. This credit is stored in the customer's account and automatically applied to invoices as they are generated, simplifying the payment process.

# Key benefits

* **Streamlined revenue recognition**: Incorporating prepayment credits into revenue reports enhances financial accuracy by reflecting real-time customer balances and potential sales.
* **Enhanced financial reporting**: Prepayment credits contribute to a more comprehensive view of financial health, allowing for precise revenue tracking and forecasting in revenue recognition reports.
* **Increased operational efficiency**: The management of prepayment credits through automated systems simplifies the reconciliation process, ensuring that credits are accurately reported in financial statements, improving overall financial transparency and compliance.

# Key details

Customers are encouraged to make advance payments, known as prepayment credits, which are then applied to purchases. This process involves the issuance of two invoices in Recurly: one acknowledging the payment and the other representing the credit.

**Payment invoice**

<Image align="center" border={true} width="80% " src="https://files.readme.io/41591a7-image.png" className="border" />

**Credit Invoice**

<Image align="center" border={true} width="80% " src="https://files.readme.io/9ed19d1-image.png" className="border" />

Prepayment credits are integrated into the Revenue Recognition (RevRec) system as a single Sales Order (SO) line, accompanied by two invoices. Adjustments to the credit are recorded as new lines, identifiable by their origin and plan code.

| Origin       | Activity                   | Plan Code                  |
| ------------ | -------------------------- | -------------------------- |
| credit-event | prepayment credit issued   | credit-prepayment          |
| credit-event | prepayment credit redeemed | credit-prepayment redeemed |
| credit-event | Prepayment credit voided   | credit-prepayment-voided   |

<Image align="center" border={true} src="https://files.readme.io/00ce3ca-image.png" className="border" />

Customers can view their total credit balance in Recurly, which is equal to the total sell price of the credit lines. This balance is visible in the customer information section.

<Image align="center" border={true} width="45% " src="https://files.readme.io/0a9446b-image.png" className="border" />

Through prepayment credits, Recurly provides a flexible and efficient way for businesses and customers to recognize and manage advance payments, offering benefits such as improved cash flow, convenience, and simplified billing processes.

# FAQ

**Q: What makes a Prepayment credit different from the other two credit types?**
A: A **prepayment credit** is **funded by the customer**. They pay in advance, and that amount is held as a credit balance to use on future subscriptions or purchases.

**Q: Why do I see two credit-event invoices in Recurly when a prepayment credit is issued?**
A: Two invoices are created to make the accounting clear:

* **Payment invoice:** Acknowledges receipt of the customer’s advance payment.
* **Credit invoice:** Converts that payment into a usable **credit balance** on the customer’s account.

**Q: How are prepayment credits and their adjustments tracked in RevRec?**
A: Filter for **origin = credit-event** and use these **plan codes**:

* **Credit issued:** `credit-prepayment`
* **Credit used/redeemed:** `credit-prepayment-redeemed`
* **Credit canceled/voided:** `credit-prepayment-voided`
