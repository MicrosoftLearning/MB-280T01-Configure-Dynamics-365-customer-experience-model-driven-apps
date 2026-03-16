---
lab:
    title: 'Lab 4.2: Create forms'
---

# Lab 4.2: Create forms

## Scenario
Bellows College is an educational organization with multiple campuses and programs. Many of Bellow Colleges instructors and administrators need to attend events, and purchase items. Historically tracking these expenses has been a challenge.
Campus administration would like to modernize their expense reporting system by providing employees with a digital way to report expenses.
Throughout this course, you will build applications and perform automation to enable the Bellows College employees to manage expenses.

This lab will take approximately **20** minutes to complete.

## High-level lab steps
Upon Successful Completion of this lab, you will have completed the following:
- Customize the table form to best fit your needs.

We will work with the following components:
- Forms: This is where the user creates/updates new rows in the tables.

## Prerequisites
- Completion of Module 1 Lab 0 - Validate lab environment

## Exercise 1: Customize Views and Forms
**Objective:** In this exercise, you will customize views and forms of the custom created tables that will be used in the model-driven app.

### Task #1: Edit Expense Report Form
1. If you are not already signed in, sign in to `https://make.powerapps.com`.
2. Select the environment that you imported the Expense Report solution into at the top right if it is not already selected.
3. Using the navigation on the left, select **Solutions.**
4. Open the Expense Report solution.
5. Locate and open the Expense Report table.
6. Under the Data experiences section, select **Forms** and open the Information form with Main Form type.

**IMPORTANT:** Since by default all forms are named Information, make sure to verify that the form you select has a Form Type of Main and not something else. By default, the form has two fields: Report Name and Owner.

### Task #2: Select columns for the form
1. On the right side of the screen on the Properties panel, select the **Display Name** field, and change it to `Report Information`.
2. Select **Table columns** from the left navigation pane and add the following fields below the Owner field by dragging columns to the form or simply clicking column names:
    - Description
    - Report Purpose
    - Report Due Date
    - Report Total
3. Drag the **Status Reason** column and drop it in the form header. The header is the top right area of the form. You may need to collapse the Properties panel on the right side of the screen to see the field on the form.
4. Drag the **Last Date for Approval** column and drop it next to Status Reason in the form header.
5. Select **Owner** field. In the Properties panel, change the Label to *`Requestor`*.
6. Using the navigation on the left, select **Components.**
7. Select the 1-column section to have it added below the current section.
8. In the Properties screen, change the label to **`Expense Lines`**.
9. With the Expense Lines section still selected, locate and select the **Subgrid** component.
10. Select the **Show Related Records** check box.
11. Set the Table to **Expense Lines (Expense Report).**
12. Set the Default view to **Active Expense Lines.**
13. Select **Done.**
14. Select the **Save and publish** button at the top right and wait for the save and publish to complete.
15. Select the back button at the top left of the screen. You should now be back to the Expense Report table Forms.

### Task #3: Edit Active Expense Line Form
In this task, we will modify the form that is used to add Expense Line Items.

1. If you are not already signed in, sign in to `https://make.powerapps.com`
2. Select the environment that you imported the Expense Report solution into at the top right if it is not already selected.
3. Using the navigation on the left, select Solutions.
4. Open the Expense Report solution.
5. Locate and open the Expense Line table.
6. Under the Data experiences section, select Forms and open the Information form with Main Form type.

**IMPORTANT:** Since by default all forms are named Information, make sure to verify that the form you select has a Form Type of Main and not something else. By default, the form has two fields: Expense Title and Owner.

1. On the right side of the screen on the **Properties** panel, select the **Display Name** field, and change it to `Item Details`.
2. Select **Table columns** from the left navigation pane and add the following fields below the Owner field by dragging columns to the form or simply clicking column names:
    - Expense Type
    - Item Description
    - Expense Amount
    - Expense Report
3. Drag the **Status Reason** column and drop it in the form header. The header is the top right area of the form. You may need to collapse the Properties panel on the right side of the screen to see the field on the form.
4. Select the **Save and Publish** button.
