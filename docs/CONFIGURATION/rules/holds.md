---
title: Holds
excerpt: >-
  Configure contract and element level holds in Recurly RevRec to pause revenue
  recognition based on specific conditions, and learn how to apply and release
  holds manually.
deprecated: false
hidden: false
metadata:
  robots: index
---
<div class="rp-page">
  <div class="rp-overview">The Holds feature in Recurly RevRec lets you pause revenue recognition based on conditions set by management. Apply a hold at the contract level to pause recognition for an entire contract, or at the element level to hold specific revenue elements independently. Once the hold condition is satisfied, revenue recognition proceeds.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Available as part of Recurly RevRec</div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#definition"><span class="rp-toc-num">1</span>Definition</a>
    <a class="rp-toc-pill" href="#configuring-holds"><span class="rp-toc-num">2</span>Configuring holds</a>
    <a class="rp-toc-pill" href="#applying-and-releasing-holds"><span class="rp-toc-num">3</span>Applying and releasing holds</a>
    <a class="rp-toc-pill" href="#applying-an-element-level-hold-manually"><span class="rp-toc-num">4</span>Applying an element-level hold manually</a>
  </div>
</div>

# Definition

<div class="rp-definition">Holds allow you to temporarily pause revenue recognition for a contract or individual revenue elements based on specific conditions. Once the defined hold condition is met — whether a specific event, date, or other management-defined criteria — revenue recognition can proceed.</div>

There are two types of holds:

<div class="rp-nav-grid">

<Cards>
  <Card title="Contract level hold">
    Applies to the entire contract. Prevents revenue recognition until the hold condition is met. Once satisfied, revenue recognition for the whole contract proceeds.
  </Card>
  <Card title="Element level hold">
    Applies to individual revenue elements within a contract. Each element can have its own hold condition. Once that condition is satisfied, recognition for that element proceeds independently.
  </Card>
</Cards>

</div>

# Configuring holds

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Navigate to Holds</h4><p>Go to Rules → Holds.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/f03f8f4-image.png" align="center" width="25%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Name the hold</h4><p>Enter a name for the hold — for example, "Delivery Hold."</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Set the level</h4><p>Under Apply on, select whether the hold applies at the Contract level or Element level.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Set the release event</h4><p>Under Release on, select the event that releases the hold. Note that this option is inactive for contract-level holds.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">5</div>
    <div><h4>Select books</h4><p>Select the books the hold configuration should apply to — either all books or specific ones.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">6</div>
    <div><h4>Set the expiry date</h4><p>Choose the date on which the hold expires and stops being applied.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">7</div>
    <div><h4>Enter days</h4><p>Enter the number of days after which the hold no longer applies.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">8</div>
    <div><h4>Set active dates</h4><p>Specify the date or period during which the hold should be active.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">9</div>
    <div><h4>Configure Release Hold</h4><p>Choose one of the following options for Release Hold.</p></div>
  </div>
</div>

<ul class="rp-list">
  <li><strong>Active:</strong> Revenue can't be scheduled and won't transfer to the general ledger, even if you attempt to release revenue manually.</li>
  <li><strong>Inactive:</strong> Revenue can be scheduled and will transfer to the general ledger when you release revenue manually.</li>
</ul>


<Image src="https://files.readme.io/d644991-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">10</div>
    <div><h4>Define criteria</h4><p>Use the Criteria section to define conditions for applying the hold to a contract or element.</p></div>
  </div>
</div>

<ul class="rp-list">
  <li><strong>Field type:</strong> Specify the field type, such as "All" or a specific field.</li>
  <li><strong>Field:</strong> Choose the field on which the hold criteria is based.</li>
  <li><strong>Operator:</strong> Select the comparison operator — for example, =, &lt;, or &gt;.</li>
  <li><strong>Value:</strong> Enter the value to compare against — for example, "Damaged" as text, or a specific number.</li>
</ul>

# Applying and releasing holds

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Create a contract-level hold</h4><p>Fill in the mandatory fields and set a criteria for the hold. For example, set criteria as "quantity equal to or greater than 5."</p></div>
  </div>
</div>


<Image src="https://files.readme.io/0eafa22-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Upload the sales order file</h4><p>Upload the sales order (SO) file that satisfies the hold criteria.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Open the contract</h4><p>Open the contract in the Revenue Workbench.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Go to the Hold tab</h4><p>Navigate to the Hold tab in the contract view.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/d0b9ff7-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">5</div>
    <div><h4>Release the hold</h4><p>Right-click on each order line that needs its hold released. A "Release Line Hold" dialog box appears — select it to release the hold on that line.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/bea81c0-image.png" align="center" width="75%" border={true} />


The released hold is reflected in the waterfall view, showing the updated revenue recognition.


<Image src="https://files.readme.io/1be3a75-image.png" align="center" width="75%" border={true} />


Element-level holds follow the same release process. If holds are configured at the element level, right-click on the element line in the Hold tab and release it the same way.


<Image src="https://files.readme.io/ab318a9-image.png" align="center" width="75%" border={true} />


# Applying an element-level hold manually

First, configure the hold at the element level:

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open Holds</h4><p>Go to the Rules section and select Hold.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Set to Element Level</h4><p>Select Element Level from the dropdown list, and set Apply on to Element Level for Line Hold.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Save</h4><p>Select the Save icon to save the configuration.</p></div>
  </div>
</div>

Then, to apply the hold manually:

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Upload the contract</h4><p>Upload a contract that doesn't satisfy the element-level hold criteria.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">5</div>
    <div><h4>Open the contract</h4><p>Go to the Revenue Workbench and open the contract.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">6</div>
    <div><h4>Go to the Hold tab</h4><p>Navigate to the Hold tab in the Revenue Workbench. No hold will be applied at this point.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">7</div>
    <div><h4>Apply the hold</h4><p>Right-click on the order line that needs the hold applied. An "Apply Line Hold" dialog box appears — select it.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/7481598-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">8</div>
    <div><h4>Choose a hold and add comments</h4><p>A second dialog box appears. Select a predefined hold from the options and add comments explaining why the hold is being applied. You can apply the hold even if the contract doesn't satisfy the configured hold criteria.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/538007b-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">9</div>
    <div><h4>Confirm and save</h4><p>Select the appropriate buttons to confirm and save the applied hold.</p></div>
  </div>
</div>

<ul class="rp-list">
  <li>In the Hold tab of the Revenue Workbench, you can see when and by whom each line hold was applied.</li>
  <li>Holds can also apply to partial revenue. For example, if 50% of a contract's revenue has been released, you can apply a hold on the remaining 50% and release it later. The same manual process above applies to partial revenue holds.</li>
</ul>

<br />
