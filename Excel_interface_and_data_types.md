# Excel Interface – Basics

This document explains the basic components of the Microsoft Excel interface.
Understanding these elements is essential before working with data analysis tasks.

---

## Workbook
A workbook is an Excel file that contains one or more worksheets.

- File extensions:
  - `.xlsx` – Standard Excel workbook
  - `.xls` – Older Excel format
- A single workbook can store multiple sheets of related data.

---

## Worksheet
A worksheet is a single sheet within a workbook.

- Consists of rows and columns
- Used to store and analyze data
- Worksheets can be added, renamed, moved, or deleted

---

## Rows
- Rows run horizontally across the worksheet
- Identified by numbers (1, 2, 3, ...)
- Each row usually represents one record or entry

Example:
- One row = one student / one transaction / one employee

---

## Columns
- Columns run vertically in the worksheet
- Identified by letters (A, B, C, ..., AA, AB, ...)
- Each column represents a field or attribute

Example:
- Name, Age, Salary, Date

---

## Cell
A cell is the intersection of a row and a column.

- Cell address format: Column Letter + Row Number
- Examples: A1, B3, C10
- A cell can contain:
  - Text
  - Numbers
  - Dates
  - Formulas

---

## Active Cell
- The currently selected cell
- Highlighted with a bold border
- Any data typed will appear in this cell

---

## Name Box
- Displays the address of the active cell
- Can be used to quickly jump to a specific cell
- Example: Typing `D10` and pressing Enter moves to cell D10

---

## Formula Bar
- Displays the content of the active cell
- Used to enter or edit formulas and values
- Formulas always start with an equals sign (`=`)

- Example:
- =SUM(A1:A2)

---

## Ribbon
The ribbon is the main toolbar at the top of Excel.

Common tabs include:
- **Home** – Formatting and basic editing
- **Insert** – Charts, tables, images
- **Formulas** – Functions and calculations
- **Data** – Sorting, filtering, data tools
- **Review** – Comments and spelling
- **View** – Display and layout options

---

## Quick Access Toolbar
- Located at the top-left corner
- Contains frequently used commands such as Save, Undo, and Redo
- Can be customized based on user preference

---

## Status Bar
- Located at the bottom of the Excel window
- Displays:
  - Current mode (Ready/Edit)
  - Sum, Average, Count of selected cells
  - Zoom level

---

## Scroll Bars
- Vertical and horizontal scroll bars
- Used to navigate large worksheets

---

## Sheet Tabs
- Located at the bottom of the workbook
- Used to switch between worksheets
- Sheets can be added, renamed, or reordered

---
# Data Types in Excel

This document explains the different data types supported by Microsoft Excel.
Understanding data types is essential for accurate calculations, sorting, filtering,
and data analysis.

---

## Text (String)
Text data is used for names, labels, and descriptions.

- Excel does not perform calculations on text values
- Text is left-aligned by default

Examples:
- Name
- Product A
- India

---

## Number
Number data is used for calculations.

- Includes whole numbers, decimals, and negative values
- Right-aligned by default

Examples:
- 100
- 45.75
- -20

---

## Date
Dates are stored internally as serial numbers in Excel.

- Each date represents the number of days since 1 January 1900
- Used in time-based analysis and calculations

Examples:
- 01-01-2025
- 15/08/2024

---

## Time
Time values are stored as a fraction of a day.

- Used to calculate durations and time differences

Examples:
- 10:30 AM
- 18:45

---

## Date and Time
A combination of both date and time values.

- Stored as a single numeric value
- Useful for timestamp-based analysis

Example:
- 15-01-2025 10:30 AM

---

## Currency
Currency values represent monetary data.

- Includes currency symbols such as ₹, $, €, £
- Treated as numbers for calculations

Examples:
- ₹15,000
- $500

---

## Percentage
Percentage values are stored as decimals but displayed as percentages.

- 0.25 is displayed as 25%

Examples:
- 85%
- 40%

---

## Boolean (Logical)
Logical values are used in conditional operations.

- Possible values:
  - TRUE
  - FALSE
- Commonly used in IF and logical formulas

---

## Formula
A formula performs calculations or logical operations.

- Always starts with an equals sign (`=`)
- Can reference cells, ranges, and functions

Examples:
- =SUM(A1:A10) =A1*B1 =IF(A1>50,"Pass","Fail")

---

## Error Values
Excel displays error values when formulas cannot be evaluated correctly.

Common error types:
- `#DIV/0!` – Division by zero
- `#VALUE!` – Incorrect data type
- `#REF!` – Invalid cell reference
- `#NAME?` – Invalid function or name
- `#N/A` – Value not available

---

## How to Check or Change Data Type
1. Select the required cell or range
2. Go to **Home → Number Group**
3. Choose the appropriate format:
   - General
   - Number
   - Text
   - Date
   - Currency
   - Percentage
