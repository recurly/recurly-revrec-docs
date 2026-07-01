---
title: Variable considerations
excerpt: >-
  Configure variable consideration (VC) templates and rules in Recurly RevRec,
  upload transaction data, and understand how VC estimates apply automatically
  to transaction lines.
deprecated: false
hidden: false
metadata:
  robots: index
---
<div class="rp-page">
  <div class="rp-overview">Variable considerations (VC) are charges associated with discounts, rebates, refunds, credits, price concessions, incentives, performance bonuses, penalties, and similar items — amounts determined by factors unrelated to the cost of producing goods or services. In Recurly RevRec, you set up VC templates once, and the system automatically applies VC estimates to transaction lines based on the rules you define.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Available as part of Recurly RevRec</div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#configuring-variable-considerations"><span class="rp-toc-num">1</span>Configuring variable considerations</a>
    <a class="rp-toc-pill" href="#uploading-files-to-vc"><span class="rp-toc-num">2</span>Uploading files to VC</a>
    <a class="rp-toc-pill" href="#key-details"><span class="rp-toc-num">3</span>Key details</a>
  </div>
</div>

# Configuring variable considerations

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Navigate to Variable Considerations</h4><p>Go to Rules → Variable Considerations.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Start a new VC template</h4><p>Select the "+" button to create a new VC template.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Name the template</h4><p>Enter a name for the VC template.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Specify the VC type</h4><p>Set the VC type, which groups VCs of similar kinds — for example, favorable VC.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">5</div>
    <div><h4>Configure ERP accounts</h4><p>Make sure the VC-related accounts in your ERP system are accurately reflected.</p></div>
  </div>
</div>

<ul class="rp-list">
  <li><strong>Accrual Account:</strong> A liability account used for VC accrual.</li>
  <li><strong>Contra Account:</strong> A revenue account for VC revenue.</li>
  <li><strong>Clearing Account:</strong> A clearing account associated with VC.</li>
</ul>


<Image src="https://files.readme.io/05b4de3-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">6</div>
    <div><h4>Define accrual timing</h4><p>Define the timing for VC accrual.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">7</div>
    <div><h4>Set active dates</h4><p>Enter the active dates for the VC.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">8</div>
    <div><h4>Manage VC status</h4><p>Toggle the status to Inactive to inactivate a VC, or to Active to reactivate one you need.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">9</div>
    <div><h4>Add VC rules</h4><p>Select the "+" button in the Rules section to assign VC rates or amounts to apply to items. You can provide active dates for each VC rule's items. To remove VC rules or items, delete them.</p></div>
  </div>
</div>

Below is an example of a completed VC template:


<Image src="https://files.readme.io/bd5875c-image.png" align="center" width="75%" border={true} />


# Uploading files to VC

There are two ways to import data for Variable Considerations:

<div class="rp-nav-grid">

<Cards>
  <Card title="Integrate invoices from Recurly">
    If VC applies, integrate invoices directly from the Recurly platform into Recurly RevRec.
  </Card>
  <Card title="Load a sales order file">
    Load a sales order file for which VC is applicable into the system.
  </Card>
</Cards>

</div>

Once data is collected and available in the system, Recurly RevRec automatically calculates VC based on your configured rules. The calculated VC amounts are visible in the system as shown below.


<Image src="https://files.readme.io/8f2de29-image.png" align="center" width="75%" border={true} />


# Key details

## VC in the Revenue Workbench

VC estimates are automatically applied to transactions based on the VC rules defined during setup. You can also manually modify VC in the Revenue Workbench — right-click the item you want to change in the VC tab to see the available adjustment options.


<Image src="https://files.readme.io/d52f106-image.png" align="center" width="75%" border={true} />


Any changes to variable consideration are reflected in the Revenue Workbench. Adjustments or updates can be made through VC true-up or by initiating clearance to release the updated information.

<ul class="rp-list">
  <li>The transaction price in the Revenue Workbench reflects the price after variable consideration adjustments.</li>
  <li>Revenue to date in the Revenue Workbench is the cumulative sum of revenue, allocations, and favorable variable considerations scheduled for the respective period.</li>
  <li>The Revenue Workbench provides visibility into the waterfall analysis for variable consideration, showing the breakdown and impact on revenue recognition.</li>
  <li>VC Accrual represents either the amount calculated by the system or the liability that will be cleared once actuals are incorporated into the process.</li>
</ul>

<br />
