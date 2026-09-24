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

2) Correcting Inconsistent Data:									
	• Identify any inconsistent text formats present in the "Product Name" column.								
	• Identify any typos present in the "Category" column.								
	• Use the find and replace function to standardize the text formats in the "Product Name" column and fix any typos or misspellings in the "Category" column.

Ans:Inconsistent data was identified by filtering the Product Name and Category columns and checking for different spellings, capitalization, and variations of the same value. Find & Replace was then used to standardize the values.

3) Removing Duplicates:									
	• Identify any duplicate rows within the dataset based on the entirety of each row, and remove them if any.

Ans:Duplicate records were identified using Excel’s Remove Duplicates feature. Three duplicate records were found and removed to ensure each record appears only once.

4) Splitting and Merging Data:									
	• Split the "Product ID" column into two separate columns for " Manufacturing Date" and "Country Code". Remove unnecessary characters, if any.
• Merge the "Brand Name" and "Product Name" columns into one column named "Product Brand".						

Ans:”Product ID” was split into “Manufacturing Date” and “Country Code”using “Text to Columns”. 
“Brand Name” and “Product Name” were merged using the “CONCATENATE” function to create a new “Product Brand” column.	
									 
									 
5)Number Formatting:									
	• Format the data type of the "Price" column to currency format. 								
	• Format the "Manufacturing Date" column to display dates in the "DD-MM-YYYY " format.

Ans:Number Formatting-Price values were formatted as Currency ($), and Manufacturing Date values were formatted using the DD-MM-YYYY format. Since the original Product ID did not include a year, 2026 was assumed as the default year for the manufacturing dates.

							
									
6)Conditional Formatting:									
	• Apply data bar or color scales conditional formatting in the "Price" column.								
	• Create a custom rule for conditional formatting in the "Category" column to highlight cells where the category is "Electronics."

Ans:Conditional formatting was applied to the Price column using Data Bars to visually compare price values.
A new conditional formatting rule was created for the Category column to highlight cells containing “Electronics”.


									
									

