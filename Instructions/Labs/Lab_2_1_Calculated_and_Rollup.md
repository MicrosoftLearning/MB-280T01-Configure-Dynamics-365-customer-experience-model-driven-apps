---
lab:
    title: 'Lab 2.1: Create calculated and rollup fields'
---

# Lab 2.1: Create calculated and rollup fields 

## Scenario
Bellows College is an educational organization with multiple campuses and programs. Many of Bellow Colleges instructors and administrators need to attend events, and purchase items. Historically tracking these expenses has been a challenge.
Campus administration would like to modernize their expense reporting system by providing employees with a digital way to report expenses.
Ideally, they want their users to complete an Expense Report after each event or purchase. For each Expense Report, they want them to be able to add individual expense line items. They have already started working on this solution. The Expense Report table has been created. You have been asked to take over the project and complete it.

This lab will take approximately **20** minutes to complete.

## High-level lab steps
Upon Successful completion of this lab, you will:
- Add new fields to an existing table
- Create a rollup field
- Create a calculated field

## Prerequisites
- Completion of Module 1 Lab 0 - Validate lab environment and Lab 1.1, where you imported the Expense Report solution

## Things to consider before you begin
- Naming conventions - enter names carefully.

## Exercise 1: Create Calculated and Rollup fields
**Objective:** In this exercise, create a rollup and a calculated field on the expense report table.

### Task #1: Add a rollup field to the Expense Report table
1. Navigate to the Power Apps Maker portal `https://make.powerapps.com`
2. Make sure that you are working in the environment that you imported the Expense Report solution into during the last exercise.
3. Using the navigation on the left, select **Solutions.**
4. Locate and select the Expense Report solution.
5. Locate and open the Expense Report table.
6. Under the Schema Group, select **Columns.**
7. Select **+New column.**
8. Enter *`Report Total`* for Display name.
9. Select **Currency** for Data type.
10. In Required, select **Optional.**
11. In the Behavior field, select **Rollup.**
12. Select the **Save** and **Edit** button.
13. Once the Column is saved, a pop-up window should appear. (If you get a pop-up message, you may need to allow pop ups.)
14. Under RELATED ENTITY, select **+Add related entity.**
15. Select **(Expense Lines) Expense Report.**
16. Select the Check mark button to accept the change.
17. Under AGGREGATION, select **+Add aggregation.**
18. Set Aggregate Function to **Sum.**
19. Set Aggregated Related Entity Field to **(Expense Line) Expense Amount.**
20. Select the green check mark and then select the **Save and Close** button.

### Task #2: Add a Power FX Formula Calculated field to the Expense Report table
1. Navigate to the Power Apps Maker portal `https://make.powerapps.com`
2. Make sure that you are working in the environment that you imported the Expense Report solution into during the last exercise.
3. Using the navigation on the left, select **Solutions.**
4. Locate and select the Expense Report solution.
5. Locate and open the Expense Report table.
6. Under the Schema Group, select **Columns.**
7. Select **+New column.**
8. Enter *`Last Date for approval`* for Display name.
9. Select **Formula** for Data type.
10. Enter the following formula: `DateAdd('Report Due Date',2)`
11. Set the Format field to **Date Only.**
12. Select the **Save** button.
