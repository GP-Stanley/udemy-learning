- [Team-Managed vs Company-Managed Projects](#team-managed-vs-company-managed-projects)
  - [Team-Managed Projects](#team-managed-projects)
  - [Company-Managed Projects](#company-managed-projects)
    - [Recap](#recap)
- [Creating a Team-Managed Project](#creating-a-team-managed-project)
  - [1. Accessing Project Creation](#1-accessing-project-creation)
  - [2. Choosing a Project Template](#2-choosing-a-project-template)
  - [3. Selecting a Template](#3-selecting-a-template)
  - [4. Creating the Project](#4-creating-the-project)
- [Navigating Team-Managed Projects](#navigating-team-managed-projects)
  - [Key Areas of the Agile Board](#key-areas-of-the-agile-board)
    - [1. Creating Issues](#1-creating-issues)
    - [2. Moving Issues](#2-moving-issues)
    - [3. Filtering Issues](#3-filtering-issues)
    - [4. Grouping Issues](#4-grouping-issues)
    - [5. Assigning Issues](#5-assigning-issues)
  - [Example Workflow:](#example-workflow)
- [Creating Issues in Team-Managed Projects](#creating-issues-in-team-managed-projects)
  - [Key Differences](#key-differences)
    - [More Fields](#more-fields)
    - [Create Another](#create-another)
  - [Customising Fields](#customising-fields)
    - [Configure Fields](#configure-fields)
  - [Assigning Issues](#assigning-issues)
    - [Assign to Users](#assign-to-users)
  - [Grouping Issues](#grouping-issues)
    - [Group by Assignee](#group-by-assignee)
- [Customising Team-Managed Projects](#customising-team-managed-projects)
  - [Adding and Customising Issue Types](#adding-and-customising-issue-types)
    - [Add a New Issue Type](#add-a-new-issue-type)
    - [Create Custom Issue Types](#create-custom-issue-types)
  - [Project Settings](#project-settings)
  - [Example Workflow](#example-workflow-1)


# Team-Managed vs Company-Managed Projects

## Team-Managed Projects
* Introduced in 2018 as next-gen projects, renamed in 2021.
* **Doesn't require JIRA administrative** **permissions** to **create**.
* **Entities** (e.g., issue types) live entirely **inside the project**.
* **Fast** and **easy** to **set up** and **maintain**.
* **Any team member can create and maintain the project**.

## Company-Managed Projects
* Previously called Classic Projects, renamed in 2021.
* **Require** JIRA administrative **permissions to create**.
* **Entities** (e.g., issue types, statuses, resolutions) can be **shared across multiple projects**.
* More **complicated** to **set up** and **maintain**.
* **Created** and **maintained** by **JIRA admins**.

### Recap
* `Team-Managed Projects` have **project scope entities** and are **easy to set up**.
* `Company-Managed Projects` have **global entities** and **require admin permissions**.

<br>

# Creating a Team-Managed Project

## 1. Accessing Project Creation
   * Go to Projects and select "Create Project".

## 2. Choosing a Project Template
   * Select a template based on your team's workflow (e.g., Kanban, Scrum, or a list of Issue types like Tasks and Bugs).
   * Note that some templates may be locked based on your JIRA license.

## 3. Selecting a Template
   * For example, choose the Kanban template.
   * This template includes Issue types like Epic, Story, Bug, Tasks, and Subtasks.
   * It provides a simple workflow with columns: To Do, In Progress, and Done.

## 4. Creating the Project
   * Choose Team-Managed Project.
   * Name the project (e.g., Website 2.0) and assign a key (e.g., WEB).
   * The key will be used for all Issues in the project (e.g., WEB-1, WEB-2).
   * Click "Create" to finalise the project.

> Once created, a Team-Managed Project cannot be switched to a Company-Managed Project and vice versa.

<br>

# Navigating Team-Managed Projects
When you create a Team-Managed Project in JIRA, you'll be taken to the project's Agile Board. 

Here's how to navigate and use it:

## Key Areas of the Agile Board

### 1. Creating Issues
* Click to create a new issue (e.g., "Build flow chart for website functionality").
* Each issue will have a project key (e.g., WEB-1, WEB-2).

### 2. Moving Issues
* Drag issues from left to right across columns as work progresses.
* Customise columns (e.g., add a QA column) to fit your workflow.

### 3. Filtering Issues
* Use filters at the top to show specific issues (e.g., issues related to the flow chart).
* Filter issues by assignee to see only the issues assigned to you.

### 4. Grouping Issues
* Group issues by assignee or subtasks to create swim lanes.
* This helps organise and view issues more effectively.

### 5. Assigning Issues
* Assign issues to team members to ensure work is distributed.
* Unassigned issues can be filtered and assigned as needed.

<br>

## Example Workflow:
**Create an Issue**
* Example: "Build flow chart for website functionality."
* Assign it to yourself or a team member.

**Move the Issue**
* Drag the issue from "To Do" to "In Progress" and then to "Done" as work is completed.

**Customise Columns**
* Add a new column for QA if needed.
* Drag the column to the desired position.

**Filter and Group Issues**
* Use filters to show specific issues.
* Group issues by assignee or subtasks for better organisation.

<br>

# Creating Issues in Team-Managed Projects
There are a couple of ways to create Issues in Team-Managed Projects:
1. Creating Issues on the Board.
   * Click on the Board and type the Issue (e.g., "UX plan for web app").
   * Press "Enter" to create the Issue.

2. Using the Create Button or Shortcut.
   * Create Button
     * Click the "Create" button at the top.
     * Fill out the fields in the pop-up window.
   * Keyboard Shortcut
     * Press the C key to open the Create Issue window.
     * Fill out the fields and give the Issue a title.

<br>

## Key Differences
### More Fields
* When using the Create button or shortcut, you have more fields to fill out.
* The Summary field is required and displayed in different places inside JIRA.

### Create Another
* Check the Create another box to keep the window open for creating multiple Issues.

## Customising Fields
### Configure Fields
* Customise the fields to show only the ones you need (e.g., attachments, labels).
* This makes it faster to fill out and create Issues.

## Assigning Issues
### Assign to Users
* Click on an Issue to open the screen and assign it to a team member.
* You can see who the Issue is assigned to on the Board.

## Grouping Issues
### Group by Assignee
* Group Issues by assignee to create swim lanes.
* This helps organise and view Issues more effectively.

<br>

# Customising Team-Managed Projects
## Adding and Customising Issue Types

### Add a New Issue Type
* Go to Project Settings > Issue types.
* Add a new Issue type (e.g., Bug, Idea).
* Customise the fields for the new Issue type (e.g., add a due date or a dropdown for location).

### Create Custom Issue Types
* Create a custom Issue type (e.g., Idea with a light bulb icon).
* Customise the fields for the custom Issue type.

## Project Settings
1. **Details**
   * Change the project name, Issue key, and default assignee.
   * Set the default assignee to the project lead or a point of contact.

2. **Board Settings**
   * Add and reorganise columns on the Board.
   * Combine multiple statuses into a single column to simplify the Board view.

3. **Access**
   * Control who can see and administer the project.
   * Adjust access based on your JIRA plan and license.

4. **Notifications**
   * Customise who gets notifications when an Issue is created or updated.
   * Default settings usually work well.

5. **Features**
   * Turn features on or off (e.g., Roadmap, Code).
   * Features depend on the Project template and can be adjusted as needed.

6. **Apps**
   * Access the Atlassian marketplace to discover and add Apps.
   * This course does not use third-party Apps.

7. **Automation**
   * Set up automation rules to automatically perform actions in JIRA.
   * Similar to tools like If This Then That or Zapier.

<br>

## Example Workflow
**Create a Custom Issue Type:**
* Example: Create an "Idea" Issue type with a light bulb icon.
* Add a due date field to the "Idea" Issue type.

**Customise Board Columns:**
* Add a new column for QA.
* Combine multiple statuses into a single column to simplify the Board view.

**Set Default Assignee:**
* Assign new Issues to the project lead by default.

**Turn Features On/Off:**
* Enable or disable features like Roadmap and Code based on project needs.

<br>