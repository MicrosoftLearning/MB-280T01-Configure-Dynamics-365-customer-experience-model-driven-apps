---
lab:
    title: 'Lab 4.3: Create a dashboard'
---

# Lab 4.3: Create a dashboard 

## Scenario
Bellows College is an educational organization with multiple campuses and programs. Many of Bellow Colleges instructors and administrators need to attend events, and purchase items. Historically tracking these expenses has been a challenge.
Campus administration would like to modernize their expense reporting system by providing employees with a digital way to report expenses.
Throughout this course, you will build applications and perform automation to enable the Bellows College employees to manage expenses.

## High-level lab steps
Upon Successful completion of this lab, you will:
- Create a new model-driven app
- Create a personal dashboard that displays Expense Report information
- Add your views and dashboards to your model-driven app

## Prerequisites
- Completion of Module 1 Lab 0 - Validate lab environment

## Exercise 1: Create a Personal Dashboard

### Task #1: Create your new model-driven app
1. If you are not already, sign in to `https://make.powerapps.com`.
2. Select the environment that you imported the Expense Report solution into at the top right if it is not already selected.
3. Using the navigation on the left, select **Solutions.**
4. Open the Expense Report solution.
5. On the command bar, select the **+ New** button.
6. From the menu that appears, go to **App > Model-driven app.**
7. Enter *`Employee Expense Management`* for Name and select **Create.**

### Task #2: Create a new view called My Active Expense Reports
1. If you are not already, sign in to `https://make.powerapps.com`.
2. Select the environment that you imported the Expense Report solution into at the top right if it is not already selected.
3. Using the navigation on the left, select **Solutions.**
4. Open the Expense Report solution.
5. Locate and open the Expense Report table.
6. Under Data experiences, select **Views.**
7. Open the **Active Expense Reports** view.
8. Select the **Save As** button.
9. Change the Name to *`My Active Expense Reports`*.
10. Select the **Save** button.
11. In the Filter By section, select **Edit filters.**
12. Select the **Add** button. From the menu that appears, select **Add Row.**
13. Select the drop-down arrow in the first blank row. From the menu that appears, select the **Owner** column.
14. Change the **Equals** field to Equals current user.
15. Select the **OK** button.
16. Select the **Save and Publish** button.

### Task #3: Add a Dashboards section to the Employee Expense Management app
1. If you are not already, sign in to https://make.powerapps.com.
2. Select the environment that you imported the Expense Report solution into at the top right if it is not already selected.
3. Using the navigation on the left, select **Solutions.**
4. Open the Expense Report solution.
5. Select **Apps.**
6. Locate the Employee Expense Management app.
7. Select the **vertical ellipses**, and from the menu that appears, select **Edit.**
8. Select the **Add Page** button.
9. Select **Dashboard.**
10. Explore the system dashboards that are available by default. When you are ready, select one of the dashboards that you would like to add to your app.
11. Select **Add.**
12. With New Group selected, change the Title to **Dashboards.**
13. Select the **Save** button.
14. Once the save is complete select the **Save and Publish** button.

### Task #4: Add a personal dashboard to the Employee Expense management app
1. If you are not already, sign in to `https://make.powerapps.com`.
2. Select the environment that you imported the Expense Report solution into at the top right if it is not already selected.
3. Using the navigation on the left, select **Solutions.**
4. Open the Expense Report solution.
5. Select **Apps.**
6. Locate the Employee Expense Management model-driven app.
7. Select the **vertical ellipses**. From the menu that appears, select **Play.**
8. Under the Dashboards group, select the system dashboard you added in Task 3.
9. Select the **New** button.
10. From the menu that appears, select **Dynamics 365 Dashboard.**
11. Choose **2-column Regular Dashboard.**
12. Select the **Create** button.
13. Change the Name of the dashboard to *`Expense Report Dashboard`*.
14. In the Upper Left section, select the **List icon.**
15. Configure the List as follows:
    - Record Type: Expense Reports
    - View: Expense Reports Due today.
16. Select the **Add** button.
17. In the Upper Right section, select the **List icon.**
18. Configure the List as follows:
    - Record Type: Expense Reports
    - View: My Active Expense Reports.
19. Select the **Add** button.
20. In the Lower Left section, select the **List icon.**
21. Configure the List as follows:
    - Record Type: Expense Lines
    - View: My Active Expense Lines.
22. Select the **Add** button.
23. In the Lower Right section, select the **List icon.**
24. Configure the List as follows:
    - Record Type: Contacts
    - View: Active Contacts.
25. Select the **Add** button.
26. Select the **Save** button in the upper left corner.
27. Once the dashboard is saved, select the **Close** button.
28. You should be taken to the Expense Report Dashboard.
29. On the Command Bar at the top, select **Set As Default.**
