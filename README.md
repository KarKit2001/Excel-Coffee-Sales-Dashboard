
# Excel Coffee Sales Dashboard

This Excel project offers an interactive sales dashboard for filtering, exploring, and visualizing data with slicers, timelines, and charts. It’s ideal for analysts and managers to track performance and gain actionable insights.


## XLOOKUP
To retrieve Customer Name, Email, and Country based on Customer ID, XLOOKUP was utilized. Missing values in the Email field were replaced with blank spaces instead of zeros to ensure data consistency.

## INDEX MATCH
INDEX MATCH was applied to dynamically pull product information—such as Coffee Type, Roast Type, Size, and Unit Price—using the Product ID. The MATCH function identified the row and column positions, enabling INDEX to fetch the required details efficiently

## Multiplication
Sales values were derived by multiplying Unit Price with Quantity Sold. This formula was extended across all rows to calculate the total sales for each transaction with minimal manual effort.

## Multiple IF functions
Abbreviations in the dataset were expanded using multiple IF functions. Coffee Type abbreviations ("ROB", "EXE", "ARA", and "LIB") were mapped to their full names like "Robusta", "Excelsa", "Arabica", and "Liberica"." Similarly, Roast Type codes ("M", "L", and "D") were converted into their complete forms, such as "Medium", "Light", and "Dark".

## Date Formatting
Date Formatting was applied to the Order Date column to display dates in a more standardized and user-friendly format. The format was customized to show the day, month abbreviation (e.g., "Sep"), and year (e.g., "2019"), transforming dates like "05/09/2019" into "05-Sep-2019".

## Check For Duplicates
The dataset was reviewed for duplicate entries using the "Remove Duplicates" function.

## Convert Range to Table
The raw dataset was structured into a formal table format using the "Convert Range to Table" option.

## Pivot Tables and Pivot Charts + Formatting
The "Pivot Tables and Pivot Charts" function was used to analyze sales trends. A pivot table was created from the "Orders Table," grouping order dates by year and month, and displaying coffee types and sales. Formatting included removing decimals and adding number formatting.

## Updating the Pivot Table Data Source

The Pivot Table data source was updated by converting the "Orders" range to a table for easy refresh. A "Loyalty Card" column was added, and XLOOKUP was used to auto-populate values based on customer IDs.

After refreshing the Pivot Table, a slicer for "Loyalty Card" was added and styled for clarity.

For the "Sales by Country" bar chart, the pivot sheet was duplicated, unnecessary fields removed, countries sorted by sales, and the chart customized with color and data labels.

The "Top Five Customers" chart was created, filtered by top sales, and the dashboard was completed with slicers, a timeline, and visualizations.

## Building the Dashboard
The final dashboard was assembled by integrating charts, slicers, and timelines from various sheets. Slicers and timelines were linked to all visuals for consistent filtering. Elements were arranged cleanly, and the Excel interface was adjusted to create a polished and user-friendly presentation.
