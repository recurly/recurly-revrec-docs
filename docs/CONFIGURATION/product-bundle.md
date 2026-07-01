---
title: Product bundle
excerpt: >-
  Group multiple products into a single unit in Recurly RevRec so one parent
  sales order line automatically expands into its configured child lines.
deprecated: false
hidden: false
metadata:
  robots: index
---
<div class="rp-page">
  <div class="rp-overview">Product bundles let you group several individual products into a single unit, so you can sell one item while Recurly RevRec handles the accounting behind it. Upload a sales order with a single parent identifier and the system automatically expands it into all the child lines you've configured — each with its own pricing, cost, and commission attribution. That means simpler selling on the front end and precise revenue recognition on the back end.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Not included in Starter or Pro — contact <a href="https://recurly.com/demo/contact-sales/" target="_blank">Recurly Sales</a> to upgrade</div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#definition"><span class="rp-toc-num">1</span>Definition</a>
    <a class="rp-toc-pill" href="#key-benefits"><span class="rp-toc-num">2</span>Key benefits</a>
    <a class="rp-toc-pill" href="#configure-a-product-bundle"><span class="rp-toc-num">3</span>Configure a product bundle</a>
    <a class="rp-toc-pill" href="#define-bundle-rules"><span class="rp-toc-num">4</span>Define bundle rules</a>
    <a class="rp-toc-pill" href="#how-it-works"><span class="rp-toc-num">5</span>How it works</a>
    <a class="rp-toc-pill" href="#faqs"><span class="rp-toc-num">6</span>FAQs</a>
  </div>
</div>

# Definition

<div class="rp-definition">In Recurly RevRec, a product bundle is a group of products defined by a single parent identifier. When you upload a sales order (SO) file containing that parent identifier, the system splits it into the child lines you've configured — and each child line inherits its sell price, list price, and cost price from the formulas you set in the bundle configuration.</div>

# Key benefits

<div class="rp-benefits">
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-diagram-project" aria-hidden="true"></i></div>
    <strong>Automated line-item expansion</strong>
    <span>Upload one parent SKU and let the system generate all child lines automatically — no manual line entry.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-calculator" aria-hidden="true"></i></div>
    <strong>Flexible pricing formulas</strong>
    <span>Apply percentage-based formulas for sales, list, and cost prices on each child line.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-scale-balanced" aria-hidden="true"></i></div>
    <strong>Accurate cost and commission attribution</strong>
    <span>Get precise revenue recognition, cost allocation, and commission tracking for every component.</span>
  </div>
</div>

# Configure a product bundle

Create a bundle to define the parent identifier that drives how parent lines split into child lines.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open the Product Bundle screen</h4><p>Go to the Transformation section and select Product Bundle.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/bb61372-image.png" align="center" width="40%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Create a new bundle</h4><p>Select the New icon to start a new product bundle.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Name the bundle</h4><p>Provide a unique name so you can identify it later.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Select the parent identifier</h4><p>Choose the parent identifier attribute — this drives how parent lines split into child lines.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">5</div>
    <div><h4>Toggle attribution options</h4><p>Turn on Revenue Recognition, Cost, and Commission Attribution as they apply to this bundle.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">6</div>
    <div><h4>Set the status</h4><p>Set the bundle status to active or inactive.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">7</div>
    <div><h4>Set the effective dates</h4><p>Specify the effective start and end dates for the bundle.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">8</div>
    <div><h4>Save the bundle</h4><p>Select the Save icon to store your configuration.</p></div>
  </div>
</div>

The example below shows a configured "TV Bundle."


<Image src="https://files.readme.io/ea99384-image.png" align="center" width="75%" border={true} />


<div class="rp-callout rp-callout-tip">
  <div><strong><i class="fa-solid fa-lightbulb" aria-hidden="true"></i> Tip</strong>To edit a bundle, update its fields and select Save again. To remove a bundle configuration, select the Delete icon.</div>
</div>

# Define bundle rules

Rules tell Recurly RevRec how to split a parent line into its child lines and how to price each one.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open the rule set</h4><p>Select Rule Set at the top of the page.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Add a new rule</h4><p>Select the New icon to add child-line rules.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Enter the parent identifier</h4><p>Under Parent Identifier, enter the exact value used in your SO file.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Define the pricing formulas</h4><p>For each child line, set the sales price formula, list price formula, and cost formula.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">5</div>
    <div><h4>Override quantity if needed</h4><p>Set a quantity per child line under Quantity to override the SO file's quantity.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">6</div>
    <div><h4>Save the rules</h4><p>Select Save to persist your rules.</p></div>
  </div>
</div>

For example, you might configure a TV bundle with five child lines. Each line uses percentage formulas to split the parent's total sales, list, and cost values, and quantities can be set independently of the SO file's quantity.


<Image src="https://files.readme.io/17c008d-image.png" align="center" width="75%" border={true} />


<div class="rp-callout rp-callout-tip">
  <div><strong><i class="fa-solid fa-lightbulb" aria-hidden="true"></i> Tip</strong>To edit an existing rule, update its fields and select Save. To remove a rule, select its row and select Delete.</div>
</div>

# How it works

When you upload an SO file containing the parent identifier, Recurly RevRec takes over the expansion automatically:

<ul class="rp-list">
  <li>Recurly RevRec detects the bundle from the parent identifier.</li>
  <li>It applies your configured formulas to split the parent line into child lines.</li>
  <li>Each child line inherits its calculated sell price, list price, cost, and quantity.</li>
  <li>Revenue recognition, cost allocation, and commission tracking run automatically at the child-line level.</li>
</ul>

# FAQs

<Accordion title="How do I set up and process product bundles for revenue recognition?">
  Setup and processing are handled entirely on the Product Bundle screen under Data transformation → Product bundles. Configure the bundle and its rule set as described in <a href="#configure-a-product-bundle">Configure a product bundle</a> and <a href="#define-bundle-rules">Define bundle rules</a>, then upload your SO file — Recurly RevRec handles the rest.
</Accordion>

<Accordion title="Why isn't my product bundle splitting correctly in the Revenue Workbench?">
  The most common cause is a mismatched parent identifier. For a bundle to split, the parent identifier on each contract line must exactly match the identifier defined in the bundle setup. Check for case sensitivity, extra spaces, and typos.
</Accordion>

<br />
