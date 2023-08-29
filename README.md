
### Exploratory Data Analysis Deutsche Bahn Cargo


🎯 Objective:
To identify patterns or regularities within a sample dataset from DB Cargo.

### Dataset (Actual DB Cargo traffic data at Bst8 level)

The data provided here represent the number of train journeys and delay minutes per day
and operating point. All Bst over which at least 10 train journeys took place were taken into
account.

Interpretation: Train journeys and delay minutes are essential indicators for the traffic at a service point. The train journeys show how heavily the operating point is used. The delay minutes that occur at a service point show whether there were disruptions at this service point, and if so, to what extent.

- BST_NR_8: This internal code or number identifies each depot. It can be used as a key for the connection with the data set "Depot register freight traffic" with the column "BST8".

- PROD_DATUM: Production date. The day for which the data in the columns "Train runs" and "Delay minutes" were measured.This represents the day when the train journeys were recorded.

- Zugfahrten (Train runs): Number of train runs of DB Cargo that ran on the day specified by the column "PROD_DATUM" via the operating point specified in the column "BST_NR_8".

- Verspätungsminuten (Delay minutes): Total of DB Cargo's delay minutes recorded on the day specified by the column "PROD_DATUM" for the operating point specified in the column "BST_NR_8".


### Analysis

The table below shows the entries in the dataset where there are multiple records
for the same operating point on the same day.
For example, for the operating point with ID 80000000 on 2016-01-15,
There are two entries: one with 69 train journeys and 0 delay minutes
and another with 30 train journeys and 0 delay minutes
This means that the number of train journeys and delay minutes have been recorded at
different times during the day for the same operating point.

<div align="center">
<img src="Interactive_plots/plt0.png" alt="overview" width="400"/>
</div>













