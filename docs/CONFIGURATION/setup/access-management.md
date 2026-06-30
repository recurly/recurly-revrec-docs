---
title: Access management
excerpt: >-
  Create roles, manage user access, and configure read-only or administrator
  privileges in Recurly RevRec.
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---
<div class="rp-page">
  <div class="rp-overview">Access Management controls who can see and do what inside Recurly RevRec. Create roles with tailored permissions, invite users, and set read-only or administrator access — all while keeping your revenue data secure and your team accountable. This feature is part of Recurly RevRec. <a href="https://docs.recurly.com/recurly-revrec/docs/recurly-revenue-recognition-advanced" target="_blank">Learn more</a>.</div>
  <div class="rp-plan"><i class="fa-solid fa-key" aria-hidden="true"></i> Available as part of Recurly RevRec</div>
  <div class="rp-toc">
    <a class="rp-toc-pill" href="#definition"><span class="rp-toc-num">1</span>Definition</a>
    <a class="rp-toc-pill" href="#key-benefits"><span class="rp-toc-num">2</span>Key benefits</a>
    <a class="rp-toc-pill" href="#revenue-recognition-user-management"><span class="rp-toc-num">3</span>User management</a>
    <a class="rp-toc-pill" href="#faq"><span class="rp-toc-num">4</span>FAQ</a>
  </div>
</div>

### Prerequisites

<ul class="rp-list">
  <li>Familiarity with Recurly's user interface.</li>
  <li>Understanding of the organization's hierarchy and user roles.</li>
  <li>Knowledge of the desired access levels and functionalities for each user.</li>
</ul>

### Limitations

<ul class="rp-list">
  <li>Any changes you make apply to future transactions only.</li>
  <li>User roles and access levels are predefined and can't be customized beyond the available options.</li>
  <li>Changes to user privileges may require a re-login or session refresh to take effect.</li>
  <li>Only users with administrative privileges can modify or create new roles.</li>
</ul>

# Definition

<div class="rp-definition">Recurly's Access Management streamlines user access and privileges within the platform. It ensures users have the right level of access to do their jobs while maintaining data integrity and security — from creating roles with tailored permissions to managing individual user access.</div>

# Key benefits

<div class="rp-benefits">
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-shield-halved" aria-hidden="true"></i></div>
    <strong>Enhanced security</strong>
    <span>Define user roles and access levels to protect data and prevent unauthorized modifications.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-sliders" aria-hidden="true"></i></div>
    <strong>Customizable roles</strong>
    <span>Create roles tailored to specific job functions, so users have the right tools for their tasks.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-gears" aria-hidden="true"></i></div>
    <strong>Streamlined operations</strong>
    <span>Manage and modify user access easily, without compromising security.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-eye" aria-hidden="true"></i></div>
    <strong>Clear oversight</strong>
    <span>Monitor user activities and access levels to support compliance and accountability.</span>
  </div>
  <div class="rp-benefit">
    <div class="rp-benefit-icon"><i class="fa-solid fa-user-gear" aria-hidden="true"></i></div>
    <strong>Flexibility</strong>
    <span>Provide read-only or administrative access to fit different operational needs across your organization.</span>
  </div>
</div>

# Revenue Recognition user management

## Creating roles and their specifications

Before creating any user, you need to establish roles that define their access and editing privileges within the platform. Roles determine the level of access and functionality a user has. There are two primary types of roles you can create: read-only (or access-only) and Administrator. The **Site Admin** role is the only role available by default, and it provides full access.

To create roles and manage their specific settings:

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Start a new role</h4><p>From the Recurly main menu, navigate to Admin → Roles → Create a Role.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/c995693-image.png" align="center" width="60%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Name the role</h4><p>Fill in the Role Name and Roles Description fields.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Set permissions</h4><p>Select the desired configuration in the Permissions section.</p></div>
  </div>
</div>

<ol>
  <li>In the revenue recognition settings, you can select whether the role provides read-only or admin access. This can only be set during this initial configuration, so we recommend creating two separate roles — one read-only and one admin.</li>
  <li>You can always manage a user's privileges within the revenue recognition <a href="https://docs.recurly.com/docs/access-management#providing-administrator-or-read-only-privileges-in-the-revenue-recognition-site" target="_blank">platform</a> afterward.</li>
</ol>


<Image src="https://files.readme.io/12745bb-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Save the role</h4><p>Select Create Role.</p></div>
  </div>
</div>

In the access configuration screen, the revenue recognition option lets you specify whether a user with a given role can access and edit information within the revenue recognition tool. The configuration of editing privileges or read-only access within the revenue recognition platform itself must be done from inside that platform.


<Image src="https://files.readme.io/a379b5c-image.png" align="center" width="75%" border={true} />


A read-only user has limited access and can only view data and reports within the revenue recognition platform — they can't make modifications. An Administrator user has full access and can perform administrative tasks, including managing users, configuring settings, and overseeing the overall workflow.

## Creating RevRec users and providing Recurly access

In the Recurly User Management section, you can create new users and grant them access to Recurly's revenue recognition platform. This is available during the initial configuration phase, assuming you've purchased Recurly's revenue recognition service.

To create a new user and provide access to Recurly:

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Invite the user</h4><p>From the Recurly main menu, navigate to Admin → Users → User Actions → Invite Users.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Set their access</h4><p>Fill in the user's email address, select their access level or role, then select "Send Invite."</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Wait for acceptance</h4><p>The user receives an invitation to join the platform and must accept it to participate as part of your team.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Manage their access</h4><p>Once the user accepts the invitation, you can see and manage their privileges in the Users section under the Admin menu.</p></div>
  </div>
</div>

## Providing administrator or read-only privileges in the revenue recognition site

### Creating a role within the platform

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open Recurly Revenue Recognition</h4><p>Navigate to Recurly Revenue Recognition in the platform.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Open Roles</h4><p>Go to Access Management and select Roles.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Start a new role</h4><p>Select the "+" button to create a new role.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Name the role</h4><p>Provide a name for the new role.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">5</div>
    <div><h4>Configure settings</h4><p>Configure the role settings by selecting each dropdown and choosing the desired options.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/4e5c5bc-image.png" align="center" width="60%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">6</div>
    <div><h4>Save the role</h4><p>Once you've configured the role settings, select Save to create the role with the specified configuration.</p></div>
  </div>
</div>

### Modifying a user's privileges within the platform

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open Recurly Revenue Recognition</h4><p>Navigate to Recurly Revenue Recognition in the platform.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Open Users</h4><p>Go to Access Management and select Users.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">3</div>
    <div><h4>Select the user</h4><p>Select the user from the list on the left.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">4</div>
    <div><h4>Add a role</h4><p>In the Roles section, select "+" to add a role configuration and set it to active. The roles available depend on those you've already created.</p></div>
  </div>
</div>


<Image src="https://files.readme.io/f3ff6a4-image.png" align="center" width="75%" border={true} />


<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">5</div>
    <div><h4>Save</h4><p>Select Save to update the user's privileges.</p></div>
  </div>
</div>

<div class="rp-callout rp-callout-note">
  <div><strong><i class="fa-solid fa-circle-info" aria-hidden="true"></i> Note</strong>The availability of the revenue recognition section and its corresponding permission set depends on the Revenue Recognition feature flag being enabled for your Recurly site. Enabling this feature flag activates revenue recognition functionality within the Recurly platform.</div>
</div>

### User profile

Users can view and modify their own profile.

<div class="rp-steps">
  <div class="rp-step">
    <div class="rp-step-num">1</div>
    <div><h4>Open your profile</h4><p>From within Recurly Revenue Recognition, select the dropdown menu in the upper right and choose "View profile." This takes you to the Recurly UI and the profile page.</p></div>
  </div>
  <div class="rp-step">
    <div class="rp-step-num">2</div>
    <div><h4>Update your details</h4><p>From here, you can modify your name, timezone, and job function.</p></div>
  </div>
</div>

# FAQ

<Accordion title="How is user management and access configured in Recurly RevRec?">
  User management and permissions are configured in the Administration area. See the User Management documentation for step-by-step setup and access details.
</Accordion>

<Accordion title="Can I customize user roles?">
  Yes. To customize a role, go to Access Management → Roles, adjust the role's permissions, and save.

  We recommend not changing the default settings for the Revenue Manager role.
</Accordion>

<Accordion title="How do I add a new user to RevRec?">
  Add users through the Recurly Billing platform, not directly in RevRec.

  1. Sign in to Recurly Billing and open Admin.
  2. Add the user by email.
  3. Assign a role that includes Revenue Recognition access so they can open RevRec.
</Accordion>

<br />
