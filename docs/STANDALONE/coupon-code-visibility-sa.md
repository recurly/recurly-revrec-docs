---
title: Coupon code - Standalone
excerpt: >-
  Track coupon codes in RevRec at the subscription and charge line level for
  discount traceability.
deprecated: false
hidden: false
metadata:
  robots: index
---
# Overview

RevRec now pulls coupon code data directly from Recurly Billing and surfaces it in your RevRec views. Instead of cross-referencing billing records and revenue schedules manually, you can now see coupon codes at both the subscription and charge line level, including on credit events. This helps your finance team trace discounts for ASC 606 and IFRS 15 reporting.

## Where coupon codes appear

| Level                                    | What you’ll see                                                                | Format                                                    | Why it matters                                                                                                          |
| ---------------------------------------- | ------------------------------------------------------------------------------ | --------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| Subscription                             | A consolidated list of coupon codes associated with the subscription lifecycle | A single concatenated string of active coupon codes       | Helps you understand the discount context for the subscription when reviewing contracts and forecasting revenue impact. |
| Charge line                              | The specific coupon code(s) that discounted an individual invoice line item    | If multiple coupons apply, codes are separated by a comma | Makes it clear which discounts affected which charge lines, so allocations and reconciliations are easier to validate.  |
| Credit events (refunds/voids/write-offs) | Coupon codes from the original invoiced charge being credited                  | Mirrors the original charge line’s coupon code list       | Preserves traceability for negative revenue events by tying the credit back to the original commercial terms.           |

## Data fields and attributes

Use the following attributes in the Workbench and in exports to report on coupon codes:

| Attribute | Type               | Label                    | What it contains                                                                             |
| --------- | ------------------ | ------------------------ | -------------------------------------------------------------------------------------------- |
| **F23**   | Contract attribute | **Coupon Codes**         | A concatenated string of all active coupon codes associated with the subscription lifecycle. |
| **F9**    | Billing attribute  | **Invoice coupon codes** | The coupon code(s) applied to a specific invoice line item.                                  |

## Frequently asked questions

**Q: I see multiple codes in one field. How do I separate them?**
**A**: Coupon codes are stored as a concatenated string (for example, `CODE1, CODE2`). If you export to CSV or Excel, you can split the field using Excel’s **Text to Columns** feature and a comma delimiter.

**Q: Why do I see a coupon code on a refund line?**
**A**: That’s expected. For refunds, voids, and write-offs, RevRec looks back to the original invoiced charge line and displays the coupon code(s) that applied there. This keeps the credit event tied to the original discount conditions for audit and reconciliation.