Bank Transaction Report

[Using Power BI]
**[Problem Statement]**

Bank Transaction Reports provide easy tracking of transactions,
deposits, withdrawals, and account balances over time and help's in
Detecting Fraud Transaction in the Data with the success rate and the
failure rate. The Report Provides an Brief View of Transaction Type,
Transaction Status, Fraud Flag, Network Slice Id, Bandwidth Group with
Time. Additionally, the solution should offer advanced features such as
drill-through capabilities, conditional formatting, and tooltips to
enhance user interaction and experience. The Final report gives the
detailed view of Transaction done in a Separate section

**[Steps Followed]**

**1.Data Collection and Preparation**

Import Data from Excel sheet and examine each case type, and clean data
such us null values, empty column, empty row etc. make sure to update or
remove null values and then check the data with the help of Power Query
Editor.

**2.Dashboard Deign**

Create Calculated Columns/Measures: Depending on your needs, you may
want to create calculated columns or measures to summarize the data.

**Measures Used:**

Total Transfered = SUM(\'bank transaction_data (1)\'\[Transaction
Amount\])

Total transaction = DISTINCTCOUNT(\'bank transaction_data
(1)\'\[Transaction ID\])

**Page 1 (HOME)**

![Alt Text](https://github.com/Aswin007ben/Bank-Transaction-Data/blob/main/Screenshot%202025-03-03%20215333.png)

**Included key performance indicator (KPIs):** Displaying the Total
Transaction and the Total Transferred Details

**Line Chart:** Used the line chart to denote the Total Transaction with
Time

**Stacked Bar Chart**: The stacked bar chart represents the Total
transaction with Transaction Status which will Give the success rate and
failed rate in the both center of the bar with different colors

**Donut Chart:** The Donut Charts is used twice to represent Fraud flag
with Total Transferred and also Transaction Type and Total Transferred
to get easy view of fraud flag and the Transaction Type

**Slicer:** Several slicers has been used to get an easy view of the
report

**Map:** Map is used to display the region to locate the device used

**  
**

**PAGE 2 (Fraud Detection)**

![Alt Text](https://github.com/Aswin007ben/Bank-Transaction-Data/blob/main/Screenshot%202025-03-03%20215347.png)
In the page2(Fraud detection) all the value has been changed to Fraud
Flage to detect the number of fraud Transaction has been done in the
over all region and Device used and the Fraud count will be displayed in
the Kpi's

**Page 3(Detailed View)**

![Alt Text](https://github.com/Aswin007ben/Bank-Transaction-Data/blob/main/Screenshot%202025-03-03%20215402.png)
Created a detailed table showcasing the count of fraud detected and the
transaction failed are indicated in the green and red. This displays a
table view of the data from the dashboard where easy page navigation has
been setup in the Home page (page 1)

Utilized filters for Network slicer, Device Type, Transaction Type and
status

**Conclusion:**

Advanced features such as drill-through, conditional formatting, and
tooltips enhance user interactivity and make the report more intuitive.
With the ability to share and refresh the report automatically,
stakeholders can rely on up-to-date, real-time data to make informed
transaction decisions. This Power BI solution effectively streamlines
transaction reporting and provides actionable insights, improving
overall financial tracking and decision-making.
