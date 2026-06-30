---
title: RevRec FAQs
excerpt: >-
  Find answers to common questions about Recurly RevRec, covering core concepts,
  application setup, data transformation, reports, administration, credit
  events, period close, and stage errors.
deprecated: false
hidden: false
metadata:
  robots: index
---
<div class="rp-page">
  <div class="rp-overview">Find quick answers to the most common questions about Recurly RevRec — from core concepts like Contract Grouping and Performance Obligations to day-to-day tasks like running reports, closing periods, and resolving stage errors. Use the categories below to jump to the topic you need, or search the page for a specific term.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Available on all Recurly plans</div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#core-concepts"><span class="rp-toc-num">1</span>Core concepts</a>
    <a class="rp-toc-pill" href="#application-setup"><span class="rp-toc-num">2</span>Application setup</a>
    <a class="rp-toc-pill" href="#data-transformation"><span class="rp-toc-num">3</span>Data transformation</a>
    <a class="rp-toc-pill" href="#reports"><span class="rp-toc-num">4</span>Reports</a>
    <a class="rp-toc-pill" href="#administration"><span class="rp-toc-num">5</span>Administration</a>
    <a class="rp-toc-pill" href="#self-service-onboarding"><span class="rp-toc-num">6</span>Self-service onboarding</a>
    <a class="rp-toc-pill" href="#stage-area"><span class="rp-toc-num">7</span>Stage area</a>
    <a class="rp-toc-pill" href="#credit-events"><span class="rp-toc-num">8</span>Credit events</a>
    <a class="rp-toc-pill" href="#period-close-process"><span class="rp-toc-num">9</span>Period close process</a>
    <a class="rp-toc-pill" href="#stage-errors"><span class="rp-toc-num">10</span>Stage errors</a>
    <a class="rp-toc-pill" href="#other-questions"><span class="rp-toc-num">11</span>Other questions</a>
    <a class="rp-toc-pill" href="#standard-reports"><span class="rp-toc-num">12</span>Standard reports</a>
  </div>
</div>

# Core concepts

<Accordion title="How do I set up Contract Grouping rules in Recurly RevRec?">
  Contract Grouping rules are configured under the Rules section of the documentation. Here is a link to the Contract Grouping documentation for detailed setup instructions.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#contract-grouping:~:text=How%20to%20configure%20contract%20grouping" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Explain the purpose and configuration of a Performance Obligation within the RevRec module.">
  Performance Obligation configuration is found within the Rules section of the RevRec documentation. Review the Performance Obligation rules documentation to understand its purpose and setup.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#performance-obligation:~:text=be%20made%20active.-,Performance%20obligation,-In%20Recurly%20Revenue" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What are the steps to automate Variable Considerations (VC) in Recurly RevRec?">
  The steps for automating Variable Considerations are located within the Core Concepts > Rules section. Refer to the Variable Considerations documentation for the full process.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#performance-obligation:~:text=use%20the%20same.-,Variable%20considerations,-In%20Recurly%20Revenue" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Can you provide guidance on defining and using Standalone Selling Price (SSP) in the RevRec system?">
  Guidance on defining and using Standalone Selling Price (SSP) is available under the Rules section. Find the detailed SSP documentation here.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#performance-obligation:~:text=date%20%2B%2030%20days-,Standalone%20selling%20price,-Setting%20up%20the" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What is the Workbench and how is it used to manage revenue recognition contracts?">
  The Workbench is the central area for managing revenue contracts and viewing your contract groups. Its usage is detailed in the Revenue Recognition Workbench documentation.

<a href="https://docs.recurly.com/recurly-revrec/docs/revenue-recognition-workbench#:~:text=Powered%20by-,Revenue%20workbench,-Explore%20Recurly%27s%20Revenue" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Can I group contracts using multiple criteria?">
  Yes. Revrec allows you to configure contract grouping rules using any combination of factors, giving you full flexibility in how you organize your contracts.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#contract-grouping:~:text=Under%20the%20%22Grouping%22%20section%2C%20click%20on%20the%20%22%2B%22%20button%20to%20add%20grouping%20criteria." target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Can I schedule a grouping rule to apply only for a specific time period?">
  Yes. When configuring a grouping rule, you can set a Start Date and an optional End Date. This allows you to control exactly when a rule becomes active and when it expires.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#contract-grouping:~:text=Provide%20a%20name%20for%20the%20contract%20grouping%20and%20specify%20the%20active%20date." target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Can a single contract have multiple Performance Obligations (POBs)?">
  Yes. A single contract with multiple line items can have many POBs. You can define these relationships in the POB Rules page within Revrec.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#:~:text=be%20made%20active.-,Performance%20obligation,-In%20Recurly%20Revenue" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Is it possible to change a POB after a contract has been processed?">
  Yes, Revrec allows you to manually change a POB after it has been assigned.. For detailed instructions, please refer to the "Change POB" feature in the Revenue Workbench documentation.

<a href="https://docs.recurly.com/recurly-revrec/docs/revenue-recognition-workbench#:~:text=of%20the%20linkage.-,Moving%20the%20POB,-Click%20on%20the" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How do POB dependencies work?">
  This feature allows you to link the revenue recognition of one POB to another. For example, you can prevent revenue from being recognized on "POB B" until "POB A" is fulfilled. You can set this up in the "Dependency" section of the main POB page.
</Accordion>

<Accordion title="Can I amend the Standalone Selling Price (SSP) after it's been assigned?">
  Yes, you can update an SSP by using the Reallocation feature in the Revenue Workbench. If you perform a reallocation within the same month without other contract changes, the system will apply the newly modified SSP configuration.
</Accordion>

<Accordion title="Is an SSP update required when a contract is modified?">
  Yes. Any change to a contract in a new period is treated as a contract modification, RevRec will automatically trigger an SSP reallocation to ensure the revenue is allocated correctly based on the updated terms.
</Accordion>

<Accordion title="I updated our Performance Obligation (POB) rules, but I don't see the changes reflected in existing contracts. Why?">
  Performance Obligations (POBs) are assigned when a subscription is first processed and the revenue contract is created. The system does not automatically re-evaluate or change POBs on existing contracts when the rules are updated. Changes to POB rules are forward-looking and will only apply to new contracts created after the rule modification
</Accordion>

<Accordion title="My configuration is saved correctly in RevRec, but it's not being applied to new subscriptions. What should I check?">
  The most common reason for this is the configuration's active date range. For a rule to be applied, the transaction or subscription date must fall within the "Active From" and "Active To" dates defined in the configuration. Please verify that your configuration is active for the period in which your subscriptions are being processed.
</Accordion>

<Accordion title="Why do I need to configure POBs and their rules?">
  Configuring POBs and their associated rules is essential for ensuring accurate and consistent revenue recognition in compliance with accounting standards. It allows the system to correctly identify and allocate revenue to the specific obligations you have with your customers.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#:~:text=be%20made%20active.-,Performance%20obligation,-In%20Recurly%20Revenue" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Are there any default POBs I should avoid editing?">
  Yes. You should avoid editing the default POBs, specifically "Material right" and "manual journal," as they are integral to system functions.
</Accordion>

<Accordion title="How do I create a new POB?">
  Navigate to Rules → POB and click the "+" button to open the configuration screen for a new performance obligation.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#performance-obligation:~:text=consistent%20revenue%20recognition.-,Adding%20POBs,-Navigate%20to%20Rules" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What is a &quot;Waterfall Type&quot; (WF Type)?">
  The Waterfall Type determines the fundamental recognition timing for the POB. It defines whether revenue is recognized at a single moment (PointInTime) or spread across a period (OverTime, OverTime Slide, etc.).

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#performance-obligation:~:text=from%20the%20dropdown%3A-,PointInTime,-%3A%20Performance%20obligations" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What is the difference between the OverTime, OverTime Slide, and OverTime Condense waterfall types?">
  - **OverTime**: Revenue is recognized over the contract period.
- **OverTime Slide**: Revenue is recognized over the contract period, but the recognition is delayed by a specified release date.
- **OverTime Condense**: Revenue recognition is adjusted based on the timing of a specific event and a release date.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#performance-obligation:~:text=from%20the%20dropdown%3A-,PointInTime,-%3A%20Performance%20obligations" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What do the different &quot;Accounting Methods&quot; mean?">
  The accounting method determines how revenue is calculated and spread over a period. For example:

- **Daily**: Prorates revenue based on the number of days.
- **FixedMonthly**: Recognizes a fixed amount each full month.
- **PartialMonthly**: Prorates revenue for the first and last months and recognizes equal amounts for the months in between.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#performance-obligation:~:text=the%20dropdown%20options%3A-,Daily,-%3A%20Revenue%20recognized" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What is a &quot;Ratable Method&quot;?">
  The ratable method determines which dates the system uses to schedule the revenue. You can base the schedule on Sales Order dates, Billing/Invoice dates, or use the Sales Order Ratable method for a prorated amortization.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#performance-obligation:~:text=the%20dropdown%20options%3A-,Sales%20Order%20Ratable,-%3A%20Revenue%20amortized" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How do I handle contract date changes?">
  You can define how a date change affects the revenue waterfall.

- **Default (Blank)**: The waterfall is not changed.
- **Cumulative Date Change**: The entire waterfall (past and future) is recalculated based on the new dates.
- **Prospective Date Change**: Only future revenue payments are adjusted; past recognition is unaffected.
</Accordion>

<Accordion title="What is a &quot;Revenue Release&quot; event?">
  A revenue release event is a trigger that determines when revenue associated with a POB can be recognized. You can link recognition to specific events, like booking, billing, or delivery.
</Accordion>

<Accordion title="Can I have more than one release event for a single POB?">
  Yes, you can add multiple release events to a single POB. This is useful when revenue for one obligation is released in parts as different milestones are met.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#performance-obligation:~:text=Please%20note%20that%20these%20steps%20allow" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What is the most important rule for multiple release events?">
  The sum of the percentages for all release events on a single POB must equal 100%.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#performance-obligation:~:text=Please%20note%20that%20these%20steps%20allow" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Are there any restrictions on the 'Upon Booking' or 'Upon Billing' release events?">
  Yes. If you select 'Upon Booking' or 'Upon Billing' as a release event, the release percentage must be 100%. You cannot combine these events with any other release events on the same POB.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#performance-obligation:~:text=Please%20note%20that%20these%20steps%20allow" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Does every POB need a rule?">
  Yes. A POB requires at least one assigned rule to function correctly and be applied to transactions.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#performance-obligation:~:text=Save%20all%20changes.-,Adding%20POB%20rules,-To%20access%20POB" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How do I add a rule to a POB?">
  You can add a rule by navigating to the "Rules" section from the main menu (Rules → Rules) or by going to the "Rules" tab within a specific POB. Once there, click the "+" icon.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#performance-obligation:~:text=Save%20all%20changes.-,Adding%20POB%20rules,-To%20access%20POB" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Can I edit a POB rule from the main POB details page?">
  No. When you open a POB and scroll to the bottom, you can view the associated rules, but you cannot add or edit them from there. You must use Method 1 or Method 2.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#performance-obligation:~:text=Save%20all%20changes.-,Adding%20POB%20rules,-To%20access%20POB" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What is an &quot;attribute&quot; in a POB rule?">
  An attribute is the criterion used to link a transaction to a POB. For example, you can create a rule that assigns a POB based on a specific "Item" or "Account Code" on a transaction line.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#performance-obligation:~:text=Save%20all%20changes.-,Adding%20POB%20rules,-To%20access%20POB" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Can I change the priority of my POB rules?">
  Yes. You can change the hierarchy of rules by clicking and dragging the drag icon to reorder them. The system evaluates rules from top to bottom.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#performance-obligation:~:text=Save%20all%20changes.-,Adding%20POB%20rules,-To%20access%20POB" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How do I delete a POB rule?">
  Select the rule you wish to remove and click the "Delete" icon. Remember to save your changes to confirm the deletion.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#performance-obligation:~:text=Save%20all%20changes.-,Adding%20POB%20rules,-To%20access%20POB" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How can I update an SSP Analyzer with a new product or change the analysis for existing products?">
  For data integrity, an SSP Analyzer can't be modified after it's been approved.

To incorporate new products or update your analysis for existing items, you must create a new SSP Analyzer. This new analyzer uses all the data integrated up to that point, so you can perform a fresh and accurate analysis.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#performance-obligation:~:text=Configuring%20the%20SSP%20Analyzer%20for%20data%20upload" target="_blank">Learn more →</a>

</Accordion>

# Application setup

<Accordion title="How do I create and manage Books in the Recurly RevRec application setup?">
  Books are managed within the Application Setup section. Follow the instructions in the Setup: Books documentation.

<a href="https://docs.recurly.com/recurly-revrec/docs/setup#books:~:text=Key%20details-,Books,-In%20Recurly%20Revenue" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What are Business Events and how do I configure them in Recurly RevRec?">
  Business Events configuration is part of the Application Setup and dictates how transactions are processed. Refer to the Setup: Business Events documentation for details.

<a href="https://docs.recurly.com/recurly-revrec/docs/setup#books:~:text=its%20respective%20contracts.-,Business%20events,-In%20Recurly%20Revenue" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Where can I find information on setting up Segments for the revenue recognition module?">
  Information on setting up Segments is available under the Application Setup documentation. See the Setup: Segments section for configuration.

<a href="https://docs.recurly.com/recurly-revrec/docs/setup#books:~:text=to%20gather%20data.-,Segments,-Segments%20help%20define" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What are Contract Modification Rules and how do they automate one-off scenarios in Recurly RevRec?">
  Contract Modification Rules configuration is detailed in the Application Setup section, providing steps for automating change scenarios. Find the guidance in the Contract Modification documentation.

<a href="https://docs.recurly.com/recurly-revrec/docs/-contract-modification#:~:text=Powered%20by-,Contract%20modification,-Discover%20the%20intricacies" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How are Holds used in Recurly RevRec, and what is the setup process?">
  Holds are used to pause revenue recognition postings. Their setup is documented under Rules. The documentation for Holds can be found here.

<a href="https://docs.recurly.com/recurly-revrec/docs/rules#:~:text=revenue%20recognition%20calculations.-,Holds,-In%20Recurly%20Revenue" target="_blank">Learn more →</a>

</Accordion>

# Data transformation

<Accordion title="How do I set up and process Bundles (Product Bundles) for revenue recognition?">
  Setting up and processing Bundles is detailed in the Data Transformation section. Find the complete guide in the Product Bundle documentation.

<a href="https://docs.recurly.com/recurly-revrec/docs/product-bundle#:~:text=Powered%20by-,Product%20bundle,-Create%20and%20manage" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What are Data Rules and how are they configured for data transformation?">
  Configuration for Data Rules is a key part of data transformation in RevRec for standardizing data. Consult the dedicated Data Rules documentation for setup.

<a href="https://docs.recurly.com/recurly-revrec/docs/data-rules#:~:text=Powered%20by-,Data%20rules,-Apply%20custom%20logic" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How do I manage and use Data Sets for custom data ingestion in the RevRec application?">
  Data Sets allow for custom data ingestion and manipulation. The documentation for managing and using Data Sets is available here.

<a href="https://docs.recurly.com/recurly-revrec/docs/data-sets#:~:text=Powered%20by-,Datasets,-Unlock%20powerful%20analytics" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Why isn't my product bundle splitting correctly in the Revenue Workbench?">
  This typically happens when there is a mismatched Parent Identifier. For a bundle to split, the Parent Identifier on the contract's line items must exactly match the identifier in the product bundle setup. Please check to ensure these values are identical.

<a href="https://docs.recurly.com/recurly-revrec/docs/product-bundle#:~:text=Powered%20by-,Product%20bundle,-Create%20and%20manage" target="_blank">Learn more →</a>

</Accordion>

# Reports

<Accordion title="What are the key filters and data points available in the Revenue Insights Report?">
  The key filters and data points for the Revenue Insights Report are explained in the documentation for that report, which provides high-level revenue summaries. Review the Revenue Insights Report documentation for details.

<a href="https://docs.recurly.com/recurly-revrec/docs/revenue-insights-report#:~:text=Powered%20by-,Revenue%20insights%20report,-Explore%20the%20detailed" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How can I use the Cost Details Report (Expense) to analyze revenue recognition expenses?">
  The Cost Details Report provides a breakdown of expenses related to revenue recognition, linking them to revenue. The documentation on the Cost Details Report explains its usage and data.

<a href="https://docs.recurly.com/recurly-revrec/docs/cost-details-report#:~:text=Powered%20by-,Cost%20details%20report,-Explore%20the%20detailed" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="I need to reconcile my revenue journal entries. Where can I access the Audit Details Report?">
  The Audit Details Report provides the necessary granular information for reconciliation and controls. You can access the Audit Details Report documentation here.

<a href="https://docs.recurly.com/recurly-revrec/docs/audit-details-report#:~:text=Powered%20by-,Audit%20details%20report,-Explore%20the%20detailed" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How do I generate a report to identify contracts with SSP exceptions or other data quality issues?">
  The system provides an Exception Report (often used for SSP Exceptions) to flag data quality or configuration issues. See the Exception Report documentation for how to run it.

<a href="https://docs.recurly.com/recurly-revrec/docs/ssp-exception-report#:~:text=Powered%20by-,SSP%20exception%20report,-Explore%20the%20detailed" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Where do I find the documentation for generating and understanding the Journal Entries Report in RevRec?">
  Documentation on generating and understanding all Journal Entries is available in the Reports section. Consult the Reports: Journal Entries documentation for guidance.

<a href="https://docs.recurly.com/recurly-revrec/docs/transfer-accounting-details-report#:~:text=Powered%20by-,Transfer%20accounting%20details%20report,-Explore%20the%20detailed" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Does Recurly RevRec offer a report to track Deferred Revenue by contract?">
  Yes, deferred revenue tracking is covered in the reporting documentation. Check the relevant section of the documentation for Deferred Revenue reporting.

<a href="https://docs.recurly.com/recurly-revrec/docs/defer-revenue-waterfall-report#:~:text=Powered%20by-,Defer%20revenue%20waterfall%20report,-Explore%20the%20detailed" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What report provides detail on the ASC 606 5-Step Model process for an individual contract?">
  The Audit Details Report typically provides the most granular, step-by-step view of how the 5-Step model was applied to a contract. Refer to the Audit Details Report documentation.

<a href="https://docs.recurly.com/recurly-revrec/docs/audit-details-report#:~:text=Powered%20by-,Audit%20details%20report,-Explore%20the%20detailed" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="There is missing revenue in the waterfall report.">
  The missing revenue could be for various reasons. Check if the revenue that is missing is for the current period or prior periods. If it is for the current period, check if all the invoices are collected in the system or if any data is stuck in the stage. If all the invoices are collected,
</Accordion>

<Accordion title="How to reconcile between Revrec Invoices and Billing invoices?">
  The reconciliation can be done using the Invoice Summary report and Billing Transaction Details report.

- The Invoice Summary report is available in the Recurly Analytics Exports section and can be downloaded for the required month.
- The Billing Transaction report can be downloaded from the Reports section, also by month.
</Accordion>

<Accordion title="The reconciliation can be done for these 2 reports basing Invoice number as the main comparison factor.">
  Common reconciliation issues include missing or mismatched data between RevRec and accounting or BI tools, variances between reports and liabilities or expected results, and export errors or missing report elements. Examples:

- "Revenue recognition report that matches with liabilities"
- "Rev Rec data export to Snowflake"
- "Reports not containing headers"
</Accordion>

# Administration

<Accordion title="How is User Management and access configured in Recurly RevRec?">
  User Management and permissions are handled within the Administration section of the application. The User Management documentation provides details on setting up access.

<a href="https://docs.recurly.com/recurly-revrec/docs/access-management#:~:text=within%20the%20organization.-,Revenue%20Recognition%20user%20management,-Creating%20roles%20and" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What is the checklist or process for the Period Close Process?">
  The Period Close Process checklist is covered in the Administration section, ensuring compliance and data finalization. Find the necessary steps and procedures for Period Close here.

<a href="https://docs.recurly.com/recurly-revrec/docs/period-close-checklist#:~:text=Powered%20by-,Automatic%20month%20end%20close,-A%20succinct%20checklist" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What is the difference between Full Access, Read-only, and No Access permissions?">
  These permissions define a user's level of access within the system:

- **Full Access**: Grants the user permission to both view (read) and save changes (write).
- **Read-only**: Allows the user to view information but not to save any changes.
- **No Access**: Prevents the user from accessing the specific menu or feature entirely.
</Accordion>

<Accordion title="Can I customize user roles?">
  Yes, roles can be customized to meet your team's specific needs.

To customize a role:

1. Navigate to Access Management > Roles.
2. Select and modify the permissions for the desired role.
3. Save the changes when you're finished.

We recommend not changing the default settings for the Revenue Manager role.

<a href="https://docs.recurly.com/recurly-revrec/docs/access-management#:~:text=Modifying%20user%E2%80%99s%20privileges%20within%20the%20platform" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How do I add a new user to RevRec?">
  New users must be added through the Recurly Billing platform, not directly in RevRec.

1. Log in to your Recurly Billing platform.
2. Go to the Admin section and add a new user using their email address.
3. Assign the user a role that has Revenue Recognition access enabled. This step is required for the user to access RevRec.

<a href="https://docs.recurly.com/recurly-revrec/docs/access-management#:~:text=Creating%20a%20role%20within%20the%20platform" target="_blank">Learn more →</a>

</Accordion>

# Self-service onboarding

<Accordion title="What happens if we ignore credit transactions?">
  Any credit (goodwill, on-account, prepayment) will not be considered in revenue recognition calculations.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-wizard#:~:text=Step%206%3A-,Handling%20credit%20transactions,-This%20feature%20is" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Can we exit the onboarding wizard and resume later?">
  Yes. Progress is saved automatically. Any user with the right permissions can continue the setup.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-wizard#:~:text=in%20any%20order.-,Note%3A,-You%20can%20safely" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What does the Global Reporting Currency affect?">
  It determines the currency used in Revenue Recognition Reports and is separate from your main Recurly site currency.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-wizard#:~:text=Step%204%3A-,Setting%20up%20global%20reporting%20currency,-It%20is%20required" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What if a product is missing accounting codes?">
  Default settings will be used, but it is highly recommended to manually assign rules and codes for accurate reporting.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-wizard#:~:text=Step%201%3A-,Assigning%20GL%20accounts%20to%20business%20entities,-Assigning%20General%20Ledger" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How do I know if activation was successful?">
  You’ll receive a confirmation email, and the activation in-progress notification will disappear from your dashboard.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-wizard#:~:text=Step%208%3A-,Activating%20Revenue%20Recognition,-Once%20all%20the" target="_blank">Learn more →</a>

</Accordion>

# Stage area

<Accordion title="Why is my invoice missing from the Workbench and reports?">
  If an invoice you integrated doesn't appear in the Workbench or your reports, check the Staging Area. Invoices are often held there due to processing errors. Our documentation provides a guide to common staging errors and how to resolve them.

<a href="https://docs.recurly.com/recurly-revrec/docs/imports-exports#:~:text=with%20established%20rules.-,Stage%20area,-The%20Stage%20Area" target="_blank">Learn more →</a>

</Accordion>

# Credit events

<Accordion title="What are the credit-event lines that can be seen in a few contracts?">
  Whenever a credit transaction flows into Revrec from the Recurly, a credit-event line is created to keep track of such credits and to balance out them once fully used.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-credits#:~:text=Powered%20by-,Credits,-Maximize%20customer%20satisfaction" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How are credit-events  shown in Revrec?">
  Credits can arise in different situations. Based on how a credit is given, the recognition or treatment differs in RevRec as follows:

- **Goodwill Credit**: A free, promotional credit given to a customer to encourage their first or future purchases. It appears as a credit invoice in Recurly and flows into RevRec as a single line, with any redemption flowing in as a separate line. These lines can be identified based on the origin (credit-event) and plan code.
- **On Account Credit**: Typically issued as an alternative to a cash refund — for instance, when a customer cancels a subscription. It keeps the value within the customer's account for future use, and flows into RevRec as a single line, with any redemption flowing in as a separate line. These lines can be identified based on the origin (credit-event).
- **Prepayment Credit**: A credit balance created when a customer pays an amount in advance for future services or subscriptions, funded by the customer themselves. It flows into RevRec as one SO line but with two invoices, and any adjustment of credit flows in as a new line.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-credits#:~:text=Powered%20by-,Credits,-Maximize%20customer%20satisfaction" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How can I see a customer's total available credit balance?">
  You can view the total available credit balance for any customer directly within their account information page in Recurly.The sum of the "Sell Price" for all active credit lines in Recurly will equal the customer's total credit balance.
</Accordion>

<Accordion title="How can I identify credit-related transactions in Revrec?">
  All credit-related transactions can be identified in Revrec by looking at the line item's origin, which will be credit-event. The specific type of credit or action (e.g., redemption, void) can be determined by its plan code.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-credits#:~:text=Powered%20by-,Credits,-Maximize%20customer%20satisfaction" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How are Goodwill Credits and their usage tracked in RevRec?">
  Goodwill credit transactions appear as distinct lines in RevRec. You can identify them using the following plan codes:

- **Credit Issued**: `credit-goodwill`
- **Credit Used/Redeemed**: `credit-goodwill-redeemed`
- **Credit Canceled/Voided**: `credit-goodwill-voided`

<a href="https://docs.recurly.com/recurly-revrec/docs/goodwill-credit#:~:text=Powered%20by-,Goodwill%20credit,-Boost%20purchases%20by" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What happens if a Goodwill Credit is given by mistake or is never used?">
  If a Goodwill Credit needs to be canceled, it can be voided. A voided credit is no longer available for the customer to use, and a corresponding line item with the plan code Credit-goodwill-voided will appear in Revrec to reflect this reversal.

<a href="https://docs.recurly.com/recurly-revrec/docs/goodwill-credit#:~:text=In%20instances%20where%20goodwill%20credit%20is%20issued%20erroneously%20or%20remains%20unused%2C%20it%20can%20be%20voided%2C%20removing%20the%20balance%20from%20the%20customer%27s%20account.%20This%20action%2C%20along%20with%20all%20other%20credit%20transactions%2C%20is%20recorded%20in%20Revenue%20Recogntion%2C%20ensuring%20comprehensive%20financial%20oversight." target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How is an On Account Credit created in our billing system?">
  When an On Account Credit is issued, a specific credit invoice is generated in Recurly. This invoice will show the initial credit amount and will be updated to reflect the remaining balance as the credit is redeemed over time.

<a href="https://docs.recurly.com/recurly-revrec/docs/on-account-credit#:~:text=Powered%20by-,On%2Daccount%20credit,-Leverage%20your%20on" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How can I differentiate the various On Account Credit activities in Revrec?">
  Each activity has a unique plan code associated with the credit-event origin:

- **Credit Issued**: `credit-on-account`
- **Credit Used/Redeemed**: `credit-on-account-redeemed`
- **Credit Canceled/Voided**: `credit-voided`
- **Credit Refunded (paid out as cash)**: `credit-paid`

<a href="https://docs.recurly.com/recurly-revrec/docs/on-account-credit#:~:text=Accounting%20table%20for%20on%2Daccount%20credits" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What makes a Prepayment Credit different from the other two credit types?">
  A Prepayment Credit is funded directly by the customer. They pay an amount in advance, which is then held as a credit balance in their account to be used for future subscription payments or purchases.

<a href="https://docs.recurly.com/recurly-revrec/docs/prepayment-credit#:~:text=Powered%20by-,Prepayment%20credit,-Prepayment%20credit%20in" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Why do I see two credit event  invoices in Recurly when a Prepayment Credit is issued?">
  Two invoices are generated for a prepayment to ensure clear accounting:

- **Payment Invoice**: Acknowledges receipt of the customer's advance payment.
- **Credit Invoice**: Reflects that the paid amount has been converted into a usable credit balance in the customer's account.

<a href="https://docs.recurly.com/recurly-revrec/docs/prepayment-credit#:~:text=transparency%20and%20compliance.-,Key%20details,-Customers%20are%20encouraged" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How are Prepayment Credits and their adjustments tracked in Revrec?">
  You can track these transactions in RevRec using the following plan codes:

- **Credit Issued**: `credit-prepayment`
- **Credit Used/Redeemed**: `credit-prepayment-redeemed`
- **Credit Canceled/Voided**: `credit-prepayment-voided`

<a href="https://docs.recurly.com/recurly-revrec/docs/prepayment-credit#:~:text=Prepayment%20credits%20are%20integrated%20into%20the%20Revenue%20Recognition%20(RevRec)%20system%20as%20a%20single%20Sales%20Order%20(SO)%20line%2C%20accompanied%20by%20two%20invoices.%20Adjustments%20to%20the%20credit%20are%20recorded%20as%20new%20lines%2C%20identifiable%20by%20their%20origin%20and%20plan%20code." target="_blank">Learn more →</a>

</Accordion>

# Period close process

<Accordion title="What does the error in the system task &quot;Data processed for the current open period&quot; mean?">
  **Reason:** Recurly invoices for the current open period have not been successfully transferred into RevRec.

**Solution:** Initiate the billing integration job to synchronize the missing invoices. After the integration completes successfully, click Retry. The system will not allow the period close to proceed until all invoices are synced.

<a href="https://docs.recurly.com/recurly-revrec/docs/period-close-checklist#:~:text=What%20does%20the%20error%20in%20the%20system%20task%20%22Data%20processed%20for%20the%20current%20open%20period%22%20mean%3F" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What does the error in the system task “Billing pending processing or Stuck in Stage” mean?">
  **Reason:** Billing data or other uploaded transaction data for the current or a previous open period is stuck in the staging area and has not been processed.

**Solution:**

1. Generate Stage Reports by navigating to Reports → Stage to find the specific transactions that are stuck.
2. Review and process the stuck data to resolve any underlying errors.
3. Once the data flows correctly into RevRec, click Retry on the period close task to continue.

Refer to the Stage Errors FAQs below for help resolving specific stage data errors.

<a href="https://docs.recurly.com/recurly-revrec/docs/period-close-checklist#:~:text=What%20does%20the%20error%20in%20the%20system%20task%20%E2%80%9CBilling%20pending%20processing%20or%20Stuck%20in%20Stage%E2%80%9D%20mean%3F" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What does the error in the system task “Transfer Journals” mean?">
  **Reason:** Transfer Journal Cards for the primary book have not been approved or summarized.

**Solution:**

1. Go to Import/Export → Transfer JE to locate the journals that are still open.
2. Approve and summarize all open journals.
3. Click Retry. This step ensures all journal entries are properly accounted for before closing the period.

<a href="https://docs.recurly.com/recurly-revrec/docs/period-close-checklist#:~:text=What%20does%20the%20error%20in%20the%20system%20task%20%E2%80%9CTransfer%20Journals%E2%80%9D%20mean%3F" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What does the error in the system task “Review the Accounted Reports” mean?">
  **Reason:** There are summarization issues or balance discrepancies in key financial reports.

**Solution:**

1. Review the roll-forward reports (like Liability and Asset Balances) and verify that all unaccounted columns show zero.
2. Confirm that the beginning balances for the current period match the ending balances from the previous period.
3. Check that the revenue waterfall aligns with the scheduled balances.
4. If you cannot identify the specific report causing the issue, please contact Recurly Support for assistance.

<a href="https://docs.recurly.com/recurly-revrec/docs/period-close-checklist#:~:text=What%20does%20the%20error%20in%20the%20system%20task%20%E2%80%9CReview%20the%20Accounted%20Reports%E2%80%9D%20mean%3F" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What happens if we close the period without integrating the invoices?">
  The revenue for the month in which the invoices weren't integrated will be nil. You can import these invoices into the current open period to ensure they're accounted for.

The new period close process won't allow the period to close if there are any missing invoices in Revenue Recognition.

<a href="https://docs.recurly.com/recurly-revrec/docs/period-close-checklist#:~:text=Recurly%20invoices%20for%20the%20current%20open%20period%20have%20not%20been%20successfully%20transferred%20into%20RevRec." target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Is it possible to reopen a closed period?">
  No, a period that has been closed cannot be reopened. Any transactions that belong to a closed period can be loaded into the current open period.

<a href="https://docs.recurly.com/recurly-revrec/docs/period-close-checklist#:~:text=Is%20it%20possible%20to%20reopen%20a%20closed%20period%3F" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Will the new period close process allow closing the period if invoices haven't been integrated?">
  No, the new period close process has a built-in check that prevents the period from being closed until all relevant invoices have been integrated.

<a href="https://docs.recurly.com/recurly-revrec/docs/period-close-checklist#:~:text=Will%20the%20new%20period%20close%20process%20allow%20closing%20the%20period%20if%20invoices%20haven%27t%20been%20integrated%3F" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="The data in the stage area is not needed, but the system is preventing the period close. What can be done?">
  The system will not allow the period to be closed while there is still data in the staging area, even if that data is not required. If the data in the staging area is not required, you must manually delete it. The period close process will only continue once the stage is empty.

<a href="https://docs.recurly.com/recurly-revrec/docs/period-close-checklist#:~:text=The%20data%20in%20the%20stage%20area%20is%20not%20needed%2C%20but%20the%20system%20is%20preventing%20the%20period%20close.%20What%20can%20be%20done%3F" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What reports does the system check during the validation step?">
  The system task checks for the following alignments in the reports:

- The unaccounted column must be zero in the liability balance and asset balance reports.
- The beginning balance of the current period must match the ending balance of the previous period in the liability and asset balance reports.
- The total of the revenue waterfall report should match the scheduled balances.

<a href="https://docs.recurly.com/recurly-revrec/docs/period-close-checklist#:~:text=What%20does%20the%20system%20check%20during%20the%20validation%20step%3F" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="A journal entry is approved, but the period close process is stuck on the “transfer journal entry” step. Why?">
  Even though a journal entry is marked as "Approved," the task will not be completed. You must also ensure the journal entry is “Summarized.” The "transfer journal entries" step will only be marked as complete after the entries are both approved and summarized.
</Accordion>

<Accordion title="Can I skip a user-created task?">
  A user-created task can only be skipped if it was marked as optional during its creation. Mandatory tasks cannot be skipped.

<a href="https://docs.recurly.com/recurly-revrec/docs/period-close-checklist#:~:text=Optional%20tasks%20may%20be%20set%20to%20Skipped%20if%20you%20do%20not%20need%20to%20complete%20them" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Can I add a new user task for the current period?">
  No. A user task added during the current period will only become visible and active in the period close process starting from the next period. You cannot add a new task for a period that is already in progress.

<a href="https://docs.recurly.com/recurly-revrec/docs/period-close-checklist#can-i-add-a-new-user-task-for-the-current-period:~:text=Can%20I%20add%20a%20new%20user%20task%20for%20the%20current%20period%3F" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Can I delete a user task in the current period?">
  Yes, you can delete a user task. However, the deletion will only take effect from the following period. The task will remain part of the period close checklist for the current period.

<a href="https://docs.recurly.com/recurly-revrec/docs/period-close-checklist#:~:text=Can%20I%20delete%20a%20user%20task%20in%20the%20current%20period%3F" target="_blank">Learn more →</a>

</Accordion>

# Stage errors

<Accordion title="What does the &quot;Debit Account is Blank&quot; or &quot;Credit Account is Blank&quot; error mean?">
  **Reason:** This error indicates that a transaction line is missing its assigned debit or credit account.

**Solution:** Please review the system configurations and assign the correct debit and credit accounts to the relevant lines to resolve the issue.

<a href="https://docs.recurly.com/recurly-revrec/docs/contract-stage-report#:~:text=encountered%20during%20processing.-,Contract%20stage%20errors,-The%20following%20table" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Why am I seeing the error &quot;Updated SO Amount is in a different sign than previous Billed Amount&quot;?">
  **Reason:** This happens when an update to a Sales Order (SO) has an amount with a different sign (positive/negative) than the original SO. For example, a positive SO amount cannot be updated with a negative amount.

**Solution:** Ensure that the updated SO amount maintains the same sign as the original.

<a href="https://docs.recurly.com/recurly-revrec/docs/contract-stage-report#:~:text=encountered%20during%20processing.-,Contract%20stage%20errors,-The%20following%20table" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What causes the &quot;Error Processing So update&quot;?">
  **Reason:** This error can occur in the case of a Credit Memo Request (CMR) when the updated Sales Order (SO) amount is less than the amount that has already been billed.

**Solution:** Verify the SO update amount and ensure it is not less than the billed amount.

<a href="https://docs.recurly.com/recurly-revrec/docs/contract-stage-report#:~:text=encountered%20during%20processing.-,Contract%20stage%20errors,-The%20following%20table" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What does &quot;Updated SO Amount is less than Billed Amount&quot; mean?">
  **Reason:** This error indicates that the total billed amount for a line has exceeded the total amount specified in the Sales Order (SO).

**Solution:** To proceed, you must either increase the SO amount to match or exceed the billed amount, or enable overage in the system settings.

<a href="https://docs.recurly.com/recurly-revrec/docs/contract-stage-report#:~:text=encountered%20during%20processing.-,Contract%20stage%20errors,-The%20following%20table" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Why am I getting the &quot;Bundle child updates are not allowed&quot; error?">
  **Reason:** The revenue recognition module does not permit direct updates to the child lines of a bundle.

**Solution:** Updates should be made to the parent bundle line, not the individual child components.

<a href="https://docs.recurly.com/recurly-revrec/docs/contract-stage-report#:~:text=encountered%20during%20processing.-,Contract%20stage%20errors,-The%20following%20table" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How do I fix &quot;Pob Rule setup is missing in the book&quot; or &quot;Pob setup missing for some lines in this contract in book&quot;?">
  **Reason:** These errors mean that one or more lines in the contract do not have a Price Obligation (POB) rule configured. The system requires POB rules to correctly recognize revenue.

**Solution:** Navigate to the POB rules section for the contract and configure the appropriate POB rules for all lines that are missing them.

<a href="https://docs.recurly.com/recurly-revrec/docs/contract-stage-report#:~:text=encountered%20during%20processing.-,Contract%20stage%20errors,-The%20following%20table" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What should I do about an &quot;Invalid References on INV&quot; error?">
  **Reason:** The reference invoice number or reference invoice line number provided is incorrect.

**Solution:** Please check and correct the reference invoice details.

<a href="https://docs.recurly.com/recurly-revrec/docs/doc-stage-details-report#doc-stage-errors:~:text=encountered%20during%20processing.-,Doc%20stage%20errors,-The%20following%20table" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Why did I get the error &quot;Invalid INV. INV belongs to Material Right Contract&quot;?">
  **Reason:** The system does not allow an invoice to be associated with a material right contract line. Invoices linked to material rights cannot be collected.

**Solution:** Remove the invoice information from the material right line.

<a href="https://docs.recurly.com/recurly-revrec/docs/doc-stage-details-report#doc-stage-errors:~:text=encountered%20during%20processing.-,Doc%20stage%20errors,-The%20following%20table" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How do I resolve a &quot;Bill Amount is incorrect&quot; error?">
  **Reason:** The amount on the bill is not correct.

**Solution:** Please check and validate that the bill amount is accurate.

<a href="https://docs.recurly.com/recurly-revrec/docs/doc-stage-details-report#doc-stage-errors:~:text=encountered%20during%20processing.-,Doc%20stage%20errors,-The%20following%20table" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What does &quot;Original Credit Memo does not exist or already Cancelled&quot; mean?">
  **Reason:** This error occurs when you try to cancel a credit memo, but the reference details provided do not correspond to an existing, active credit memo in the system.

**Solution:** Re-upload the cancellation file with the correct reference invoice details.

<a href="https://docs.recurly.com/recurly-revrec/docs/doc-stage-details-report#doc-stage-errors:~:text=encountered%20during%20processing.-,Doc%20stage%20errors,-The%20following%20table" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How do I fix &quot;Original Invoice does not exist or already Cancelled&quot; or &quot;Original Invoice does not exist&quot;?">
  **Reason:** This error appears when a credit memo is uploaded with reference details for an invoice that does not exist or has already been cancelled.

**Solution:** Correct the reference invoice details in your upload file and re-process it.

<a href="https://docs.recurly.com/recurly-revrec/docs/doc-stage-details-report#doc-stage-errors:~:text=encountered%20during%20processing.-,Doc%20stage%20errors,-The%20following%20table" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Why am I seeing &quot;Invalid INV. SO not present in System&quot;?">
  **Reason:** This error occurs when an invoice is loaded with a reference to a Sales Order (SO) that is not in the system.

**Solution:** Please re-process the file with a valid and existing SO number.

<a href="https://docs.recurly.com/recurly-revrec/docs/doc-stage-details-report#doc-stage-errors:~:text=encountered%20during%20processing.-,Doc%20stage%20errors,-The%20following%20table" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What should I do for an &quot;Error Loading SO Line&quot;?">
  **Reason:** The associated Sales Order (SO) line has not been successfully processed from the contract stage into the system.

**Solution:** Check the contract stage for the relevant SO and ensure it is processed successfully before you proceed with the invoice.

<a href="https://docs.recurly.com/recurly-revrec/docs/contract-stage-report#:~:text=encountered%20during%20processing.-,Contract%20stage%20errors,-The%20following%20table" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How do I resolve &quot;CM cannot be processed as INV is in error&quot;?">
  **Reason:** You are trying to process a Credit Memo (CM) against an invoice that is currently in an error state in the stage area.

**Solution:** First, review and resolve the error associated with the original invoice. Once the invoice is processed successfully, you can process the credit memo.

<a href="https://docs.recurly.com/recurly-revrec/docs/doc-stage-details-report#doc-stage-errors:~:text=encountered%20during%20processing.-,Doc%20stage%20errors,-The%20following%20table" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What causes the &quot;Cumulative bill amount is over sell price&quot; error?">
  **Reason:** This error occurs when the total value of invoices for a subscription exceeds the sell price, and the system is not configured to allow over-billing.

**Solution:** To resolve this, navigate to Profiles → Overage and enable the overage setting.

<a href="https://docs.recurly.com/recurly-revrec/docs/doc-stage-details-report#doc-stage-errors:~:text=encountered%20during%20processing.-,Doc%20stage%20errors,-The%20following%20table" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What does the &quot;Invalid Cost: SO not present in System&quot; error mean?">
  **Reason:** The Sales Order (SO) number referenced in the cost file is incorrect or does not exist in the system.

**Solution:** Please verify the SO number in your cost file is accurate and re-upload the file.

<a href="https://docs.recurly.com/recurly-revrec/docs/contract-stage-report#:~:text=encountered%20during%20processing.-,Contract%20stage%20errors,-The%20following%20table" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="Why am I seeing &quot;Bundle child updates are not allowed&quot; in the Cost Stage?">
  **Reason:** The revenue recognition module does not permit direct updates to the child lines of a bundle, and this rule applies to cost updates as well.

**Solution:** Updates must be made at the parent bundle level.

<a href="https://docs.recurly.com/recurly-revrec/docs/contract-stage-report#:~:text=encountered%20during%20processing.-,Contract%20stage%20errors,-The%20following%20table" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How do I fix &quot;Invalid Cost Type. Cost Type Setup is missing&quot;?">
  **Reason:** The cost type specified is not valid because it has not been configured in the system.

**Solution:** Please revisit your configuration to ensure the cost type setup is correct. Refer to the user manual for more details on this setup.

<a href="https://docs.recurly.com/recurly-revrec/docs/contract-stage-report#:~:text=encountered%20during%20processing.-,Contract%20stage%20errors,-The%20following%20table" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What does &quot;Allocated Commission lines cannot be updated&quot; mean?">
  **Reason:** Once commission has been allocated to a line, the revenue recognition module does not allow that line to be updated.

**Solution:** Avoid attempting to update lines where commission has already been allocated. Any changes may require a new transaction or reversal.

<a href="https://docs.recurly.com/recurly-revrec/docs/contract-stage-report#:~:text=encountered%20during%20processing.-,Contract%20stage%20errors,-The%20following%20table" target="_blank">Learn more →</a>

</Accordion>

# Other questions

<Accordion title="">
  
</Accordion>

<Accordion title="">
  
</Accordion>

# Standard reports

<Accordion title="How do I access the Revenue Recognition reports in Recurly?">
  To access the reports, log in to your Recurly account, click on "Analytics" in the left-hand sidebar menu, and then select the desired report from the submenu that appears.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-standard-reports#:~:text=insights%20and%20accuracy.-,Accessing%20reports,-To%20retrieve%20the" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What are the main components of the report interface?">
  The report interface generally includes:

- **Report Filters**: To customize the data shown.
- **Report Metrics**: To display key data points.
- **Graphs and Visualizations**: To help understand the data.
- **Download Options**: To export the data.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-standard-reports#:~:text=access%20detailed%20insights.-,Report%20interface%20and%20navigation,-Upon%20accessing%20the" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="In what formats can I download the reports?">
  You can export report data in formats like CSV or Excel for further analysis or sharing.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-standard-reports#:~:text=access%20detailed%20insights.-,Report%20interface%20and%20navigation,-Upon%20accessing%20the" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What is the purpose of the Revenue Waterfall Report?">
  The Revenue Waterfall Report provides an analysis of how revenue is distributed across various accounting periods. It helps visualize how contracted revenue is recognized over time.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-standard-reports#:~:text=The%20Revenue%20Waterfall%20Report%20in%20Recurly%27s%20revenue%20recognition%20standard%20offers%20insightful%20analysis%20into%20revenue%20distribution%20across%20various%20periods" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What kind of data can I see in the Revenue Waterfall Report?">
  You can view detailed revenue and transaction data by customer account, plan, transaction, and company currency.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-standard-reports#:~:text=The%20Revenue%20Waterfall%20Report%20in%20Recurly%27s%20revenue%20recognition%20standard%20offers%20insightful%20analysis%20into%20revenue%20distribution%20across%20various%20periods" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What is the Liability Balance Report used for?">
  This report provides information about your deferred revenue balances, helping you track and manage them effectively.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-standard-reports#:~:text=Liability%20balance%20report" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How can I analyze deferred revenue using the Liability Balance Report?">
  You can review deferred revenue balances across different accounting periods, apply filters to break down the data by product or customer segment, and track balances by plan.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-standard-reports#:~:text=Liability%20balance%20report" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What information does the Transfer Accounting Report provide?">
  The Transfer Accounting Report offers extensive details on revenue transfers between different accounts or entities, including source and destination accounts and the amounts transferred.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-standard-reports#:~:text=systems%20or%20tools.-,Transfer%20accounting%20report,-The%20Transfer%20Accounting" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How can the Transfer Accounting Report help with financial accuracy?">
  It helps you identify any discrepancies or issues in revenue transfers, allowing you to verify the accuracy and integrity of your financial records.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-standard-reports#:~:text=systems%20or%20tools.-,Transfer%20accounting%20report,-The%20Transfer%20Accounting" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How can I customize my reports in Recurly?">
  You can customize reports by creating custom dimensions, changing column names, adding or removing fields, using different visualization options, applying filters, and using aggregation functions.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-standard-reports#:~:text=systems%20or%20tools.-,Reporting%20tips,-Customizing%20your%20reports" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What are custom dimensions?">
  Custom dimensions are user-created attributes that add more context to your data. They can be crafted from existing data fields or derived from calculations.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-standard-reports#:~:text=systems%20or%20tools.-,Reporting%20tips,-Customizing%20your%20reports" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How do I focus on the most important metrics in a report?">
  You can add and remove fields from your report menu to streamline the options and concentrate on the metrics and dimensions that are most vital to you.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-standard-reports#:~:text=systems%20or%20tools.-,Reporting%20tips,-Customizing%20your%20reports" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="How can I get a more focused view of my data?">
  You can use filters and slicers to view specific subsets of your data, allowing for more dynamic data exploration.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-standard-reports#:~:text=systems%20or%20tools.-,Reporting%20tips,-Customizing%20your%20reports" target="_blank">Learn more →</a>

</Accordion>

<Accordion title="What are aggregation functions and how are they useful?">
  Aggregation functions, such as "sum," allow you to calculate summary statistics for your data, which adds more depth to your analysis.

<a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-standard-reports#:~:text=systems%20or%20tools.-,Reporting%20tips,-Customizing%20your%20reports" target="_blank">Learn more →</a>

</Accordion>

<br />
