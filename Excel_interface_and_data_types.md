1. Excel Interface
Understanding the Excel interface is the first step to working efficiently with data.
1.1 Workbook
A workbook is an Excel file.
It can contain one or more worksheets.
Common file extensions:
.xlsx – standard Excel workbook
.xls – older Excel format
1.2 Worksheet
A worksheet is a single sheet inside a workbook.
It consists of rows and columns arranged in a grid.
Each worksheet has a unique name (Sheet1, Sheet2, etc.).
Worksheets can be added, renamed, moved, or deleted.
1.3 Rows
Rows run horizontally across the worksheet.
Identified by numbers: 1, 2, 3, and so on.
Each row usually represents one record or entry.
1.4 Columns
Columns run vertically down the worksheet.
Identified by letters: A, B, C … Z, AA, AB, etc.
Each column represents a field or attribute.
1.5 Cell
A cell is the intersection of a row and a column.
Cell address format: Column Letter + Row Number.
Example: A1, B5, C10.
A cell can store text, numbers, dates, or formulas.
1.6 Active Cell
The currently selected cell.
Highlighted with a bold border.
Any data typed will be entered into this cell.
1.7 Name Box
Displays the address of the active cell.
Can be used to jump directly to a specific cell by typing its address.
1.8 Formula Bar
Shows the contents of the active cell.
Used to enter or edit data and formulas.
Formulas always start with an equals sign (=).
1.9 Ribbon
The ribbon is the main toolbar at the top of Excel.
It is divided into tabs containing related commands.
Common tabs include:
Home – formatting and basic editing
Insert – charts, tables, images
Formulas – functions and calculations
Data – sorting, filtering, data tools
Review – comments, spelling
View – display and layout options
1.10 Quick Access Toolbar
Located at the top-left corner.
Contains frequently used commands like Save, Undo, and Redo.
Can be customized.
1.11 Status Bar
Located at the bottom of the Excel window.
Displays information such as:
Ready or Edit mode
Sum, Average, Count of selected cells
Zoom level
1.12 Scroll Bars
Vertical and horizontal scroll bars.
Used to navigate large worksheets.
1.13 Sheet Tabs
Located at the bottom of the workbook.
Used to switch between worksheets.
2. Data Types in Excel
Data types define how Excel stores, displays, and processes data.
2.1 Text (String)
Used for names, labels, and descriptions.
Text values are not used in calculations.
Example:
Name
Product A
India
Text is left-aligned by default.
2.2 Number
Used for calculations.
Includes integers, decimals, and negative numbers.
Example:
100
45.75
-20
Numbers are right-aligned by default.
2.3 Date
Excel stores dates as serial numbers.
Each date represents the number of days since 1 January 1900.
Used for time-based analysis.
Example:
01-01-2025
15/08/2024
2.4 Time
Stored as a fraction of a day.
Used to calculate time differences and durations.
Example:
10:30 AM
18:45
2.5 Date and Time
Combination of both date and time values.
Stored as a single numeric value.
Example:
15-01-2025 10:30 AM
2.6 Currency
Represents monetary values.
Includes currency symbols such as ₹, $, €, £.
Still treated as numbers for calculations.
Example:
₹15,000
$500
2.7 Percentage
Stored internally as a decimal.
Displayed with a percentage symbol.
Example:
0.25 displayed as 25%
85%
2.8 Boolean (Logical)
Represents logical values.
Possible values:
TRUE
FALSE
Commonly used in conditional formulas.
2.9 Formula
A formula is an expression that performs calculations.
Always starts with an equals sign (=).
Example:
=SUM(A1:A10)
=A1*B1
=IF(A1>50,"Pass","Fail")
2.10 Error Values
Excel displays error values when a formula cannot be evaluated.
Common errors include:
#DIV/0! – division by zero
#VALUE! – incorrect data type
#REF! – invalid cell reference
#NAME? – incorrect function or name
#N/A – value not available
3. Importance of Data Types in Data Analytics
Ensures accurate calculations
Helps with proper sorting and filtering
Improves chart accuracy
Prevents data errors during analysis
