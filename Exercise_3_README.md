# Employee Data

This README explains how to use the VLOOKUP function in Excel to merge employee data from two tables into a third table. The first table contains employee IDs, names, and cities, while the second table contains employee IDs, designations, departments, and performance data. The goal is to use VLOOKUP to combine the information from both tables into the third table.

## Tables:

- First Table: Contains columns for EmpId, Name, and City.
 
![image](https://github.com/user-attachments/assets/914a488e-cba0-4c98-acbb-71b198f97be1)

- Second Table: Contains columns for EmpId, Designation, Department, and Performance.
  
![image](https://github.com/user-attachments/assets/bf08ff3a-37b0-43dc-a605-45a26092a440)

- Third Table: This is the merged table where data from both the first and second tables are combined based on EmpId.
				
![image](https://github.com/user-attachments/assets/4678619e-9dbf-4421-8745-ed0868f9d92d)


### Using VLOOKUP to Merge Data

**Example of VLOOKUP Formula for Name:**

`=VLOOKUP(A2, $A$2:$C$8, 2, FALSE)`
- A2: Refers to the EmpId in the third table.
- $A$2:$C$8: Refers to the range of EmpId, Name, and City columns in the first table.
- 2: Refers to the column index for the Name.
- FALSE: Ensures an exact match of the EmpId.

**Example of VLOOKUP Formula for Performance:**

`=VLOOKUP(A2, $A$2:$D$8, 4, FALSE)`

- A2: Refers to the EmpId in the third table.
- $A$2:$D$8: Refers to the range of EmpId, Designation, Department, and Performance columns in the second table.
- 4: Refers to the column index for Performance.
- FALSE: Ensures an exact match of the EmpId.

**Example of VLOOKUP Formula for City:**

`=VLOOKUP(A2, $A$2:$C$8, 3, FALSE)`

-A2: Refers to the EmpId in the third table.
-$A$2:$C$8: Refers to the range of EmpId, Name, and City columns in the first table.
-3: Refers to the column index for City.
-FALSE: Ensures an exact match of the EmpId.

**Example of VLOOKUP Formula for Department:**

`=VLOOKUP(A2, $A$2:$D$8, 3, FALSE)`

- A2: Refers to the EmpId in the third table.
- $A$2:$D$8: Refers to the range of EmpId, Designation, Department, and Performance columns in the second table.
- 3: Refers to the column index for Department.
- FALSE: Ensures an exact match of the EmpId.

 **Example of VLOOKUP Formula for Designation:**

 `=VLOOKUP(A2, $A$2:$D$8, 2, FALSE)`

 - A2: Refers to the EmpId in the third table.
- $A$2:$D$8: Refers to the range of EmpId, Designation, Department, and Performance columns in the second table.
- 2: Refers to the column index for Designation.
- FALSE: Ensures an exact match of the EmpId.

### Final updated table using Vlookups


![image](https://github.com/user-attachments/assets/d5bd2591-4f85-4195-8a61-486a345677f6)


## Important Notes:
Absolute References: Always use absolute references (e.g., $A$2:$D$8) for the table ranges in the VLOOKUP formulas so that the range remains fixed when you drag the formula down.
Exact Match: Ensure that the last argument in the VLOOKUP formula is FALSE to search for an exact match of the EmpId.












