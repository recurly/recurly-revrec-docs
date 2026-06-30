---
title: Books (ASC606 vs IFRS15)
excerpt: >-
  Configure ASC 606 and IFRS 15 books in Recurly RevRec to control revenue
  recognition treatment, including how to set up your primary and secondary
  books.  <br />
deprecated: false
hidden: false
metadata:
  robots: index
---
<div class="rp-page">
  <div class="rp-overview">Books determine how Recurly RevRec treats revenue for your transactions. Set up multiple books to apply different recognition rules side by side, and designate one as your Primary Book under either ASC 606 or IFRS 15 — whichever fits your organization's country of origin or account currency.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Available as part of Recurly RevRec</div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#definition"><span class="rp-toc-num">1</span>Definition</a>
    <a class="rp-toc-pill" href="#creating-books"><span class="rp-toc-num">2</span>Creating books</a>
  </div>
</div>

# Definition

<div class="rp-definition">In Recurly RevRec, books determine the revenue treatment for your transactions. You can establish multiple books to apply different revenue recognition rules, and choose a Primary Book — ASC 606 or IFRS 15 — based on your organization's country of origin or account currency. At least one primary book must be configured before Recurly RevRec can process revenue transactions.</div>

# Creating books

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Navigate to Books</h4><p>Go to Set Up → Books.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/69476ad-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Add a new book</h4><p>Select the "+" icon to start creating a book, then complete the fields below.</p></div>
  </div>
</div>

<ul class="rp-list">
  <li><strong>Name:</strong> Must be unique (for example, "Revenue subledger book").</li>
  <li><strong>Compliance:</strong> Choose the relevant accounting standard — ASC 606 or IFRS 15.</li>
  <li><strong>Type of transactions:</strong> Choose booking or pipeline transactions.</li>
  <li><strong>Primary:</strong> Mark this if it's your main book. Only one Primary book is allowed; unmarked books become secondary, and you can have multiple secondary books.</li>
  <li><strong>Status:</strong> Mark as Active if the book is in use. Once a book is deactivated, it can't be reactivated.</li>
  <li><strong>System controls:</strong> Choose from Allocation, forecasting, cost, and posting. Primary books must always have posting active.</li>
</ul>


<Image src="https://files.readme.io/3a64df9-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Save your book</h4><p>Once you've set up your book or books, select the Save icon.</p></div>
  </div>
</div>

After your books are established, the Revenue Workbench lets you view contracts under each book individually or collectively, and reports are tailored based on the books you've created.

<div class="rp-callout rp-callout-note">
  <div><strong><i class="fa-solid fa-circle-info" aria-hidden="true"></i> Note</strong>Secondary books exclusively use pipeline features for forecasting, resembling orders booked through opportunities rather than sales orders.</div>
</div>

<br />
