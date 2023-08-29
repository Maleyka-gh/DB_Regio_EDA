
## Exploratory Data Analysis Deutsche Bahn Cargo


### The goal is to find if there are any regularies, or trends(patterns) in a sample dataset from DB Cargo.

### Dataset

Actual DB Cargo traffic data at Bst8 level

Interpretation: Train journeys and delay minutes are essential indicators for the traffic at a service point. The train journeys show how heavily the operating point is used. The delay minutes that occur at a service point show whether there were disruptions at this service point, and if so, to what extent.

BST_NR_8: This is an internal code or number that identifies each depot. Can be used as a key for the connection with the data set "Depot register freight traffic" with the column "BST8".

PROD_DATUM: Production date. The day for which the data in the columns "Train runs" and "Delay minutes" were measured.This represents the day when the train journeys were recorded.

Zugfahrten (Train runs): Number of train runs of DB Cargo that ran on the day specified by the column "PROD_DATUM" via the operating point specified in the column "BST_NR_8".

Verspätungsminuten (Delay minutes): Total of DB Cargo's delay minutes recorded on the day specified by the column "PROD_DATUM" for the operating point specified in the column "BST_NR_8".



