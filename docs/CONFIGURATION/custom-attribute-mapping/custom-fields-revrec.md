---
title: Custom fields for RevRec
excerpt: >-
  Map Recurly custom fields to RevRec attribute slots F36–F40 to carry
  contextual business data into your revenue recognition workflows, reports, and
  ERP output.  <br />
deprecated: false
hidden: false
metadata:
  robots: index
---
<div class="rp-page">
  <div class="rp-overview">RevRec custom fields let you carry contextual business data from your Recurly account directly into your revenue recognition workflows. Map up to five Recurly custom fields to RevRec's dedicated attribute slots — F36 through F40 — so your finance and operations teams have subscriber-level, subscription-level, and plan-level metadata right where they need it.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Available as part of Recurly RevRec</div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#definition"><span class="rp-toc-num">1</span>Definition</a>
    <a class="rp-toc-pill" href="#key-benefits"><span class="rp-toc-num">2</span>Key benefits</a>
    <a class="rp-toc-pill" href="#key-details"><span class="rp-toc-num">3</span>Key details</a>
    <a class="rp-toc-pill" href="#data-sync-behavior"><span class="rp-toc-num">4</span>Data sync behavior</a>
    <a class="rp-toc-pill" href="#pre-save-checklist"><span class="rp-toc-num">5</span>Pre-save checklist</a>
    <a class="rp-toc-pill" href="#faq"><span class="rp-toc-num">6</span>FAQ</a>
  </div>
</div>

### Prerequisites

<ul class="rp-list">
  <li>Custom fields must be created and configured in your Recurly account under <strong>Configuration → Custom Fields</strong> before they can be mapped in RevRec. RevRec reads from Recurly — it can't create fields independently.</li>
  <li>You've identified which Recurly custom fields to surface in RevRec, keeping in mind that only five slots are available.</li>
  <li>You've confirmed the correct field names, types, and entities (Account, Subscription, or Plan) for each custom field in Recurly. Data type defaults to Text in RevRec and can't be changed after saving.</li>
  <li>You have administrative permissions in RevRec to access Configuration settings.</li>
</ul>

### Limitations

<ul class="rp-list">
  <li>RevRec supports a maximum of five custom field mappings, corresponding to slots F36 through F40.</li>
  <li>Once a slot's configuration is saved, the Upload Name, Data Type, and RSM checkbox state are permanently frozen and can't be edited through the UI. Changes require a support ticket.</li>
  <li>Custom attribute configuration is forward-looking only — historical subscription data already processed in RevRec won't be retroactively updated.</li>
  <li>Data type is always Text when an RSM slot is activated. No other data types are supported.</li>
  <li>If a mapped Recurly custom field is later deleted in Recurly, the corresponding RevRec slot returns blank values and can't be remapped without a support ticket.</li>
</ul>

# Definition

<div class="rp-definition">RevRec custom fields let you carry contextual business data from your Recurly account directly into your revenue recognition workflows. By mapping Recurly custom fields to RevRec's dedicated attribute slots, your finance and operations teams gain access to subscriber-level, subscription-level, and plan-level metadata — right where they need it for revenue reporting, contract analysis, and downstream ERP output.</div>

# Key benefits

<div class="rp-benefits">
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-layer-group" aria-hidden="true"></i></div>
    <strong>Richer revenue context</strong>
    <span>Attach meaningful business attributes — such as customer region, contract tier, or product category — to your RevRec data for deeper insight into how and why revenue is recognized.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-rotate" aria-hidden="true"></i></div>
    <strong>Automatic data sync</strong>
    <span>Custom attribute values update automatically with every integration run between Recurly and RevRec — no manual work required to keep your data current.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-sliders" aria-hidden="true"></i></div>
    <strong>Flexible entity support</strong>
    <span>Custom fields can be sourced from Account, Subscription, and Plan objects in Recurly, giving you broad flexibility in how you classify revenue recognition treatment across your catalog.</span>
  </div>
</div>

# Key details

## Understanding the attribute slots: F36–F40

RevRec reserves five dedicated attribute slots — F36, F37, F38, F39, and F40 — for custom field mapping from Recurly. By default, all five function as standard RevRec attributes with no connection to Recurly data. When you activate a slot by enabling the RSM checkbox, it becomes a Recurly-linked custom attribute that pulls data from a corresponding Recurly custom field on every integration run.

<table class="rp-params">
  <tr class="rp-thead-row"><td>Slot</td><td>Default state</td><td>RSM-activated state</td></tr>
  <tr><td>F36</td><td>Standard RevRec attribute</td><td>Linked to a Recurly custom field</td></tr>
  <tr><td>F37</td><td>Standard RevRec attribute</td><td>Linked to a Recurly custom field</td></tr>
  <tr><td>F38</td><td>Standard RevRec attribute</td><td>Linked to a Recurly custom field</td></tr>
  <tr><td>F39</td><td>Standard RevRec attribute</td><td>Linked to a Recurly custom field</td></tr>
  <tr><td>F40</td><td>Standard RevRec attribute</td><td>Linked to a Recurly custom field</td></tr>
</table>

Each slot holds exactly one Recurly custom field mapping. Once a slot is activated and saved, its configuration is permanently frozen.

## Step 1 — Create custom fields in Recurly

Custom fields must exist in Recurly before they can be mapped in RevRec.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Log in to Recurly</h4><p>Log in to your Recurly account.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Open Custom Fields</h4><p>Navigate to <strong>Configuration → Custom Fields</strong>.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Define the field</h4><p>Set the field name, entity type (Account, Subscription, or Plan), and any display settings.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Save</h4><p>Save the field, then repeat for each custom field you intend to map in RevRec — up to a maximum of five.</p></div>
  </div>
</div>

Prioritize the fields your finance and operations teams rely on most for revenue reporting and contract analysis before moving on to Step 2.

## Step 2 — Configure attribute labels

Once your custom fields exist in Recurly, map them to the F36–F40 slots in RevRec through Attribute Labels.

### Navigate to Attribute Labels

Go to **Configuration → Attribute Labels** and locate the slot you want to configure (F36–F40).

### Activate the RSM checkbox

The RSM checkbox converts a standard RevRec attribute into a Recurly-linked custom field.

<ul class="rp-list">
  <li><strong>Unchecked (default):</strong> The slot functions as a standard RevRec attribute with no connection to Recurly.</li>
  <li><strong>Checked:</strong> The slot is activated for RSM integration. The Upload Name dropdown becomes visible and is required before saving.</li>
</ul>

To activate a slot, check the RSM checkbox for your chosen slot.


<Image src="https://files.readme.io/b93fe5f35a0e6242340c17a0e6053028a899eb4c7cccabeb38898bf7edb32ff9-Image_1.png" align="center" width="80%" border={true} />


The Upload Name dropdown appears and becomes mandatory. Data Type automatically defaults to Text — this can't be changed.

### Select the Upload Name

The Upload Name dropdown lists all custom fields currently configured in your connected Recurly account.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open the dropdown</h4><p>Select the <strong>Upload Name</strong> dropdown.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Select the field</h4><p>Choose the Recurly custom field you want to map to this slot. Review your selection carefully — this is a one-time, permanent assignment.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/1acb179bd4f73ab6b75c0979f7786f28f961b78f1b987476ad133d839a5177f1-Image_2.png" align="center" width="80%" border={true} />


### Save the configuration

Before selecting **Save**, confirm the following for each activated slot:

<ul class="rp-list">
  <li>The RSM checkbox is checked.</li>
  <li>The correct Upload Name is selected.</li>
  <li>The Data Type (Text) is accepted.</li>
</ul>

<div class="rp-callout rp-callout-warning">
  <div><strong><i class="fa-solid fa-triangle-exclamation" aria-hidden="true"></i> Permanent freeze — read before saving</strong>Once saved, the Upload Name, Data Type, and RSM checkbox state for each attribute slot are permanently frozen. No further edits can be made through the UI. If a change is required after saving, raise a support ticket with the engineering team.</div>
</div>

## UI behavior reference

### Before saving

<table class="rp-params">
  <tr class="rp-thead-row"><td>Action</td><td>Result</td></tr>
  <tr><td>Check the RSM checkbox</td><td>Activates the slot. Upload Name becomes required. Data Type defaults to Text.</td></tr>
  <tr><td>Uncheck the RSM checkbox</td><td>Resets Upload Name to default. No configuration is persisted. Slot remains a standard attribute.</td></tr>
  <tr><td>Change Upload Name selection</td><td>New selection is applied until Save is selected.</td></tr>
</table>

### After saving

<table class="rp-params">
  <tr class="rp-thead-row"><td>Field</td><td>State</td></tr>
  <tr><td>Upload Name</td><td>Frozen — can't be modified.</td></tr>
  <tr><td>Data Type</td><td>Frozen — can't be modified.</td></tr>
  <tr><td>RSM checkbox</td><td>Frozen — can't be checked or unchecked.</td></tr>
  <tr><td>Other attribute label checkboxes</td><td>Can be changed as needed.</td></tr>
  <tr><td>Application/display name</td><td>Can be modified after saving.</td></tr>
</table>

# Data sync behavior

Custom attribute data updates automatically as part of every standard integration run between Recurly and RevRec — there's no separate sync schedule.

<ul class="rp-list">
  <li><strong>New subscriptions:</strong> Custom attribute values are captured at the time of subscription creation and flow into RevRec on the next integration run.</li>
  <li><strong>Subscription changes:</strong> If a custom field value changes on an existing subscription in Recurly, the updated value syncs to RevRec on the next integration run.</li>
  <li><strong>Historical data:</strong> Custom attribute configuration applies forward only. Subscriptions and contracts already processed in RevRec before the attribute was configured won't be backfilled.</li>
  <li><strong>Blank values:</strong> If a custom field has no value in Recurly for a given record, RevRec displays the attribute as blank. This is expected behavior and doesn't indicate an error or sync failure.</li>
</ul>

# Pre-save checklist

Use this checklist before saving your configuration to avoid irreversible mistakes.

<ul class="rp-list">
  <li>Custom fields have been created in Recurly.</li>
  <li>Custom fields have been created in RevRec (<strong>Configuration → Create New Custom Fields</strong>).</li>
  <li>You've identified which slots (F36–F40) will be used for RSM mapping.</li>
  <li>The RSM checkbox is checked for each slot you want to activate.</li>
  <li>An Upload Name has been selected from the dropdown for each activated slot.</li>
  <li>Data Type (Text) is confirmed and accepted for each activated slot.</li>
  <li>All selections have been reviewed — changes can't be made after saving.</li>
  <li>Team members who rely on this data have been informed that custom attributes apply to future subscriptions and changes only.</li>
</ul>

# FAQ

<Accordion title="Can I edit the Upload Name after saving?">
  No. Once saved, the Upload Name is permanently frozen. If a change is required, raise a support ticket and the engineering team will assist. Note that the display or application name shown in the RevRec UI can still be modified after saving.
</Accordion>

<Accordion title="What happens if I uncheck the RSM checkbox before saving?">
  The Upload Name reverts to its default value and no configuration is saved for that slot. The slot continues to function as a standard RevRec attribute with no Recurly connection.
</Accordion>

<Accordion title="What happens if I check the RSM checkbox but don't select an Upload Name before saving?">
  RevRec won't permit saving without a valid Upload Name selection. The Upload Name field is mandatory whenever the RSM checkbox is checked.
</Accordion>

<Accordion title="What happens if a Recurly custom field mapped in RevRec is later deleted in Recurly?">
  The corresponding RevRec slot stops receiving data and displays blank values for that attribute. The slot itself remains frozen in its configured state. To remap it to a different Recurly custom field, raise a support ticket with the engineering team.
</Accordion>

<Accordion title="Can I map more than five custom fields in RevRec?">
  No. RevRec supports a maximum of five custom fields, corresponding to slots F36 through F40. Prioritize the most critical fields for revenue reporting and contract analysis before configuring.
</Accordion>

<Accordion title="How often is custom attribute data synced from Recurly?">
  Custom attribute data updates with every integration run between Recurly and RevRec. There's no separate or independent sync schedule for custom attributes.
</Accordion>

<Accordion title="Does custom attribute configuration apply to existing historical subscriptions?">
  No. Custom attribute configuration is forward-looking only. It applies to new subscriptions created after configuration is in place, and to future changes made to existing subscriptions. Historical records already processed in RevRec won't be retroactively updated.
</Accordion>

<Accordion title="What does RevRec display if a custom field has no value for a record in Recurly?">
  RevRec displays the attribute as blank for that record. This is expected behavior and doesn't indicate a configuration error or sync failure.
</Accordion>

<Accordion title="What entities can custom fields be associated with in Recurly?">
  Custom fields in Recurly can be associated with Account, Subscription, and Plan entities. Confirm the entity type of each field in Recurly before mapping it to a RevRec slot.
</Accordion>

<Accordion title="Can I reuse a slot that was previously configured?">
  No. Once a slot's RSM configuration is saved, it's permanently frozen. If the mapped Recurly field is deleted or you need a different mapping, raise a support ticket for engineering assistance. Slots can't be reset or reused through the UI.
</Accordion>

<br />
