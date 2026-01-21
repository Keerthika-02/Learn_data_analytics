
## 1. Basic Math & Calculation Functions

### SUM  
Adds up a group of numbers.  
**Syntax**: `=SUM(number1, number2, ...)  or  =SUM(A1:A10)`  
**Example**: `=SUM(B2:B10)` → adds all values from B2 to B10  
**Useful for**: Total sales, total expenses, total marks, etc.

### AVERAGE  
Finds the average (mean) of numbers.  
**Syntax**: `=AVERAGE(range)`  
**Example**: `=AVERAGE(C2:C20)` → average score of 19 students  
**Useful for**: Average salary, average marks, average monthly sales.

### MIN / MAX  
Finds the smallest or largest value in a range.  
**Syntax**: `=MIN(range)`  or  `=MAX(range)`  
**Example**: `=MAX(D2:D100)` → highest salary in the list  
**Useful for**: Finding top scorer, lowest price, maximum temperature.

### ROUND / ROUNDUP / ROUNDDOWN  
Controls how many decimal places a number shows.  
**Syntax**: `=ROUND(number, num_digits)`  
**Example**: `=ROUND(123.45678, 2)` → 123.46  
**ROUNDUP** always rounds up, **ROUNDDOWN** always rounds down.  
**Useful for**: Money calculations, formatting reports.

## 2. Logical Functions (Making Decisions)

### IF  
Checks a condition and returns one value if true, another if false.  
**Syntax**: `=IF(condition, value_if_true, value_if_false)`  
**Example**: `=IF(A2>=60, "Pass", "Fail")`  
→ If marks ≥ 60 → "Pass", otherwise "Fail"  
**Useful for**: Grading students, categorizing sales (High/Low), bonus calculation.

### AND / OR  
Helps combine multiple conditions.  
**Syntax**: `=AND(condition1, condition2, ...)`  
**Example**: `=IF(AND(A2>=80, B2="Yes"), "Excellent", "Normal")`  
→ Only if marks ≥ 80 **and** attendance is "Yes" → "Excellent"  
**OR** returns TRUE if any condition is true.

### IFS  
Like multiple IFs in one function (cleaner).  
**Syntax**: `=IFS(condition1, value1, condition2, value2, ..., TRUE, default)`  
**Example**: `=IFS(A2>=90,"A+", A2>=80,"A", A2>=70,"B", TRUE,"C")`

### IFERROR  
Hides error messages (like #DIV/0!) and shows something nice instead.  
**Syntax**: `=IFERROR(value, value_if_error)`  
**Example**: `=IFERROR(A1/B1, "Cannot divide by zero")`

## 3. Text Functions (Working with Words)

### CONCAT / & (Join Text)  
Joins pieces of text together.  
**Syntax**: `=CONCAT(A1, " ", B1)`  or  `=A1 & " " & B1`  
**Example**: `=A2 & " " & B2` → "Keerthika Selvam"

### TEXTJOIN  
Joins text with a separator and can ignore empty cells.  
**Syntax**: `=TEXTJOIN(", ", TRUE, A2:A10)`  
**Example**: Joins names with commas → "Apple, Banana, Cherry"

### LEFT / RIGHT / MID  
Extracts part of the text.  
**Syntax**: `=LEFT(text, number_of_characters)`  
**Example**: `=LEFT("Hello World", 5)` → "Hello"  
`=RIGHT("2025-12-31", 4)` → "2031"  
`=MID("Excel is fun", 7, 3)` → "is "

### TRIM  
Removes extra spaces from text.  
**Example**: `=TRIM("   Hello   World   ")` → "Hello World"

### UPPER / LOWER / PROPER  
Changes text case.  
**PROPER** makes first letter of each word capital → "Hello World"

## 4. Lookup Functions (Finding Information)

### XLOOKUP (Modern & Best – Excel 365/2021+)  
The best way to look up values today.  
**Syntax**: `=XLOOKUP(what_to_find, where_to_look, what_to_return, [if_not_found])`  
**Example**: `=XLOOKUP("Apple", A2:A100, B2:B100, "Not found")`  
→ Finds price of "Apple"

### VLOOKUP (Classic – Still widely used)  
Looks up vertically in a table.  
**Syntax**: `=VLOOKUP(what_to_find, table, column_number, FALSE)`  
**Example**: `=VLOOKUP("P001", A2:D100, 3, FALSE)` → gets price from 3rd column

### INDEX + MATCH (Most Powerful Combo)  
More flexible than VLOOKUP.  
**Syntax**: `=INDEX(return_range, MATCH(what_to_find, lookup_range, 0))`  
**Example**: `=INDEX(B2:B100, MATCH("Apple", A2:A100, 0))`

## 5. Date & Time Functions

### TODAY / NOW  
Shows current date or date+time.  
**Example**: `=TODAY()` → 21-Jan-2026  
`=NOW()` → 21-Jan-2026 17:45

### DAY / MONTH / YEAR  
Extracts day, month, or year from a date.  
**Example**: `=YEAR(TODAY())` → 2026

### EOMONTH  
Gives the last day of the month.  
**Example**: `=EOMONTH(TODAY(), 0)` → 31-Jan-2026

### NETWORKDAYS  
Counts working days between two dates (excludes weekends).  
**Example**: `=NETWORKDAYS(A1, B1)` → number of working days

## 6. Modern Dynamic Array Functions (Excel 365 / 2021+)

### FILTER  
Shows only rows that meet a condition.  
**Example**: `=FILTER(A2:C100, B2:B100>5000)` → all sales > 5000

### UNIQUE  
Gives only unique values (no duplicates).  
**Example**: `=UNIQUE(A2:A100)` → list of unique customer names

### SORT  
Automatically sorts a range.  
**Example**: `=SORT(B2:B100)` → sorted list

## 7. Counting Functions

### COUNT / COUNTA / COUNTBLANK  
- `COUNT` → counts numbers only  
- `COUNTA` → counts all non-empty cells  
- `COUNTBLANK` → counts empty cells

### COUNTIF / COUNTIFS  
Counts cells that match a condition (or multiple conditions).  
**Example**: `=COUNTIF(A2:A100, "Apple")` → how many times "Apple" appears

## Quick Learning Tips

- Press **F4** while writing a formula → adds $ signs (locks cell reference)  
- **Alt + =** → AutoSum instantly  
- Use **Ctrl + Shift + Enter** only for old-style array formulas (not needed in modern Excel)  
- Start practicing with small data first!
