# Sheet-1: Critic's Restaurant Ranking

## Overview

This README explains how to use the VLOOKUP function in Excel to fill in data from one table (the first table) into another table (the second table) based on matching values. The first table contains a list of restaurants with their respective cuisines and visit dates, while the second table is populated using VLOOKUP to fetch the corresponding details from the first table.

### Dataset

![image](https://github.com/user-attachments/assets/b2266013-6ae9-4d39-8267-b6bff9fd0cef)

This contains the reference data with columns for Restaurants, Cuisine, and Visit Date.


**Second Table (Updated with VLOOKUP): This table is populated by retrieving data from the first table based on the restaurant names**

![image](https://github.com/user-attachments/assets/3f4011b1-6ea6-4705-88da-624335e2769b)

### Apply VLOOKUP to Fetch Cuisine Data:

To fill in the Cuisine column in the second table, use the VLOOKUP function to look up the restaurant name in the first table and retrieve the corresponding cuisine.


![image](https://github.com/user-attachments/assets/d9d86238-6eb4-41ce-9a6c-cf27652c3a9f)

#### Example of VLOOKUP Formula for Restaurants:

`=VLOOKUP(A2, $A$2:$C$7, 2, FALSE)`

- A2: Refers to the restaurant name in the second table.
- $A$2:$C$7: Refers to the range of the first table (restaurants, cuisine, and visit dates).
- 2: Refers to the column index for Cuisine in the first table.
- FALSE: Ensures an exact match for the restaurant name

#### Example of VLOOKUP Formula for Visit Date:

`=VLOOKUP(A2, $A$2:$C$7, 3, FALSE)`

- A2: Refers to the restaurant name in the second table.
- $A$2:$C$7: Refers to the range of the first table (restaurants, cuisine, and visit dates).
- 3: Refers to the column index for Visit Date in the first table.


