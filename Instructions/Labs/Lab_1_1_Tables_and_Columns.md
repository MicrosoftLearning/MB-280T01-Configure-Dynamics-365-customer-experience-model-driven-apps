---
lab:
    title: 'Lab 1.1: Create and manage tables and columns'
---

# Lab 1.1: Create and manage tables and columns

## Scenario
Bellows College is an educational organization with multiple campuses and programs. Many of Bellow Colleges instructors and administrators need to attend events, and purchase items. Historically tracking these expenses has been a challenge.
Campus administration would like to modernize their expense reporting system by providing employees with a digital way to report expenses.
Ideally, they want their users to complete an Expense Report after each event or purchase. For each Expense Report, they want them to be able to add individual expense line items. They have already started working on this solution. The Expense Report table has been created. You have been asked to take over the project and complete it.

## High-level lab steps
Upon Successful completion of this lab, you will:
- Import a Solution into your environment that includes the Expense Report Table.
- Create Expense line-item table
- Add the necessary columns to the Expense line-item table
- Add some sample data.

## Prerequisites
- Completion of Module 1 Lab 0 - Validate lab environment

## Things to consider before you begin
- Naming conventions - enter names carefully.

## Exercise 1: Import the Expense Report solution into your environment
**Objective:** In this exercise, you will import the Expense Report solution that includes the Expense Report table.

### Task #1: Import the solution
The Expense Report table will contain information about the expense report that the individual is submitting.
1. If you are not already signed in, sign into `make.powerapps.com` using your environment credentials.
2. From the Environment menu in the top right, ensure you are in the environment that you want to import the solution to.
3. Using the navigation on the left, select **Solutions.**
4. On the command bar at the top select **Import Solution.**
5. Select the **Browse** button.
6. Locate and select the `ExpenseReport_1_0_0_1` solution file that was located in your course materials.
7. Select the **Import** button.

*Note: it can take several minutes for the solution to be imported into your environment.*

## Exercise 2: Create tables and columns
**Objective:** In this exercise, you will import the Expense Report solution that includes the Expense Report table.

### Task #1: Create Expense Line table
1. If necessary, navigate to the Power Apps Maker Portal.
2. Make sure that you are working in the environment that you imported the `ExpenseReport_1_0_0_1` solution into during the last exercise.
3. Using the navigation on the left, select **Solutions.**
4. Locate and select the Expense Report solution.
5. Select the **New** button.
6. From the menu that appears, go to **Table.** Next, select **Table (advanced properties).**
7. Configure your new table as follows:
   - Display name: `Expense Line`
   - Plural name: `Expense Lines`
   - Enable attachments (Including notes and files): Selected
8. Select the Primary Column tab and change the Display Name to Expense Title.
9. Select the Save button.

*Note: It might take a minute or two for the table to be created.*

### Task #2: Add the necessary columns to the Expense Line table
1. With the Expense Line table open, select Columns under the Schema group.
2. Select **+ New column.**
3. Enter **`Expense Type`** for Display name.
4. Select **Choice > Choice** for Data type.
5. In Required, select **Optional.**
6. Set Sync with global Choice to **Yes (recommended)**.
7. Under the Sync this choice with field, select **+ New Choice.**
8. In the Display Name field, enter *`Expense Type`*.
9. In the Label field for the first choice, enter *`Meals`*.
10. Select **+ New Choice.**
11. In the Label field, enter *`Lodging`*.
12. Repeat Steps 10 & 11 to add the following options:
    - `Travel`
    - `Entertainment`
    - `Supplies / Equipment`
    - `Other`
13. Select the **Save** button.
14. In Sync this choice with field, select the **Expense Type** choice you just created.
15. Set the Default choice field to **None.**
16. Select **Save.**

### Task 3: Create Expense Amount column
1. Select + New column.
2. Enter `Expense Amount` for Display name.
3. Select Currency for Data type.
4. Select Save.

### Task 4: Create Item Description column
1. Select **+ New column.**
2. Enter *`Item Description`* for Display name.
3. Select **Multiple Lines of text > Plain Text** for Data type.
4. Select **Save.**

### Task 5: Create Expense Date column
1. Select **+ New column.**
2. Enter *`Expense Date`* for the Display Name.
3. Select **Date Only** from the Date and Time group in the Data Type Field.
4. Expand **Advanced options.**
5. Set the Time Zone adjustment field to **User Local.**
6. Select **Save.**

### Task 6: Create Expense Report column
1. Select **+ New column.**
2. Enter *`Expense Report`* for the Display Name.
3. Select **Lookup** from the Lookup group in the Data Type Field.
4. In the Related table field, select **Expense Report.**
5. Select **Save.**

## Exercise 3: Edit table
**Objective:** In this exercise, you will manually modify a table.

### Task #1: Modify the columns displayed
1. If necessary, navigate to the Power Apps Maker Portal.
2. Make sure that you are working in the environment that you imported the **ExpenseReport_1_0_0_1** solution into during the last exercise.
3. Using the navigation on the left, select **Solutions.**
4. Locate and select the **Expense Report** solution.
5. Using the navigation on the left, select **Tables.**
6. Open the Expense Line table created in the previous exercise.
7. Next to the Import Sequence column, select **+[X] more**. (The number shown here will depend on your browser size.)
8. From the menu that appears, select the following columns:
   - Expense Amount (Base)
   - Expense Date (If not already selected)
   - Expense Report
   - Expense Type
   - Expense Amount
   - Item Description
9. Select the **Save** button.
10. Locate the **Created By** column and select it.
11. From the menu that appears, select **Hide.**
12. Repeat steps 10 & 11 to remove the following columns:
    - Created By
    - Expense Line
    - Import Sequence
