## OverView

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





