---
title: Mid-tier offering of Revenue Recognition - Standalone
excerpt: >-
  Learn what’s included in RevRec’s mid-tier offering, plus optional modules you
  can enable as you scale.
deprecated: false
hidden: true
metadata:
  robots: index
---
# Overview

Recurly Revenue Recognition (RevRec) mid-tier offering is built for organizations that need sophisticated revenue recognition without the high onboarding costs or long implementation timelines of a full-scale advanced solution. It bridges the gap between standard and advanced systems, giving you a cost-effective, quick-to-deploy platform for complex revenue scenarios and audit-ready compliance with Accounting Standards Codification (ASC) 606 and International Financial Reporting Standard (IFRS) 15.

The mid-tier offering is a configurable RevRec package that includes core functionality by default, plus optional modules a Revenue Super Admin can activate as your needs grow. When optional features are off, RevRec hides related fields, tabs, reports, and menu items to keep your workspace focused.

# Key benefits

* **Lower total cost for complex revenue**: Get audit-ready tooling for multi-element and advanced scenarios without an enterprise-style onboarding effort
* **Faster time-to-value**: Implement and start recognising revenue sooner with a quick-to-deploy setup
* **Scalable feature set**: Turn on optional modules as your requirements evolve, without rebuilding your processes
* **Cleaner workspace**: Only see the tabs, fields, and reports that match what your organisation has enabled

# Key details

## Key objectives

* Provide a cost-effective solution for complex revenue recognition
* Enable faster implementation and time-to-value
* Deliver key capabilities like contract grouping, performance obligations (POBs), and business event management
* Offer modular features you can activate as your business needs grow

## Feature enablement behaviour

RevRec uses feature enablement to control what appears in the application.

* When a feature isn’t enabled, its related fields, Workbench tabs, reports, and menu items are hidden
* When a Revenue Super Admin enables a feature, related interface elements and functions automatically appear for users who have permission

## Roles and permissions

Access is managed through three roles.

| Role                | Who it’s for                                        | What they can do                                                                     |
| ------------------- | --------------------------------------------------- | ------------------------------------------------------------------------------------ |
| Revenue Super Admin | System administrators (Recurly internal users only) | Access the RevRec admin menu, and enable optional features in **Feature management** |
| Revenue Manager     | Day-to-day revenue operations                       | Use all core features, plus any optional features enabled by the Revenue Super Admin |
| Read-only user      | Stakeholders who need visibility                    | View-only access to all enabled features                                             |

## Core offering (system default)

All organisations receive the core offering during setup.

### Core functions

| Function                       | What it’s for                                                                                                                |
| ------------------------------ | ---------------------------------------------------------------------------------------------------------------------------- |
| Contract grouping              | Define and manage multi-element arrangements so reporting and compliance stays accurate                                      |
| Performance obligations (POBs) | Create and manage POBs and related rules (expense and dependency areas appear only when those optional features are enabled) |
| Data sets and Data Rules       | Classify, filter, and structure revenue data inputs                                                                          |
| Additional entry rules         | Create custom posting rules to match your business requirements                                                              |

### Core Workbench tabs

The Workbench is your primary workspace. By default, it includes:

* Search
* POB (Performance Obligation)
* Billing
* Waterfall
* Journals
* Business Events
* Contract Balance
* Audit

### Core Workbench actions

You can perform these actions in the Workbench by default:

* Link
* Move POB
* Recognise
* Event

### Core reporting

RevRec includes a full suite of reports by default.

| Report area         | What you’ll get                                         |
| ------------------- | ------------------------------------------------------- |
| Revenue reports     | Insight, Revenue Waterfall, and Defer Revenue Waterfall |
| Transaction details | Contract and Billing reports                            |
| Stage details       | Contract, Doc, and Event reports                        |
| Report balances     | All balance reports                                     |
| Audit reports       | Audit-focused reporting for traceability and review     |

## Optional features (Revenue Super Admin activation)

A Revenue Super Admin can enable optional modules in **Super Admin → Feature management**. When enabled, RevRec automatically updates the interface for permissioned users.

### Allocation

**Purpose:** Support complex allocation requirements, such as Standalone Selling Price (SSP).

**What it enables:**

* **Rules:** Configure SSP rules
* **Workbench tabs:** Adds **Modifications** and **Allocation Details**, plus allocation-related columns in **Contract Balance**
* **Workbench actions:** Adds **Allocation** and **ReAllocation**
* **Setup:** Activates allocation-related attributes in Attribute labels, turns on the **Contract Modifications** page, and adds profiles under the RevRec admin **Profiles** section
* **Reports:** Enables SSP exception reports, plus allocation-related attributes across other reports

### Variable consideration

**Purpose:** Manage and account for variable consideration components.

**What it enables:**

* **Rules:** Configure Variable Consideration rules
* **Workbench tab:** Adds the **VC** tab and related functionality, plus VC-related columns in **Contract Balance**
* **Fields:** Adds VC-related fields and labels across the application, and enables VC-related attributes in other reports
* **Reports:** Enables VC/Cost reports

### Expense accounting

**Purpose:** Recognise and manage costs associated with revenue.

**What it enables:**

* **Rules:** Configure cost rules
* **POB:** Activates the **Expense** section within Performance Obligations
* **Workbench tab:** Adds the **Cost** tab
* **Stage area:** Enables a Cost stage area
* **Fields:** Adds cost-related fields and labels across the application
* **Reports:** Enables Cost/VC reports, plus cost-related attributes across other reports

### Additional features

**Purpose:** A set of advanced capabilities for specialised processes.

**What it enables:**

* **Holds:** Place and manage holds, including Holds exception reporting

  * Adds hold functionality under rules, a **Holds** tab in the Workbench, hold-related Workbench actions, and hold-related columns in **Contract Balance**
  * Enables the **HOLD** event type under Business Events
* **Bundle:** Enable **Product Bundle** transformation rules

  * Adds bundle allocation profiles under the **Profiles** section
* **POB:** Activates the forecast section within Performance Obligations and adds forecast-related Workbench actions
* **Fields and reports:** Adds Holds and Bundle-related fields, labels, and reporting attributes

### App management

**Purpose:** Manage application-level integrations and data flows.

**What it enables:**

* **Jobs:** Adds **App Management** under the Jobs section

**Important:** After this feature is enabled, it can’t be disabled.

# FAQs

**Q: Who can enable optional modules?**

**A:** Only the Revenue Super Admin can activate optional features in **Super Admin → Feature management**. Once enabled, the related tabs, fields, reports, and menu items appear automatically for permissioned users.

**Q: Why don’t I see a tab or report mentioned here?**

**A:** It’s usually one of these reasons:

* The feature that controls it hasn’t been enabled
* Your role doesn’t have permission to access it

**Q: Can I turn features on as we grow?**

**A:** Yes. Optional modules are designed to be activated over time, so your RevRec setup can evolve with your revenue complexity.