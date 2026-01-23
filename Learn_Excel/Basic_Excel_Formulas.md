# Basic Excel Formulas Cheat Sheet

| Category          | Formula                  | Description / Example                                                                                 | Example Result |
|-------------------|--------------------------|-------------------------------------------------------------------------------------------------------|----------------|
| **Basic Math**    | `=A1+B1`                 | Addition                                                                                              | Sum of two cells |
|                   | `=A1-B1`                 | Subtraction                                                                                           | Difference |
|                   | `=A1*B1`                 | Multiplication                                                                                        | Product |
|                   | `=A1/B1`                 | Division                                                                                              | Quotient |
|                   | `=A1^B1`                 | Exponent (power) – A1 raised to the power of B1                                                       | e.g., 2^3 = 8 |
| **Rounding**      | `=ROUND(number, num_digits)` | Rounds to specified number of decimals<br>→ `=ROUND(3.5678,2)` → 3.57                             | 3.57 |
|                   | `=ROUNDUP(number, num_digits)` | Rounds up                                                                                       | `=ROUNDUP(3.14159,2)` → 3.15 |
|                   | `=ROUNDDOWN(number, num_digits)` | Rounds down                                                                                   | `=ROUNDDOWN(3.99,0)` → 3 |
| **Text**          | `=CONCAT(A1," ",B1)` <br>or `=A1&" "&B1` | Joins text/strings<br>→ "John" + " " + "Doe" → "John Doe"                                 | John Doe |
|                   | `=LEFT(text, num_chars)` | Extracts characters from the left<br>→ `=LEFT("Excel",3)` → "Exc"                                 | Exc |
|                   | `=RIGHT(text, num_chars)`| Extracts characters from the right<br>→ `=RIGHT("2024-12-31",4)` → "2031"                         | 2031 |
|                   | `=MID(text, start_num, num_chars)` | Extracts from the middle<br>→ `=MID("Hello World",7,5)` → "World"                           | World |
|                   | `=TRIM(text)`            | Removes extra spaces<br>→ `=TRIM("  Hello   World  ")` → "Hello World"                            | Hello World |
|                   | `=UPPER(text)`           | Converts to UPPERCASE                                                                                 | HELLO WORLD |
|                   | `=LOWER(text)`           | Converts to lowercase                                                                                 | hello world |
|                   | `=PROPER(text)`          | Capitalizes first letter of each word                                                                 | Hello World |
| **Lookup / Reference** | `=VLOOKUP(lookup_value, table_array, col_index_num, [range_lookup])` | Vertical lookup<br>→ `=VLOOKUP("Apple",A2:B10,2,FALSE)` | Price of Apple |
|                   | `=HLOOKUP(lookup_value, table_array, row_index_num, [range_lookup])` | Horizontal lookup                                          | |
| **Logical**       | `=IF(logical_test, value_if_true, value_if_false)` | Conditional logic<br>→ `=IF(A1>=60,"Pass","Fail")`                                       | Pass / Fail |
|                   | `=AND(condition1, condition2, ...)` | Returns TRUE if ALL conditions are true                                                     | |
|                   | `=OR(condition1, condition2, ...)` | Returns TRUE if ANY condition is true                                                        | |
|                   | `=NOT(condition)`        | Reverses logic (TRUE → FALSE, FALSE → TRUE)                                                           | |
| **Count & Sum**   | `=SUM(range)`            | Adds up a range of numbers<br>→ `=SUM(A1:A10)`                                                        | Total |
|                   | `=AVERAGE(range)`        | Calculates average<br>→ `=AVERAGE(B2:B20)`                                                            | Average |
|                   | `=COUNT(range)`          | Counts cells that contain numbers                                                                     | |
|                   | `=COUNTA(range)`         | Counts all non-empty cells                                                                            | |
|                   | `=COUNTBLANK(range)`     | Counts empty cells                                                                                    | |
|                   | `=MIN(range)`            | Finds the smallest value                                                                              | |
|                   | `=MAX(range)`            | Finds the largest value                                                                               | |
| **Date & Time**   | `=TODAY()`               | Returns current date                                                                                  | 21-Jan-2026 |
|                   | `=NOW()`                 | Returns current date **and** time                                                                     | 21-Jan-2026 17:30 |
|                   | `=DAY(date)`             | Extracts day number from date                                                                         | 21 |
|                   | `=MONTH(date)`           | Extracts month number                                                                                 | 1 |
|                   | `=YEAR(date)`            | Extracts year                                                                                         | 2026 |
|                   | `=DATEDIF(start_date, end_date, "unit")` | Difference between dates<br>→ `"Y" = years, "M" = months, "D" = days` | |

### Quick Tips
- **Absolute reference**: Use `$` to lock rows/columns  
  → `=A1*$B$1` (B1 stays fixed when dragging formula)
- **Toggle between relative & absolute**: Press **F4** while editing formula
- **AutoSum**: Select cells → **Alt + =** (shortcut)
- **Paste values only**: Copy → Paste Special → Values (or Ctrl+Alt+V → V)
