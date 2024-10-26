
In this Project I perform the data cleaning operations and create a Dashboard on the Excel.

STEPS-

Create a working sheet-

	Working Sheet are created because we don’t perform data cleaning operations on the main data set that’s why we create a copy of that data set into the working sheet.
	
Remove Duplicates-

	Firstly we remove the duplicate rows in the Table.
	26 Duplicate values are Found.

Replace the Data-

	In this data "Married Status" Column Married and Single are denoted with 'M' & 'S' we find and replace that with the 'M' = "Married" & 'S' = "Single" using Find and Replace Function.
	Same for "Gender" Column Replace 'M' = "Male" & 'F' = "Female".
	
Categorize the Age Column-

	In the "Age" Column there are age number present but we need to categorize that data for simple understanding and For visualization for that we do
	New Column name as "Age Brackets" and write a conditions
		IF Age < 31 then "Adolescent"
		IF Age >= 31 then "Middle Age"
		IF Age > 54 then "Old"
	For that we use a Nested IF statement 
		=IF(L2>54,"Old",IF(L2>=31,"Middle Age",IF(L2<31,"Adolescent","Invalid")))
		
Pivot Table-

	1. Table for those Male and Female Average income where they Purchased Bike or Not.                                                                                                                                                                 
	Create a Chart Average Income Per Purchase.
	
	2.  Table for Commute Distance where Bike purchased count and Bike purchased or not.
	 Create a Chart Customer Commute.
		
	3. Table for Based on Age how many Bikes are purchased or Not Purchased.
	Customer Bike Purchased Based on Age Bracket.
	
Create a Dashboard-

	Copy all the charts from the Pivot Table and past it into the Dashboard Table.
	Use Slicer for more Specific data. Eg. Only data for Single People.
