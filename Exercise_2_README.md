# Exercise-1: Critic's Restaurant Ranking

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



----------------------------------------------------------------------------------------------------------------------------------------------------------

# Exercise-2: Critic's Restaurant Ranking

The first table contains a list of restaurants with their area pincodes, cuisines, and visit dates, while the second and third tables need to be populated using VLOOKUP to fetch the corresponding details from the first table.

### Dataset

![image](https://github.com/user-attachments/assets/7ebce07b-5f5b-4653-9344-ba8bde1e6f7b)

- First Table (Dataset): Contains the reference data with columns for Area Pincode, Restaurants, Cuisine, and Visit Date.
  
- Second Table: Partially filled with restaurant names, cuisines, and visit dates that need to be cross-verified or fetched from the first table.
  
![image](https://github.com/user-attachments/assets/8f8ba7c6-a26a-464d-baea-6606cdf19c94)

- Third Table: Contains area pincodes and restaurant names, which need to have their cuisines filled using VLOOKUP from the first table.
	
![image](https://github.com/user-attachments/assets/b6e8ae52-0c00-404c-a4b1-8cf44d3ba2f2)


### Apply VLOOKUP to Fetch Cuisine and Visit Date:

Use the VLOOKUP function to look up the restaurant name in the first table and retrieve the corresponding Cuisine and Visit Date.

![image](https://github.com/user-attachments/assets/2a747e60-d538-4656-99bf-896c9515166a)

#### Example of VLOOKUP Formula for Cuisine

`=VLOOKUP(A2, $B$2:$D$8, 2, FALSE)`

- A2: Refers to the restaurant name in the second table.
- $B$2:$D$8: Refers to the range of columns (Restaurant, Cuisine, Visit Date) in the first table.
- 2: Refers to the column index for Cuisine in the first table.
- FALSE: Ensures an exact match for the restaurant name.

 #### Example of VLOOKUP Formula for Visit Date:

 `=VLOOKUP(A2, $B$2:$D$8, 3, FALSE)`

- A2: Refers to the restaurant name in the second table.
- $B$2:$D$8: Refers to the range of columns (Restaurant, Cuisine, Visit Date) in the first table.
- 3: Refers to the column index for Visit Date in the first table.
  
**Once you have applied the formulas for Cuisine and Visit Date in the second table, drag the formulas down for the other rows**


### Apply VLOOKUP to Fetch Cuisine:

Use the VLOOKUP function to look up the restaurant name in the first table and retrieve the corresponding Cuisine.











