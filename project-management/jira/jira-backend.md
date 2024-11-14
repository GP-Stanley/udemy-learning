- [User management in JIRA](#user-management-in-jira)
  - [Understanding Users in JIRA](#understanding-users-in-jira)
  - [Managing Users](#managing-users)
  - [Site Access](#site-access)
  - [Product Access](#product-access)
  - [Adding a New User](#adding-a-new-user)
  - [Inviting a User](#inviting-a-user)
  - [Organising Users with Groups](#organising-users-with-groups)
    - [Recap](#recap)
- [Company-Managed Project Administration Overview](#company-managed-project-administration-overview)
  - [Accessing Project Settings](#accessing-project-settings)
  - [Project Details](#project-details)
  - [People Management](#people-management)
  - [Automation](#automation)
  - [Features](#features)
  - [Issue Types](#issue-types)
  - [Workflow](#workflow)
  - [Screens](#screens)
  - [Fields](#fields)
  - [Components](#components)
  - [Opsgenie Integration](#opsgenie-integration)
  - [Permissions](#permissions)
  - [Issue Security](#issue-security)
  - [Notifications](#notifications)
  - [Development Tools](#development-tools)
  - [Issue Collectors](#issue-collectors)
  - [Slack Integration](#slack-integration)
  - [Recap](#recap-1)
- [Understanding Workflows](#understanding-workflows)
  - [What is a Workflow?](#what-is-a-workflow)
    - [Statuses and Transitions](#statuses-and-transitions)
    - [Accessing Workflows](#accessing-workflows)
    - [Default Behavior](#default-behavior)
    - [Customising Workflows](#customising-workflows)
    - [Publishing Workflows](#publishing-workflows)
    - [Benefits of Company-Managed Projects](#benefits-of-company-managed-projects)
    - [Practical Example](#practical-example)
- [Understanding How Schemes Work (1)](#understanding-how-schemes-work-1)
  - [What are Schemes?](#what-are-schemes)
  - [Applying Workflows to Different Projects](#applying-workflows-to-different-projects)
    - [Process](#process)
  - [Benefits of Schemes](#benefits-of-schemes)
  - [Types of Schemes](#types-of-schemes)
    - [Practical Example](#practical-example-1)
  - [Recommendations](#recommendations)
- [Creating a New Issue type](#creating-a-new-issue-type)
  - [Steps to Create a Custom Issue Type](#steps-to-create-a-custom-issue-type)
    - [1. Access JIRA Administration](#1-access-jira-administration)
    - [2. Add a New Issue Type](#2-add-a-new-issue-type)
    - [3. Customise the Issue Type](#3-customise-the-issue-type)
  - [Associating the Issue Type with a Project](#associating-the-issue-type-with-a-project)
    - [1. Use a Scheme](#1-use-a-scheme)
    - [2. Edit the Scheme](#2-edit-the-scheme)
    - [3. Verify the Issue Type](#3-verify-the-issue-type)
- [Creating Custom Fields](#creating-custom-fields)
  - [Steps to Create a Custom Field](#steps-to-create-a-custom-field)
    - [1. Access JIRA Settings](#1-access-jira-settings)
    - [2. Create a New Custom Field](#2-create-a-new-custom-field)
    - [3. Field Placement](#3-field-placement)
  - [Creating and Editing Screens](#creating-and-editing-screens)
    - [1. Copy an Existing Screen](#1-copy-an-existing-screen)
    - [2. Edit the Screen](#2-edit-the-screen)
  - [Creating a Screen Scheme](#creating-a-screen-scheme)
    - [Create a New Screen Scheme](#create-a-new-screen-scheme)
  - [Associating the Screen Scheme with an Issue Type](#associating-the-screen-scheme-with-an-issue-type)
    - [Issue Type Screen Scheme](#issue-type-screen-scheme)
  - [Verifying the Custom Field](#verifying-the-custom-field)
    - [Create a New Issue](#create-a-new-issue)
- [Basics of Automation in JIRA](#basics-of-automation-in-jira)
  - [Creating an Automation Rule](#creating-an-automation-rule)
    - [1. Access Automation](#1-access-automation)
    - [2. Components of Automation](#2-components-of-automation)
      - [Example Automation](#example-automation)
  - [Setting Up the Automation](#setting-up-the-automation)
  - [Testing the Automation](#testing-the-automation)
  - [Combining Automation with Post Functions](#combining-automation-with-post-functions)
  - [Global Rules](#global-rules)
  - [Customisation](#customisation)
  - [Recap](#recap-2)
  - [Additional Details](#additional-details)
- [JIRA System Administration Overview](#jira-system-administration-overview)
- [Quiz](#quiz)


# User management in JIRA

## Understanding Users in JIRA
* Billing in JIRA is based on Users, specifically **Product access**.
* You pay for **Product access**, not just the number of Users.
* **Users without access** can still have their **past comments** and **issues** **attributed to them**.

## Managing Users
* Requires JIRA **administrative permissions**.
* Access the User management section from the top right.
* **Control Site** access and **Product access** from the left side menu.

## Site Access
* **Control** how **Users get access** to JIRA.
* **Limit access** based on **email domain** or require **admin approval for new Users**.
* **Manage access requests** to **control** **who joins** JIRA.

## Product Access
* By default, **new Users have Product access**, increasing your bill.
* Monitor and manage Product access to **control costs**.

## Adding a New User
* Invite a user by adding their **email address**.
* **Control their role** (basic, trusted, or Site administrator).
  * **Basic access**: Only what you specify.
  * **Trusted**: Can invite other Users.
  * **Site administrator**: Has all billing details.

## Inviting a User
* Send an **invitation email**.
* User follows the link to join and create an Atlassian account if needed.
* User appears in the list with Product access.

## Organising Users with Groups
* Create **groups** to **organise Users**.
* Add members to groups for easier management.
* **Shared items** with a group are **accessible to all** group members.

### Recap
* Users and Product access are different.
  * **Users**: anyone who has an account, regardless of whether they have access to any products.
  * **Products**: refers to the permissions that allow a user to access specific JIRA products
* Control Site access settings.
* Invite Users and manage their roles.
* Use groups to organise Users efficiently.

<br>

# Company-Managed Project Administration Overview

## Accessing Project Settings
* **Project Settings Location**: Found at the bottom of the left side menu within a project.
* **Administrative Permissions**: Required to access project settings. 
  * Project admin permissions differ from overall JIRA admin permissions. 
  * JIRA administrators have admin permissions over all projects, while some users may have admin permissions over individual projects only.

## Project Details
* **Project Name and Key**: Can be changed, but the key must be unique as it is tied to issue URLs. 
  * JIRA will re-index URLs if the key is changed, but old links will still work.
* **Project Lead**: The default assignee for new issues if no one is specified. 
  * Useful for ensuring issues are assigned and managed. 
  * The Project lead can be a point of contact to ensure nothing slips through the cracks and can delegate tasks to other team members.

## People Management
* **User Roles**: Control user roles at the project level. In the free plan, this feature is limited.
* **Groups**: Create groups to manage permissions and roles efficiently.
  * For example, you can create a group for managers and assign project-level administrative permissions to all members of that group.

## Automation
* **Automation Rules**: Set up rules to automate tasks (e.g., closing an Epic when all its stories are closed). 
  * Similar to tools like If This Then That (IFTTT) or Zapier. 
  * Automation can help streamline workflows and reduce manual effort.

## Features
* **Feature Toggles**: Enable or disable features like the Roadmap. 
  * Some features are tied to board settings, while others are project-wide.
  * For example, you can turn off the code link if it's not relevant to your project.

> Provides a summary of current settings, including Screens and Workflows. Customisable based on project needs.

## Issue Types
* **Customisation**: Add or remove issue types specific to the project. Control the fields displayed for each issue type.
* **Screens**: Define fields for each issue type. 
  * Screens can be shared across multiple projects, requiring overall JIRA admin permissions to modify. 
  * This allows for consistency and reuse of configurations across projects.

## Workflow
* **Statuses and Transitions**: Defines the statuses and transitions between them for issues in the project.
* **Control**: Manage how issues move through different statuses.

## Screens
* **Current Screens**: View and manage the screens used in the project.
* **Customisation**: Screens can be customised to show specific fields for different issue types.

## Fields
* **Project Fields**: View and manage the fields used in the project.
* **Screen Association**: Determine which fields appear on which screens.
* **Overall JIRA Admin**: Customisations may require overall JIRA administrative permissions as configurations can be shared across multiple projects.

## Components
* **Definition**: Components are sub-sections of a project, used to group issues.
* Example: A website project might have a payment processing component.
* **Organisation**: Helps in organising and managing issues related to specific parts of the project.

## Opsgenie Integration
* **Integration**: Control how Opsgenie, another Atlassian product, integrates with your project.

## Permissions
* **Project Permissions**: Set up and manage permissions for the project.
* **User and Group Permissions**: Control who can browse the project, manage sprints, and access other features.

## Issue Security
* **Visibility Control**: Hide certain issues from specific users.
* **Use Case**: Useful for managing sensitive issues like customer feedback that should only be visible to certain teams.

## Notifications
* **Notification Scheme**: Manage who gets notified about issue updates.
* **Default Scheme**: By default, watchers, assignees, and reporters get notifications.
* **Shared Schemes**: Notification schemes can be shared across multiple projects, requiring overall JIRA admin permissions to edit.

## Development Tools
* **Integration**: Link development tools like Bitbucket or GitHub to JIRA.

## Issue Collectors
* **Forms**: Create forms to collect issues directly from your website.
* **Automatic Issue Creation**: Forms filled out on the website automatically create issues in JIRA.
* **Customisation**: Configure fields, issue types, and other settings for the issue collector.

## Slack Integration
* **Integration**: Link JIRA issues and notifications to your team's Slack channel.

## Recap
* **Customisation**: There are many ways to customise your projects in JIRA to fit your team's needs.
* **Project-Specific**: Customisations discussed are specific to the project you are working on.
* **Future Topics**: The next video will cover Workflows in JIRA.

<br>

# Understanding Workflows

## What is a Workflow?
* A Workflow in JIRA **controls the process for issues in a project**.
* Consists of **Statuses** and **Transitions**.

### Statuses and Transitions
* **Statuses**: Represent the **current state** of an issue (e.g., To Do, In Progress, Done).
* **Transitions**: The process of **moving an issue** from **one Status to another** (e.g., from To Do to In Progress).

### Accessing Workflows
* **Navigation**: Go to `Settings > Issues > Workflows` to view active Workflows for Company-Managed Projects.

### Default Behavior
* **All Statuses Transition**: By default, JIRA allows all Statuses to transition to all other Statuses. This is expected behavior to provide flexibility.

### Customising Workflows
* **Draft State**: Editing a Workflow puts it into a draft state to **prevent disruption for active users**.
* **Adding a Status**: You can add new Statuses and allow all Statuses to transition into the new one.
* **Post Functions**: Add post functions to transitions. 
  * For example, automatically assign an issue to a specific user when it transitions to a certain Status.

### Publishing Workflows
* **Publishing Drafts**: After making changes, **publish the draft** to make the **Workflow active**.
* **Example**: Adding a new Status "Graphics" and assigning issues to Mary when they transition to this Status.

### Benefits of Company-Managed Projects
* **Shared Configurations**: Ability to share Workflows and other configurations across different projects.

### Practical Example
* **Creating a New Status**: If you add a new Status called "Graphics," you can configure it so that any issue moved to this Status is automatically assigned to a specific user, such as Mary, who is responsible for graphic design.
* **Post Function Setup**: This involves setting up a post function on the transition to the "Graphics" Status, ensuring that the issue is assigned to Mary.
* **Publishing Changes**: Once the new Status and post function are set up, publish the draft Workflow to make it active. This ensures that the changes are applied and the Workflow is updated.

<br>

# Understanding How Schemes Work (1)

## What are Schemes?
* Schemes in JIRA are used to **share configurations across** multiple Company-Managed **Projects**.
* They help in organising and managing projects by **applying consistent settings and workflows**.

## Applying Workflows to Different Projects
Example: Applying a Workflow from a sample Scrum project to a Marketing Team project.

### Process
1. Go to the `project settings` of the target project.
2. Navigate to `Workflows` and view the **current Workflow**.
3. **Switch** the Workflow Scheme to the **desired one**.
4. JIRA will **migrate issues** to the **new Workflow**, ensuring compatibility.

## Benefits of Schemes
* **Consistency**: Allows for consistent workflows and settings across multiple projects.
* **Efficiency**: Simplifies the management of multiple projects by sharing configurations.

## Types of Schemes
* **Workflow Schemes**: Control the workflows for different issue types within projects.
* **Issue Type Schemes**: Determine which issue types are available in projects.
* **Issue Type Screen Schemes**: Control the fields displayed on issues.
* **Field Configuration Schemes**: Define field requirements (e.g., required fields) for different projects.
* **Issue Security Schemes**: Manage visibility of issues for different users or groups.
* **Notification Schemes**: Customise how notifications are sent for different projects.
* **Permission Schemes**: Share permissions across multiple projects for easier management.

### Practical Example
* **Workflow Customisation**: Create a Workflow that assigns issues to a specific user when they transition to a certain status.
* **Scheme Application**: Apply the customised Workflow to multiple projects using Schemes.

## Recommendations
* **Simplify Schemes**: Avoid over-complicating Schemes to prevent user confusion.
* **Review and Clean Up**: Regularly review and clean up Schemes to ensure they are necessary and not excessive.

<br>

# Creating a New Issue type

## Steps to Create a Custom Issue Type
### 1. Access JIRA Administration
* Navigate to `Settings > Issues`.
* Select **Issue types** from the left side menu.

### 2. Add a New Issue Type
* Click on "Add Issue type".
* Enter a **name** for the new Issue type (e.g., New Feature).
* Choose the **type** of Issue type (Standard or Subtask).

### 3. Customise the Issue Type
* Optionally, add an image or icon to represent the Issue type.

## Associating the Issue Type with a Project
### 1. Use a Scheme
* After creating the **Issue type**, it needs to be **associated with a project** using a Scheme.
* Navigate to **Issue type schemes**.

### 2. Edit the Scheme
* Select the **scheme associated with the target project** (e.g., Marketing Team project).
* **Add** the new Issue type to the scheme and **save** the changes.

### 3. Verify the Issue Type
* Create a new issue in the target project to see the new Issue type listed.
* **Note**: the Issue type will not appear in other projects unless it is associated with their respective schemes.

<br>

# Creating Custom Fields

## Steps to Create a Custom Field
### 1. Access JIRA Settings
* Navigate to `Settings > Issues`.
* Select "Custom Fields" from the left-hand side menu.

### 2. Create a New Custom Field
* Click on "Create Custom Field".
* Choose the **field type** (e.g., single select list).
* **Name** the field (e.g., Feature Location).
* **Add options** for the field (e.g., website, mobile app, social, other).

### 3. Field Placement
* Decide **where** the field should **appear**. 
* Do not select any existing screens if you want it to show up only on a specific issue type.

## Creating and Editing Screens
### 1. Copy an Existing Screen
* Copy an **existing screen** (e.g., the default screen for the Marketing Team project) to use as a **starting point**.
* **Name** the new screen (e.g., New Feature Screen).

### 2. Edit the Screen
* **Add** the newly created field to the **screen**.
* **Rearrange or remove** other fields as needed.

## Creating a Screen Scheme
### Create a New Screen Scheme
* Navigate to `Screen Schemes`.
* Add a new **Screen Scheme** (e.g., New Feature Screen Scheme).
* Set the **default screen** to the one you just created.

## Associating the Screen Scheme with an Issue Type
### Issue Type Screen Scheme
* Navigate to `Issue type Screen Schemes`.
* **Edit** the scheme associated with the target project.
* **Associate** the **new Issue type** (e.g., New Feature) with the **new Screen Scheme**.

## Verifying the Custom Field
### Create a New Issue
* Create a new issue in the target project.
* Verify that the new field appears when the appropriate Issue type is selected.

Recommendations:
* **Team Collaboration**: Work with team leaders to determine necessary fields for productivity.
* **Remove Unnecessary Fields**: Eliminate fields that are not used to reduce visual clutter and improve efficiency.

<br> 

# Basics of Automation in JIRA

## Creating an Automation Rule
### 1. Access Automation
* Navigate to your **Agile board**.
* Click on "Automation" at the top right-hand side.

### 2. Components of Automation
* **Trigger**: The event that starts the automation (e.g., issue assigned).
* **Condition**: Criteria that must be met for the action to occur (e.g., assignee equals Mary).
* **Action**: The task performed when the condition is met (e.g., set priority to highest).

#### Example Automation
* **Trigger**: When an issue is assigned.
* **Condition**: Assignee equals Mary.
* **Action**: Edit the issue to set the priority to highest.

## Setting Up the Automation
1. **Select Trigger**: Choose "Issue assigned" as the trigger.
2. **Add Condition**: Set the condition to check if the assignee is Mary.
3. **Define Action**: Configure the action to edit the issue and set the priority to highest.
4. **Save and Turn On**: Save the automation rule and turn it on.

## Testing the Automation
1. **Assign Issue**: Assign an issue to Mary.
2. **Observe Priority Change**: The priority level should automatically change to highest.

## Combining Automation with Post Functions
* Post Function: Automatically assign an issue to Mary when it transitions to the Graphics status.
* Automation Layer: Add an automation rule to set the priority to highest when the issue is assigned to Mary.

## Global Rules
* Project-Level Automation: Automations specific to a single project.
* Global Rules: Automations that apply across all projects.

## Customisation
* **Triggers, Conditions, Actions**: Explore various combinations to automate different tasks.
* **Experimentation**: Play around with different automation rules to find what works best for your organisation.

## Recap
* **Automation Components**: Trigger, condition, and action.
  * Example: Automating priority changes for issues assigned to Mary.
* **Global and Project-Level Rules**: Flexibility to create rules for individual projects or across all projects.

## Additional Details
* **Automation Scope**: Automations can be created at both the project level and globally across all projects.
* **Layering Automations**: You can layer multiple automations and post functions to create complex workflows. For example, combining a post function that assigns an issue to Mary with an automation that changes the priority.
* **Exploring Triggers**: There are numerous triggers available, such as issue creation, status changes, and field updates, allowing for a wide range of automation possibilities.
* **Conditions and Actions**: Conditions can be based on various fields and criteria, and actions can include editing fields, sending notifications, and more.
* **Automation Templates**: JIRA provides templates for common automation scenarios, making it easier to get started.

<br>

# JIRA System Administration Overview

**Global Administration Area**
* **Access**: Navigate to `Settings > System` to access JIRA’s global administration area.
* **Scope**: Applies to the entire JIRA installation, not just a single project.

**Global Permissions**
* **Control**: Manage who can create Team-Managed projects and other global permissions.
  * **Example**: Restrict project creation to users in the Managers group.

**Permission and Notification Helper**
* **Purpose**: Helps troubleshoot permission and notification issues.
* **Usage**: Identify why a user cannot access an issue or is not receiving notifications.
  * **Example**: If a user like Mary cannot access an issue, the helper can diagnose if it's a permission issue or something else, like a browser extension.

**Default Dashboard**
* **Customisation**: Create a default dashboard for new users.
* **Global Impact**: This dashboard is seen by all new users upon joining the JIRA installation.
* **User Customisation**: Users can create and share their own dashboards.

**Search Functionality**
* **Admin Search**: Use the search bar or press the period key to quickly find settings and tools within the admin area.

**Project Management**
* **Control Projects**: Manage all projects within the JIRA installation.
* **Visibility**: JIRA administrators can see and manage all projects by default.

**Issue Management**
* **Settings**: Configure fields, screens, and workflows for issues.
* **Customisation**: Tailor issue settings to fit the needs of the organisation.

**Apps and Extensions**
* **Manage Apps**: Add or manage apps to extend JIRA’s functionality.
* **Default Setup**: The course uses the default JIRA setup without additional apps.

**Billing**
* **Management**: Handle billing and license management for JIRA.
* **Privacy**: Billing information is private and managed separately.

**Recommendations**
* **Customisation**: Customise JIRA settings to fit the organisation’s needs.
* **Review**: Regularly review and adjust settings to ensure optimal configuration.

<br>

# Quiz

1. What determines your subscription cost with Jira Cloud?
   * The number of users with product access.
  
2. What feature of company-managed projects lets you control the fields displayed on issues?
   * Screens.

3. What do workflows control in a project?
   * Statuses and transitions.

4. Which of these schemes controls the statuses used in a company-managed project?
   * Workflow scheme.

5. Once a new issue type is created, how do you tell Jira which project uses it?
   * Issue type schemes.

6. What do you use to add a custom field to issues?
   * Screens.

7. What are the three components of an automation rule?
   * Trigger, condition and action.

8. Where do you go to limit who can create team-managed projects?
   * Permissions.

<br>

