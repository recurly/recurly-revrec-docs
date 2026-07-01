---
title: Cost
excerpt: >-
  Configure cost types, cost rules, and cost file uploads in Recurly RevRec to
  manage manual and formula-based cost calculation for revenue recognition.
deprecated: false
hidden: false
metadata:
  robots: index
---
<div class="rp-page">
  <div class="rp-overview">Recurly RevRec lets you account for costs in two ways: load them manually via a cost file, or have the system calculate them automatically based on predefined formulas. Use the Cost section of the Rules page to define your Cost Types and Cost Rules.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Available as part of Recurly RevRec</div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#configuring-a-cost-type"><span class="rp-toc-num">1</span>Configuring a cost type</a>
    <a class="rp-toc-pill" href="#calculating-cost-using-a-cost-file"><span class="rp-toc-num">2</span>Calculating cost using a cost file</a>
  </div>
</div>

# Configuring a cost type

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Navigate to Cost</h4><p>Go to Rules and select Cost from the menu.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/f03f8f4-image.png" align="center" width="25%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Enter the cost type</h4><p>Enter the Cost Type to specify the type of cost you're defining.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Set the cost treatment</h4><p>Determine how the cost is recognized.</p></div>
  </div>
</div>

<ul class="rp-list">
  <li><strong>Point in time:</strong> Recognize the cost in the month it's incurred.</li>
  <li><strong>Follow Revenue:</strong> Recognize the cost according to the revenue recognition pattern over the contract period.</li>
</ul>

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Set cost keys (optional)</h4><p>Select the field and choose the appropriate options from the pop-up menu. Setting cost keys is optional.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">5</div>
    <div><h4>Configure formula-based calculation (optional)</h4><p>If you need Recurly RevRec to calculate the cost amount, use the "Formula on" feature. Type <code>Line.SellPrice</code> (case-sensitive) to apply cost rules based on a percentage of the sell price.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">6</div>
    <div><h4>Set account numbers</h4><p>Specify a unique account number for the debit account (Dr account number) and the credit account (Cr account number). These numbers are compared with the Sales Order number.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">7</div>
    <div><h4>Enable cost capitalization (optional)</h4><p>If your incremental cost needs to be amortized and capitalized, activate the Cost Capitalize option.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/b6ce8f1-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">8</div>
    <div><h4>Save</h4><p>Select the Save icon to save your cost configuration.</p></div>
  </div>
</div>

## Adding cost rules

To apply the cost formula to specific contract lines — for example, to an item called "Macbook" — add cost rules to your configuration:

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Add a new cost rule</h4><p>Under the Cost Rules section, select the "+" button to add a new rule.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Select the book</h4><p>Choose the book the cost should apply to, so the rule is associated with the correct book.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Specify the item</h4><p>In the Item column, enter the item name — for example, "Macbook" — to target the cost rule to contract lines for that item.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Enter the cost percentage</h4><p>In the Value column, enter the percentage of the sell price to treat as cost for the specified item.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">5</div>
    <div><h4>Save</h4><p>Select Save to save the cost rule.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/c0e7dae-image.png" align="center" width="75%" border={true} />


<div class="rp-callout rp-callout-note">
  <div><strong><i class="fa-solid fa-circle-info" aria-hidden="true"></i> Note</strong>If your cost calculation is based on an attribute other than "Item," go to the mapper and select the required fields.</div>
</div>

# Calculating cost using a cost file

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Prepare the cost file</h4><p>Prepare a cost file that includes the necessary columns reflecting the cost attributes defined in the system. Make sure the cost type in the file matches the cost type already defined in the system.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Navigate to Transactions</h4><p>Go to the Transactions page in Recurly RevRec.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Upload the cost file</h4><p>Select the Upload icon, then choose the cost file from your local system using Browse or Choose File and select the appropriate file.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/43d3a70-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Initiate the upload</h4><p>Select Open to start the upload process. The system processes the file, calculates cost based on your Cost Rules configuration, and applies the calculated cost to the respective contract lines — even if cost isn't explicitly assigned to the item or POB in the contract.</p></div>
  </div>
</div>

<br />
