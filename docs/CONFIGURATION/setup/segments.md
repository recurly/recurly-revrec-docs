---
title: Segments
excerpt: >-
  Define your accounting structure in Recurly RevRec using Segments, and use the
  Segment mapper to link segment values to contract attributes or static codes.
deprecated: false
hidden: false
metadata:
  robots: index
---
<div class="rp-page">
  <div class="rp-overview">Segments help define your company's accounting structure, typically based on your reporting needs or business processes. Set them up once, then use the Segment mapper to control how each segment gets its value — pulled from a contract attribute or assigned as a fixed code.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Available as part of Recurly RevRec</div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#defining-segments"><span class="rp-toc-num">1</span>Defining segments</a>
  </div>
</div>

# Defining segments

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Navigate to setup</h4><p>Go to Setup.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Select Segment</h4><p>Choose "Segment" from the setup menu.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Add your segments</h4><p>Select "+" to add new segments and mark the natural segment containing the account.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/3c26ee3-image.png" align="center" width="75%" border={true} />


### Segment mapper

The Segment mapper lets you assign a value to each defined segment — either by linking it to a contract attribute or assigning a static value. For example, segments like Company and Revenue Code might pull from contract attribute values, while others, like Cost Center, use a fixed code. The segment account pulls the account number from its respective contract.
