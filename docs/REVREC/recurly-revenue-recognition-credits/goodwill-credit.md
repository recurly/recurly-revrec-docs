---
title: Goodwill credit
excerpt: >-
  Boost purchases by recognizing goodwill credits with Recurly Revenue
  Recognition. This feature allows businesses to bring credit information
  directly into revenue recognition.
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

Goodwill credit is a complimentary credit balance given to customers as a gesture of goodwill. This credit can be applied toward purchases, facilitating payment adjustments and enhancing customer loyalty. Importantly, this system allows for seamless integration into the customer's Enterprise Resource Planning (ERP) system or revenue recognition ecosystem, streamlining reporting and financial tracking.

# Key benefits

* **Streamlined revenue recognition**: Incorporating goodwill credits into revenue reports enhances financial accuracy by reflecting real-time customer balances and potential sales.
* **Enhanced financial reporting**: Goodwill credits contribute to a more comprehensive view of financial health, allowing for precise revenue tracking and forecasting in revenue recognition reports.
* **Increased operational efficiency**: The management of goodwill credits through automated systems simplifies the reconciliation process, ensuring that credits are accurately reported in financial statements, improving overall financial transparency and compliance.

# Key details

To support business growth and enhance customer satisfaction, companies can issue goodwill credits. These credits serve as a balance in the customer's account, applicable towards purchases.

When goodwill credit is allocated, Recurly generates a credit invoice, reflecting the credit balance which can be adjusted against subsequent payments. This process not only simplifies account management but also ensures transparency in financial transactions.

<Image align="center" border={true} width="80% " src="https://files.readme.io/82c8766-Screenshot_1_2024-03-04_at_4.45.08_PM.png" className="border" />

The issuing and redemption of goodwill credits are accurately documented, facilitating seamless financial reporting. Credits are recorded as a single line in revenue recognition reports, with redemptions detailed separately. This clear delineation helps businesses track credit usage and its impact on financial health.

The following table outlines the identifiers for goodwill credit transactions:

| Origin       | Activity          | Plan Code                |
| ------------ | ----------------- | ------------------------ |
| credit-event | Goodwill issued   | credit-goodwill          |
| credit-event | Goodwill redeemed | credit-goodwill-redeemed |
| credit-event | Goodwill voided   | credit-goodwill-voided   |

<Image align="center" border={true} src="https://files.readme.io/19cd870-image.png" className="border" />

In instances where goodwill credit is issued erroneously or remains unused, it can be voided, removing the balance from the customer's account. This action, along with all other credit transactions, is recorded in Revenue Recogntion, ensuring comprehensive financial oversight.

<Image align="center" border={true} src="https://files.readme.io/efb1208-image.png" className="border" />

# FAQ

**Q: How are Goodwill Credits and their usage tracked in RevRec?**
A: Goodwill credits appear as distinct lines that you can identify by **plan code**:

* **Credit issued:** `credit-goodwill`
* **Credit used/redeemed:** `credit-goodwill-redeemed`
* **Credit canceled/voided:** `credit-goodwill-voided`
  Tip: Credit-related lines also show **origin = credit-event**.

**Q: What happens if a Goodwill Credit is given by mistake or is never used?**
A: Void the credit. A voided credit is no longer available to the customer, and RevRec records a reversal line with plan code **`credit-goodwill-voided`**.
