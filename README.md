# Entri-Assignment-2
Data Cleaning and Transformation 

1) Handling Missing Values:									
	• Check for missing values in the 'Price' column. How would you handle products with missing price information?

Ans:Replacing Missing Numerical Values:
Used the IF and ISBLANK functions to identify missing numerical values and replace them with an appropriate value such as Mean,Median or Mode
For a Price column, Median is often a sensible choice if some prices are unusually high or low.
=IF(ISBLANK(C2),MEDIAN($C$2:$C$100),C2)
								
	•If there are products with missing categories, propose a strategy to impute or deal with these missing values effectively.

Ans:Used the IF and ISBLANK functions to identify blank cells and replace the missing values with “Unknown”.
=IF(ISBLANK(B2),"Unknown",B2)

									
3) Correcting Inconsistent Data:									
	• Identify any inconsistent text formats present in the "Product Name" column.								
	• Identify any typos present in the "Category" column.								
	• Use the find and replace function to standardize the text formats in the "Product Name" column and fix any typos or misspellings in the "Category" column.								
									
4) Removing Duplicates:									
	• Identify any duplicate rows within the dataset based on the entirety of each row, and remove them if any.								
									
5) Splitting and Merging Data:									
	• Split the "Product ID" column into two separate columns for " Manufacturing Date" and "Country Code". Remove unnecessary characters, if any.								
	• Merge the "Brand Name" and "Product Name" columns into one column named "Product Brand".								
									
6) Number Formatting:									
	• Format the data type of the "Price" column to currency format. 								
	• Format the "Manufacturing Date" column to display dates in the "DD-MM-YYYY " format. 								
									
7) Conditional Formatting:									
	• Apply data bar or color scales conditional formatting in the "Price" column.								
	• Create a custom rule for conditional formatting in the "Category" column to highlight cells where the category is "Electronics."								
									
									

