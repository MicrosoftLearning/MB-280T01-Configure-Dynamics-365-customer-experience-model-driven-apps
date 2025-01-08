---
lab:
    title: 'Lab 4.1: Visualize data with views'
---

# Lab 4.1: Visualize data with views

## Scenario

Bellows College is an educational organization with multiple campuses and programs. Many of Bellow Colleges instructors and administrators need to attend events, and purchase items. Historically tracking these expenses has been a challenge.

Campus administration would like to modernize their expense reporting system by providing employees with a digital way to report expenses.

Throughout this course, you will build applications and perform automation to enable the Bellows College employees to manage expenses.

## High-level lab steps

As part of creating the model-driven app, you will complete the following:

Create different views for viewing expense report elements.

We will work with the following components:

Views: Views allow the user to display the existing data in the form table.

## Prerequisites

Completion of Module 1 Lab 0 - Validate lab environment

## Exercise 1: Manage views

**Objective:** In this exercise, you will create a new view that can be used later in model-driven apps.

### Task #1: Edit the different Expense Lines views

1. If you are not already, sign in to `https://make.powerapps.com`.
2. Select the environment that you imported the Expense Report solution into at the top right if it is not already selected.
3. Using the navigation on the left, select **Solutions.**
4. Open the Expense Report solution.
5. Locate and open the Expense Line table.
6. Under Data experiences, select **Views.**
7. Open the **Active Expense Lines** view.
8. Click **View Column.** Select **Expense Date, Item Description, Expense Type,** and **Expense Amount.**
9. Locate and select the **Created On** column. From the menu that appears select **Remove.**
10. Your view should have the Expense Title, Expense Date, Item Description, Expense Type and Expense Amount columns on it.
11. Select the **Save and publish** button.
12. Select the back button to return to the list of views.

Next, we will repeat that process to update the Expense Line Associated View. This is the view that will appear when you are looking at Expense Lines from a parent table such as Expense Report.

### Task #2: Update the Expense Line Associated View 

1. Locate and open the Expense Line Associated view.
2. Click **View Column.** Select **Expense Date, Item Description, Expense Type,** and **Expense Amount.**
3. Locate and select the **Created On** column. From the menu that appears select **Remove.**
4. Your view should have the Expense Title, Expense Date, Item Description, Expense Type and Expense Amount columns on it.
5. Select the **Save and publish** button.
6. Select the back button to return to the list of views.

Finally, we will repeat that process one more time to update the Quick Find Active Expense Lines View. This is the view that is used whenever a user uses the search field to look for a specific Expense Line.

### Task #3: Update the Quick Find view

1. Locate and open the Quick Find Active Expense Lines view.
2. Click **View Column.** Select  **Expense Date, Item Description, Expense Type,** and **Expense Amount.**
3. Locate and select the **Created On** column. From the menu that appears select **Remove.**
4. Your view should have the Expense Title, Expense Date, Item Description, Expense Type and Expense Amount columns on it.
5. On the right side of the screen, in the Find by section, select **Edit Find Table Columns.**
6. Add the following columns:
    - Expense Date
    - Expense Type
7. Select the **Apply** button.
8. Select the **Save and publish** button.
9. Select the back button to return to the list of views.

### Task #4: Edit the different Expense Reports views

1. If you are not already, sign in to `https://make.powerapps.com`.
2. Select the environment that you imported the Expense Report solution into at the top right if it is not already selected.
3. Using the navigation on the left, select **Solutions.**
4. Open the Expense Report solution.
5. Locate and open the Expense Report table.
6. Under Data experiences, select **Views.**
7. Open the **Active Expense Reports** view.
8. Click **View Column.** Select **Report Purpose, Report Due Date, Report Total,** and **Last Date for Approval.**
9. Locate and select the **Created On** column. From the menu that appears select **Remove.**
10. Your view should have the Report Purpose, Report Due Date, Report Total, and Last Date for Approval columns on it.
11. Select the **Save and publish** button.
12. Select the back button to return to the list of views.

Next, we will repeat that process to update the Inactive Expense Reports view.

### Task #5: Update the Inactive Expense Reports view

1. Locate and open the Inactive Expense Reports view.
2. Click **View Column.** Select **Report Purpose, Report Due Date, Report Total,** and **Last Date for Approval.**
3. Locate and select the **Created On** column. From the menu that appears select **Remove.**
4. Your view should have the Report Purpose, Report Due Date, Report Total, and Last Date for Approval columns on it.
5. Select the **Save and publish** button.
6. Select the back button to return to the list of views.

### Task #6: Update the Quick Find Active Expense Reports view 

Finally, we will repeat that process one more time to update the Quick Find Active Expense Reports View. This is the view that is used whenever a user uses the search field to look for a specific Expense Report.

1. Locate and open the Quick Find Active Expense Reports view.
2. Click **View Column.** Select **Report Purpose, Report Due Date, Report Total,** and **Last Date for Approval.**
3. Locate and select the **Created On** column. From the menu that appears select **Remove.**
4. Your view should have the Report Purpose, Report Due Date, Report Total, and Last Date for Approval columns on it.
5. On the right side of the screen, in the Find by section, select **Edit Find Table Columns.**
6. Add the Report Purpose column.
7. Select the **Apply** button.
8. Select the **Save and publish** button.
9. Select the back button to return to the list of views.

### Task #7: Create a new view called Expenses Reports Due today

1. If you are not already, sign in to `https://make.powerapps.com`.
2. Select the environment that you imported the Expense Report solution into at the top right if it is not already selected.
3. Using the navigation on the left, select **Solutions.**
4. Open the Expense Report solution.
5. Locate and open the Expense Report table.
6. Under Data experiences, select **Views.**
7. Open the Active Expense Reports view.
8. Select the **Save As** button.
9. Change the Name to *`Expense Reports Due Today`*.
10. Select the **Save** button.
11. In the Filter By section, select **Edit filters.**
12. Select the **Add button.** From the menu that appears, select **Add Row.**
13. Select the drop-down arrow in the first blank row. From the menu that appears, select the **Report Due Date** column.
14. Change the Equals field to **Today.**
15. Select the **OK** button.
16. Select the **Save and Publish** button.
