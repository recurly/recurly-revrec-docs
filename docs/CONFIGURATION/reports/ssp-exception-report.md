---
title: SSP exception report
excerpt: ' Explore the detailed guide on SSP Exception Report in Recurly''s Revenue Recognition user guide.'
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

### Required Plan

This feature or setting is available to all customers on any Recurly subscription plan.

# Definition

SSP Exception Report provides visibility into transactions that are not eligible for SSP (Stand-Alone Selling Price) allocation. This report displays transactions where the Allocation Flag is set to "No," indicating that the transaction does not meet the criteria for SSP allocation. It helps in identifying and addressing instances where SSP cannot be determined for certain transactions, enabling further analysis and appropriate actions.

# Guide

## Accessing and configuring the report

To access and configure the SSP Exception Report:

1. **Navigate to the Report:**
   * Go to **Reports > Exception Reports > SSP Exception Report**.
2. **Run the Report:**
   * Click the **Run** button to generate the report.
3. **Download the Report:**
   * Click the **Download** button to save the report locally.

## Report columns

* **Contract ID:** Displays the unique identifier for the contract.
* **Order Number:** Lists the order number associated with the transaction.
* **Order Line:** Provides details on the specific order line.
* **Book Date:** Indicates the date when the transaction was recorded.
* **Item:** Details the item or service involved in the transaction.
* **Sell Price:** Shows the selling price of the item.
* **List Price:** Displays the list price of the item.

# FAQ

**Q: How do I generate a report to identify contracts with SSP exceptions or other data quality issues?**
A: Use the **Exception report** (commonly used for **SSP Exceptions**) to flag pricing outside SSP bands, missing SSP assignments, and related configuration gaps. Go to **Analytics → Reports → Exception report**, choose your **Book** and **period**, and run the report. From there, drill into affected contracts/lines and remediate in **Rules → SSP (Analyzer)** or via **Workbench** as needed. For step-by-step instructions and field definitions, see the **Exception report** documentation.

<br />
