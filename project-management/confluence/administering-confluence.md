- [Administering Confluence](#administering-confluence)

<br>

# Administering Confluence

# User Management Overview
Overview:
* Understand how user management works in Confluence, including adding, managing, and removing users.

## User Accounts and Product Access
* Confluence allows an **unlimited number of users**.
* **Billing is based on product access** (e.g., Confluence, JIRA), not the number of users.

### Common Use Case
* **Inactive Users**: When a user leaves the team, their account can be deactivated instead of deleted to retain their contributions without incurring additional costs.

## Accessing User Management
* Administrative Permissions are required to manage users.
* Go to `Settings > User management` to access "Atlassian Administration".

## Adding a New User
Steps:
1. Click on "Add User".
2. Select the **role** (Basic, Trusted User, Site Administrator).
3. Choose which **products** the user will have **access to** (e.g., Confluence, JIRA).
4. Send an invitation to the user's email.

## User Roles
* **Basic**: Access to selected products only.
* **Trusted User**: Can invite Basic Users to products.
* **Site Administrator**: Full control over all settings, including billing.

## User Invitation and Setup
* The user receives an **email** to set up their profile and access the selected products.
* Administrators can **see** if the **user has accepted** the invitation and **set up their account**.

## Managing Users
* Administrators can **log in as a user** to **troubleshoot issues** (the user is notified via email).
* Users can be **removed**, which retains their contributions but revokes access.

<br> 

# Working With Groups
* Organise users with groups in Confluence to **streamline permissions** and **access management**.

## Creating and Managing Groups
* Navigate to the "User Management" area in "Atlassian Administration".
* Click on "Groups" on the left side and **create a new group** (e.g., Managers).
* Add users to the group either during creation or later by clicking on the group and adding members.

## Product Access
* **Assigning Access**: Groups can be assigned product access, which **controls licensing and billing**.
  * Example: If Brad has access to Confluence but not JIRA, and the Managers group has access to JIRA, Brad will have access to both Confluence and JIRA if he is part of the Managers group.
* **Default Access Group**: New users added to Confluence are automatically added to the default access group, granting them **access to the product**.

## Practical Example
* **Sharing Pages**: Share a page with a group (e.g., Managers) to grant access to multiple users simultaneously.
* **Adjusting Access**: Control product access for groups to manage billing and ensure users have the necessary permissions.

## Monitoring Access
* **Product Access Overview**: Keep an eye on the Product Access section to monitor the number of users and manage costs.
* **Adding/Removing Access**: Add or remove groups from product access as needed to control who has access to Confluence.

## Tips
* **Managing Costs**: Turn off default access for new users to manually control who gets access and manage billing effectively.
* **Permissions Management**: Use groups to streamline permissions management, making it easier to grant or revoke access for multiple users at once.

<br>

# Controlling User Permissions in Confluence
* Customise user permissions in Confluence to allow more **flexibility** and **control** over **who can create and manage spaces**.

## Global Permissions
* Navigate to `Settings > Global Permissions`.
* Customising Permissions:
  * Example: Allowing the Managers group to create spaces.
  * **Adding Groups**: If a group is not listed, add it through the Atlassian Administration area.

## Practical Example
Managers Group:
* Add the Managers group to "Global Permissions".
* Allow the Managers group to **create spaces**.

## Additional Global Permissions
* **JIRA Service Management**: Control whether users can view content on the site without a license.
* **Anonymous Access**: Allow public documentation by enabling anonymous access across the site.
* **App Permissions**: Control what third-party apps can access and do within Confluence.

## Space Permissions
* Navigate to `Settings > Space Permissions`.
* Customising Space Permissions:
  * Assign **specific permissions** to **groups** and **individual users**.
  * Example: Allowing Brad to add, delete, and archive pages in a specific space.
* **Anonymous Access**: Grant **viewing** and **commenting permissions** to **anonymous users** for a specific space.

## Default Space Permissions
* **Setting Defaults**: Customise default permissions for new spaces to **streamline the creation process**.
  * Example: Assigning the Managers group default permissions to add, delete, archive pages, and administer the space.

## Tips
* **Review Permissions**: Regularly review both global and space permissions to ensure they align with your organisation's needs.
* **Limit Anonymous Access**: Follow Atlassian's recommendation to limit anonymous access to viewing and commenting to maintain security.

<br>

# Creating New Templates
* Using templates in Confluence to standardise page layouts and content.

## Templates vs. Blueprints
* `Templates`: **Customisable page layouts** that **users** can **create and edit**.
* `Blueprints`: **Pre-built templates** provided by Confluence, which can also be **customised**.

## Creating a New Template
Steps:
1. Go to `Settings > Global Templates and Blueprints`.
2. Click on "Add global page template".
3. Give the template a **name** (e.g., My Templates).
4. Add columns, headings, and any other formatting or content as needed.
5. **Save** the template to make it available for users.

## Using the Template
* Users can **access the new template** when creating a page by **searching for the template name**.
* Users **fill out** the **pre-defined layout** and content when creating a new page.

## Managing Templates and Blueprints
* **Disabling Blueprints**: Disable built-in blueprints across all spaces if not needed.
* **Editing Blueprints**: Customise built-in blueprints to fit organisational needs.
* **Deleting Templates**: Only custom templates can be deleted, not built-in blueprints.

### Practical Example
Creating and Using a Template:
* Create a new template called "My Templates" with a specific layout.
* User (e.g., Brad) creates a new page using the "My Templates" layout.
* Edit or delete the custom template as needed.

## Tips
* **Standardisation**: Use templates to ensure pages follow a standard layout and contain consistent information.
* **Propagation**: Changes to templates may take time to propagate to all users, especially if they are currently editing a page.

<br>

# Using JIRA and Confluence
* Integrate and use JIRA and Confluence together to **enhance project management** and **collaboration**.

## Linking JIRA and Confluence
* Cloud **subscriptions** for **Confluence** and **JIRA** are typically **linked by default**.
* **Update/Verify Link**: Verify or update the link between JIRA and Confluence in `Settings > Application Links`.
* The **URL** for linking will be **specific** to your **organisation's setup**. 
  * Contact Atlassian Support for assistance if needed.

## Creating a Page with JIRA Integration
Steps:
1. Create a new page in "Confluence".
2. Add JIRA Macro: Use the **JIRA macro** to **pull in issues from JIRA**.
3. Configure JIRA Query: Set up a **JIRA query** to **filter issues** (e.g., issue type is a bug).
4. Adjust display options to show relevant information (e.g., assignee, priority).

## Real-Time Updates
* **Automatic Updates**: The JIRA macro in Confluence will automatically update with changes from JIRA, though **not in real-time**.
* **Manual Refresh**: Refresh the Confluence page to see the latest updates from JIRA.

## Creating JIRA Issues from Confluence
Steps:
1. **Select Text**: Highlight text on a Confluence page.
2. **Create JIRA Issue**: Use the option to create a JIRA issue directly from the selected text.
3. **Configure Issue**: Choose the JIRA project and issue type, then create the issue.
4. **Automatic Linking**: The new issue will be linked and displayed on the Confluence page.

## Creating Confluence Pages from JIRA
* **Sprint Retrospectives**: After completing a Sprint in JIRA, create a retrospective page in Confluence.
* **Documentation**: Use Confluence to document what went well, what can be improved, and action items for the next Sprint.

### Practical Examples
* **JIRA Macro**: Add a JIRA macro to a Confluence page to display issues from a specific JIRA project.
* **Creating Issues**: Create JIRA issues directly from Confluence pages to streamline task management.
* **Retrospectives**: Use Confluence to document Sprint retrospectives, leveraging templates for consistency.

## Tips
* **Standardisation**: Use templates in Confluence to ensure consistent documentation for retrospectives and other recurring tasks.
* **Integration** Benefits: Leverage the integration between JIRA and Confluence to enhance collaboration and project tracking.

<br> 

# Archiving and Deleting Spaces and Pages
Overview:
* Understand the difference between archiving and deleting pages and spaces in Confluence, and how to manage them.

## Archiving Pages
Steps:
1. Go to the page you want to archive.
2. Click on the **three dots** at the top right and select "Archive".
3. **Effect**: The page will disappear from the sidebar and will not show up in search results by default.
4. **Access Archived Pages**: Archived pages can be accessed from the "Archive" section in the space.

### Restoring Archived Pages
1. Go to the "Archive" section in the space.
2. Select the page and click "Restore". The page will reappear in the sidebar and search results.

## Deleting Pages
Steps:
1. Go to the page you want to delete.
2. Click on the **three dots** at the top right and select "Delete".
3. **Effect**: The page will be moved to the Trash and will not show up in search results.

### Restoring Deleted Pages
1. Only a Space Administrator can restore deleted pages.
2. Go to `Space Settings > Manage Pages > Trash`.
3. Select the page and click "Restore". The page will reappear in the sidebar and search results.

### Permanently Deleting Pages
1. Go to `Space Settings > Manage Pages > Trash`.
2. Select the page and click "Purge". This action is irreversible.

## Archiving Spaces
Steps:
1. Go to the "Space Settings" of the space you want to archive.
2. Select "Archive space".
3. **Effect**: The space and its pages will not show up in listings or search results by default.

### Restoring Archived Spaces
1. Go to the "Space Settings" of the archived space.
2. Select "Restore space". The space and its pages will reappear in listings and search results.

### Deleting Spaces
Steps:
1. Go to the "Space Settings" of the space you want to delete.
2. Select "Delete space".
3. **Effect**: The space and its pages will be permanently deleted with no option to restore.

## Tips
* **Prefer Archiving**: Generally, it is recommended to archive pages and spaces instead of deleting them, as archived content can be easily restored.
* **Backup**: Ensure you have backups of spaces before deleting them to allow for recovery if needed.

<br>

# Exporting and Space Backups
* How to back up Confluence spaces for future restoration.

## Exporting a Space
Steps:
1. Go to the space you want to back up.
2. Select "Export space".
3. **Choose Format**: Select XML for a full export that includes comments and attachments (note: does not include blog posts).
4. Export the space and download the resulting zip file.

### Practical Example
* **Website Documentation Space**: Export the Website Documentation space as XML.
* **File Contents**: The zip file will contain attachments and other data from the space.

## Restoring a Space
Steps:
1. Go to `Settings > Import space`.
2. **Choose** the exported zip **file** and **upload** it.
3. Optionally **link** the **space** to a **JIRA project**.
4. **Import** the **space** back into Confluence.

## Common Error and Workaround
**Error**: If a space with the same key already exists, an error will occur.

**Solution**:
1. **Extract Zip File**: Extract the contents of the zip file.
2. **Edit XML Files**: Change the space key in the XML files to a unique key.
3. **Re-Zip Files**: Re-zip the files and import the space again.

### Practical Example
* **Renaming Space Key**: Change the space key from "WEB" to "WEB2" in the XML files to avoid conflicts.
* **Importing**: Import the space with the new key.

## Tips
* **Backup Regularly**: Regularly back up important spaces to ensure data can be restored if needed.
* **Check Space Keys**: Ensure space keys are unique to avoid import errors.

<br>

# Quiz

1. What’s the name of where you can invite users to Confluence?
   * Atlassian Administration.

2. Who can create new groups for Confluence?
   * Administrators.

3. What’s the benefit of archiving a space?
   * Pages don't show up in search by default. 

<br>


