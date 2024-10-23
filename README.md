## Employee Data OverView 

### Sheet-1

This dataset contains information about employees, including their first name, last name, the company they work for, and their years of experience. The file showcases the original dataset and uses a VLOOKUP function to retrieve specific employee details in a second section.

## Structure

### Main Table (Original DataFirst Name	Last Name	Company	Experience

![image](https://github.com/user-attachments/assets/760488bb-c69e-4547-b20c-c96f34ce66a3)
):

This table contains the full list of employees and their details, including their first name, last name, company, and years of experience.

### Filtered Table (VLOOKUP Results):
		

![image](https://github.com/user-attachments/assets/0840809b-ceb5-4017-8c39-497e786524a9)

	
This section uses the VLOOKUP function to retrieve specific rows of data from the main table, based on the first names of certain employees.

## Instructions

**VLOOKUP Formula Used:**

For each row in the second table, the VLOOKUP function searches for the corresponding data from the first table using the first name as the lookup value. The formula is applied as follows:

`=VLOOKUP(A2, OriginalTableRange, ColumnIndex, FALSE)`


## Use Cases

**Data Retrieval:** Quickly retrieve employee details from a larger dataset using VLOOKUP.
**Dynamic Data Management:** Automatically update employee information in the second table when the original data changes.
**Reporting:** Filter and present specific employee details for reporting or analysis.



# Sheet-2 Overview
This dataset is part of a multi-sheet workbook where Sheet 2 contains raw data for employees and projects, and subsequent tables are populated using VLOOKUP to retrieve specific data points. The dataset includes information such as employee IDs, their performance across multiple terms, and the projects they are assigned to.

## Structure 

#### 1. Main Table (Raw Data)
The primary table includes detailed data for each individual. Each row contains an individual's information, including their name, ID, performance in three terms (Term1, Term2, Term3), and the project they are currently working on.


![image](https://github.com/user-attachments/assets/5ce8a839-e4f4-4eac-8d86-a0cdbebe355d)

#### 2. Filtered Table Using VLOOKUP (Name-Based Retrieval)
This table retrieves specific rows from the raw data using VLOOKUP. The function is applied to retrieve data based on the employee's name, and the corresponding values for their ID, Term3 performance, and project assignment are returned.

![image](https://github.com/user-attachments/assets/4207abc4-d6de-4b93-a242-71716d6c55c8)

#### 3. Filtered Table Using VLOOKUP (ID-Based Retrieval)

This table retrieves specific rows from the raw data using VLOOKUP based on the employee's ID. The corresponding values for their Term3 performance and project assignment are then returned.

![image](https://github.com/user-attachments/assets/709594a6-218f-4717-a712-03d55a204c7d)


## Instructions

**VLOOKUP Formula Explanation:**

In both the name-based and ID-based tables, the VLOOKUP function has been used to automatically retrieve data from the raw data table. Here's how the formula is structured:

`=VLOOKUP(lookup_value, table_array, col_index_num, [range_lookup])`

 -lookup_value: This is the value used to search for corresponding data (e.g., name or ID).

-table_array: This represents the range of the main data table (e.g., A2:F8 for the raw data).

**col_index_num:** The column index number of the data you want to retrieve (e.g., 2 for "Id", 6 for "Project").

**range_lookup:** A Boolean value (FALSE ensures an exact match).

**Application of VLOOKUP:**

In the **Name-Based Table**, the employee's name is used as the lookup_value.

In the **ID-Based Table**, the employee's ID is used as the lookup_value.

### Potential Use Cases

**Employee Performance Tracking:** Track employee performance across multiple terms and retrieve data dynamically.

**Project Assignment Overview:** Quickly filter and retrieve project assignments for specific employees or IDs.

**Dynamic Data Retrieval:** When new data is added to the main table, the results in the VLOOKUP tables will update automatically without manual entry.


