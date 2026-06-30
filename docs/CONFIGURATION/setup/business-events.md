---
title: Business events
excerpt: >-
  Configure standard and custom business events in Recurly RevRec, link them to
  POBs, and structure your event file upload template.
deprecated: false
hidden: false
metadata:
  robots: index
---
<div class="rp-page">
  <div class="rp-overview">Business events are the custom or standard triggers that drive revenue and cost actions in Recurly RevRec. Set up an event, link it to a Performance Obligation, then upload an event file — RevRec processes the events and applies the results to your revenue waterfall.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Available as part of Recurly RevRec</div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#key-details"><span class="rp-toc-num">1</span>Key details</a>
    <a class="rp-toc-pill" href="#configuring-events"><span class="rp-toc-num">2</span>Configuring events</a>
    <a class="rp-toc-pill" href="#associating-an-event-with-a-pob"><span class="rp-toc-num">3</span>Associating an event with a POB</a>
    <a class="rp-toc-pill" href="#event-file-template"><span class="rp-toc-num">4</span>Event file template</a>
  </div>
</div>

# Key details

## Standard events

Standard events are built-in business triggers in Recurly RevRec that help release a POB:

<div class="rp-nav-grid">

<Cards>
  <Card title="Upon billing">
    The event occurs upon billing for sales orders.
  </Card>
  <Card title="Upon booking">
    The event occurs upon sales order loading.
  </Card>
  <Card title="Expiration">
    The event triggers upon expiration.
  </Card>
</Cards>

</div>

## Custom events

You can also create custom events in Recurly RevRec, such as:

<div class="rp-nav-grid">

<Cards>
  <Card title="Revenue">
    Associated with a POB template to release revenue.
  </Card>
  <Card title="Holds">
    Linked to holds or approvals to release revenue, or to transfer revenue placed on a contract, POB, or line hold.
  </Card>
</Cards>

</div>

# Configuring events

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Navigate to Events</h4><p>Go to Set Up → Events.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/9648676-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Fill in event details</h4><p>Fill in the necessary fields and select options as needed.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Save</h4><p>Once you've set up the event, select the Save icon.</p></div>
  </div>
</div>

# Associating an event with a POB

Before uploading an event file to Recurly RevRec, you need to link the business event with a POB.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Add a revenue release event</h4><p>Navigate to the desired POB. Within the Revenue Release tab, select the "+" icon, then choose the event from the dropdown and specify the percentage of revenue release for it. Set this to 100 if it's the only event.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/a76fa5f-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Link additional events as needed</h4><p>You can link multiple events to a single POB, and you have the flexibility to edit or delete revenue release events.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Save</h4><p>Once you're done, select the Save icon.</p></div>
  </div>
</div>

# Event file template

Your event file template should resemble the table below:

<table class="rp-params">
  <tr class="rp-thead-row"><td>Attribute 1 (from event mapper)</td><td>Attribute 2 (from event mapper)</td><td>Event action</td><td>Start date</td><td>End date</td><td>Release date</td><td>Effective date</td><td>Expiry date</td></tr>
  <tr><td>—</td><td>—</td><td>—</td><td>—</td><td>—</td><td>—</td><td>—</td><td>—</td></tr>
</table>

## Template components

<div class="rp-card">

### Event code

Every uploaded event file must include an event code. Recurly RevRec supports the following event codes:

<table class="rp-params">
  <tr class="rp-thead-row"><td>Event type</td><td>Event action</td></tr>
  <tr><td><code>EventActionRemoveHold</code></td><td>1</td></tr>
  <tr><td><code>EventActionRecognize</code></td><td>2</td></tr>
  <tr><td><code>EventActionDefer</code></td><td>3</td></tr>
  <tr><td><code>EventActionExpiryDate</code></td><td>4</td></tr>
  <tr><td><code>EventActionDeferFuture</code></td><td>5</td></tr>
  <tr><td><code>EventActionAccelerate</code></td><td>6</td></tr>
  <tr><td><code>EventActionDeferReRecognize</code></td><td>7</td></tr>
</table>

</div>

<ul class="rp-list">
  <li><strong>Start and end date:</strong> Optional, but they determine the revenue recognition period and override any dates specified in the contract.</li>
  <li><strong>Release date:</strong> Lets you input data for the current period as if the event is scheduled for a future date. For example, you can upload an event file in May 2023 for July 2023, which helps with waterfall catchup.</li>
  <li><strong>Effective date:</strong> Governs future events. For example, if events dated July 2023 are loaded in May 2023, the system won't process them until July 2023 is active — the effective date manages this future scheduling.</li>
  <li><strong>Expiry date:</strong> Applicable for events with a set expiration, and can be used to update an event's expiration date.</li>
</ul>

<br />
