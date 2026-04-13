---
title: Custom fields
excerpt: Map Recurly custom fields to RevRec for richer revenue reporting and analysis.
deprecated: false
hidden: false
metadata:
  robots: index
---
# Overview

### Prerequisites

* Custom fields must be created and configured in your Recurly account under **Configuration → Custom Fields** before they can be mapped in RevRec. RevRec reads from Recurly — it cannot create fields independently.
* You have identified which Recurly custom fields to surface in RevRec, keeping in mind that only five slots are available.
* You have confirmed the correct field names, types, and entities (Account, Subscription, or Plan) for each custom field in Recurly. Data type defaults to Text in RevRec and cannot be changed after saving.
* You have administrative permissions in RevRec to access Configuration settings.

### Limitations

* RevRec supports a maximum of five custom field mappings, corresponding to slots F36 through F40.
* Once a slot's configuration is saved, the Upload Name, Data Type, and Recurly Subscription Management (RSM) checkbox state are permanently frozen and cannot be edited through the UI. Changes require a support ticket.
* Custom attribute configuration is forward-looking only — historical subscription data already processed in RevRec will not be retroactively updated.
* Data type is always Text when an RSM slot is activated. No other data types are supported.
* If a mapped Recurly custom field is later deleted in Recurly, the corresponding RevRec slot will return blank values and cannot be remapped without a support ticket.

# Definition

RevRec custom fields let you carry contextual business data from your Recurly account directly into your revenue recognition workflows. By mapping Recurly custom fields to RevRec's dedicated attribute slots, your finance and operations teams gain access to subscriber-level, subscription-level, and plan-level metadata — right where they need it for revenue reporting, contract analysis, and downstream ERP output.

# Key benefits

* **Richer revenue context**: Attach meaningful business attributes — such as customer region, contract tier, or product category — to your RevRec data, giving your team deeper insight into how and why revenue is recognized the way it is.
* **Automatic data sync**: Custom attribute values update automatically with every integration run between Recurly and RevRec, so there's no manual work required to keep your data current.
* **Flexible entity support**: Custom fields can be sourced from Account, Subscription, and Plan objects in Recurly, giving you broad flexibility in how you classify and differentiate revenue recognition treatment across your catalog.

# Key details

## Understanding the attribute slots: F36–F40

RevRec reserves five dedicated attribute slots — F36, F37, F38, F39, and F40 — for custom field mapping from Recurly. By default, all five slots function as standard RevRec attributes with no connection to Recurly data.

When you activate a slot by enabling the RSM checkbox, it becomes a Recurly-linked custom attribute that pulls data from a corresponding Recurly custom field on every integration run.

| Slot | Default state             | RSM-activated state              |
| ---- | ------------------------- | -------------------------------- |
| F36  | Standard RevRec attribute | Linked to a Recurly custom field |
| F37  | Standard RevRec attribute | Linked to a Recurly custom field |
| F38  | Standard RevRec attribute | Linked to a Recurly custom field |
| F39  | Standard RevRec attribute | Linked to a Recurly custom field |
| F40  | Standard RevRec attribute | Linked to a Recurly custom field |

Each slot holds exactly one Recurly custom field mapping. Once a slot is activated and saved, its configuration is permanently frozen.

***

## Step 1 — Create custom fields in Recurly

Custom fields must exist in Recurly before they can be mapped in RevRec.

1. Log in to your Recurly account.
2. Navigate to **Configuration → Custom Fields**.
3. Define the field name, entity type (Account, Subscription, or Plan), and any display settings.
4. Save the field.
5. Repeat for each custom field you intend to map in RevRec, up to a maximum of five.

Prioritize the fields your finance and operations teams rely on most for revenue reporting and contract analysis before moving on to configuration in RevRec.

***

## Step 2 — Configure attribute labels

Once your custom fields exist in Recurly, map them to the F36–F40 slots in RevRec through the Attribute Labels configuration.

### Navigate to attribute labels

Go to **Configuration → Attribute Labels** and locate the slot you want to configure (F36–F40).

### Activate the RSM checkbox

The RSM checkbox is the toggle that converts a standard RevRec attribute into a Recurly-linked custom field.

* **Unchecked (default)**: The slot functions as a standard RevRec attribute with no connection to Recurly.
* **Checked**: The slot is activated for RSM integration. The Upload Name dropdown becomes visible and is required before saving.

To activate a slot, check the RSM checkbox for your chosen slot.

<Image align="center" border={true} width="80% " src="https://files.readme.io/b93fe5f35a0e6242340c17a0e6053028a899eb4c7cccabeb38898bf7edb32ff9-Image_1.png" className="border" />

The Upload Name dropdown will appear and become mandatory. The Data Type will automatically default to Text — this cannot be changed.

### Select the upload name

The Upload Name dropdown lists all custom fields currently configured in your connected Recurly account.

1. Click the **Upload Name** dropdown.
2. Select the Recurly custom field you want to map to this slot.

<Image align="center" border={true} width="80% " src="https://files.readme.io/1acb179bd4f73ab6b75c0979f7786f28f961b78f1b987476ad133d839a5177f1-Image_2.png" className="border" />

Review your selection carefully — this is a one-time, permanent assignment.

### Save the configuration

Before clicking **Save**, review each activated slot and confirm:

* The RSM checkbox is checked for each slot you intend to activate
* The correct Upload Name is selected
* The Data Type (Text) is accepted

> ⚠️ **Warning — permanent freeze**
>
> Once saved, the Upload Name, Data Type, and RSM checkbox state for each attribute slot are permanently frozen. No further edits can be made through the UI. If a change is required after saving, raise a support ticket with the engineering team.

***

## UI behavior reference

### Before saving

| Action                       | Result                                                                                          |
| ---------------------------- | ----------------------------------------------------------------------------------------------- |
| Check the RSM checkbox       | Activates the slot; Upload Name becomes required; Data Type defaults to Text                    |
| Uncheck the RSM checkbox     | Resets Upload Name to default; no configuration is persisted; slot remains a standard attribute |
| Change Upload Name selection | New selection is applied until Save is clicked                                                  |

### After saving

| Field                            | State                                   |
| -------------------------------- | --------------------------------------- |
| Upload Name                      | Frozen — cannot be modified             |
| Data Type                        | Frozen — cannot be modified             |
| RSM checkbox                     | Frozen — cannot be checked or unchecked |
| Other attribute label checkboxes | Can be changed as needed                |
| Application/display name         | Can be modified after saving            |

***

## Data sync behavior

Custom attribute data is not managed on a separate sync schedule. It updates automatically as part of every standard integration run between Recurly and RevRec.

* **New subscriptions**: Custom attribute values are captured at the time of subscription creation and flow into RevRec on the next integration run.
* **Subscription changes**: If a custom field value changes on an existing subscription in Recurly, the updated value syncs to RevRec on the next integration run.
* **Historical data**: Custom attribute configuration applies forward only. Subscriptions and contracts already processed in RevRec before the attribute was configured will not be backfilled.
* **Blank values**: If a custom field has no value in Recurly for a given record, RevRec displays the attribute as blank. This is expected behavior and does not indicate an error or sync failure.

***

## Quick reference checklist

Use this checklist before saving your configuration to avoid irreversible mistakes.

* [ ] Custom fields have been created in Recurly
* [ ] Custom fields have been created in RevRec (**Configuration → Create New Custom Fields**)
* [ ] You have identified which slots (F36–F40) will be used for RSM mapping
* [ ] RSM checkbox is checked for each slot you wish to activate
* [ ] Upload Name has been selected from the dropdown for each activated slot
* [ ] Data Type (Text) is confirmed and accepted for each activated slot
* [ ] All selections have been reviewed — changes cannot be made after saving
* [ ] Team members who rely on this data have been informed that custom attributes apply to future subscriptions and changes only

# FAQs

**Can I edit the Upload Name after saving?**
No. Once saved, the Upload Name is permanently frozen. If a change is required, you'll need to raise a support ticket and the engineering team will assist. Note that the display/application name shown in the RevRec UI can still be modified after saving.

**What happens if I uncheck the RSM checkbox before saving?**
The Upload Name reverts to its default value and no configuration is saved for that slot. The slot continues to function as a standard RevRec attribute with no Recurly connection.

**What happens if I check the RSM checkbox but don't select an Upload Name before saving?**
RevRec won't permit saving without a valid Upload Name selection. The Upload Name field is mandatory whenever the RSM checkbox is checked.

**What happens if a Recurly custom field mapped in RevRec is later deleted in Recurly?**
The corresponding RevRec slot will stop receiving data and will display blank values for that attribute. The slot itself remains frozen in its configured state. To remap it to a different Recurly custom field, raise a support ticket with the engineering team.

**Can I map more than five custom fields in RevRec?**
No. RevRec supports a maximum of five custom fields, corresponding to the five reserved slots F36 through F40. Prioritize the most critical fields for revenue reporting and contract analysis before configuring.

**How often is custom attribute data synced from Recurly?**
Custom attribute data is updated with every integration run between Recurly and RevRec. There's no separate or independent sync schedule for custom attributes.

**Does the custom attribute configuration apply to existing historical subscriptions?**
No. Custom attribute configuration is forward-looking only. It applies to new subscriptions created after the configuration is in place, and to future changes made to existing subscriptions. Historical records already processed in RevRec won't be retroactively updated.

**What does RevRec display if a custom field has no value for a record in Recurly?**
RevRec displays the attribute as blank for that record. This is expected behavior and doesn't indicate a configuration error or sync failure.

**What entities can custom fields be associated with in Recurly?**
Custom fields in Recurly can be associated with Account, Subscription, and Plan entities. Confirm the entity type of each field in Recurly before mapping it to a RevRec slot.

**Can I reuse a slot that was previously configured?**
No. Once a slot's RSM configuration is saved, it's permanently frozen. If the mapped Recurly field is deleted or you need a different mapping, you must raise a support ticket for engineering assistance. Slots cannot be reset or reused through the UI.

<br />
