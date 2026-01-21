

## 1. Math & Statistics

| Function                  | Description / Example                                      | Example Result          |
|---------------------------|------------------------------------------------------------|--------------------------|
| `=SUM(A1:A10)`            | Sum of range                                               | Total                   |
| `=AVERAGE(A1:A10)`        | Average of range                                           | Mean                    |
| `=MIN(A1:A10)`            | Smallest value                                             |                         |
| `=MAX(A1:A10)`            | Largest value                                              |                         |
| `=ROUND(number, digits)`  | Rounds to specified digits<br>`=ROUND(3.5678, 2)`          | 3.57                    |
| `=ROUNDUP()` / `=ROUNDDOWN()` | Rounds up / down                                       |                         |
| `=SUMPRODUCT(array1, array2, ...)` | Multiplies & sums arrays<br>Weighted average, etc. |                         |
| `=SUMIFS(sum_range, criteria_range1, criteria1, ...)` | Sum with multiple conditions |                         |
| `=COUNTIFS(criteria_range1, criteria1, ...)` | Count with multiple conditions |                         |
| `=AVERAGEIFS()`           | Average with multiple conditions                           |                         |

## 2. Logical Functions

| Function                  | Description / Example                                      | Example Result          |
|---------------------------|------------------------------------------------------------|--------------------------|
| `=IF(A1>=60, "Pass", "Fail")` | Simple condition                                       | Pass / Fail             |
| `=IFS(logical_test1, value_if_true1, ...)` | Multiple conditions (like switch) |                         |
| `=AND(condition1, condition2)` | All conditions true → TRUE                           |                         |
| `=OR(condition1, condition2)`  | Any condition true → TRUE                            |                         |
| `=NOT(condition)`         | Reverses TRUE/FALSE                                        |                         |
| `=IFERROR(value, value_if_error)` | Returns custom value on error<br>`=IFERROR(A1/B1, "Error")` |                         |
| `=IFNA(value, value_if_na)` | Handles only #N/A errors                                 |                         |

## 3. Lookup & Reference (Modern Excel)

| Function                  | Description / Example                                      | Notes                   |
|---------------------------|------------------------------------------------------------|--------------------------|
| `=XLOOKUP(lookup_value, lookup_array, return_array, [if_not_found], [match_mode])` | Modern, flexible lookup | Excel 365 / 2021+       |
| `=INDEX(range, MATCH(lookup_value, lookup_range, 0))` | Classic powerful combo (any direction) | Still widely used       |
| `=VLOOKUP(lookup_value, table_array, col_index, [range_lookup])` | Classic vertical lookup | Approximate match if FALSE → exact |
| `=HLOOKUP()`              | Horizontal version of VLOOKUP                              |                         |
| `=FILTER(array, include, [if_empty])` | Dynamic filter<br>`=FILTER(A2:C100, B2:B100>5000)` | Excel 365 / 2021+       |
| `=SORT(range, [sort_index], [sort_order])` | Dynamic sort                                             | Excel 365 / 2021+       |
| `=UNIQUE(range)`          | Returns only unique values                                 | Excel 365 / 2021+       |

## 4. Text Functions

| Function                  | Description / Example                                      | Example Result          |
|---------------------------|------------------------------------------------------------|--------------------------|
| `=CONCAT(A1," ",B1)` or `=A1&" "&B1` | Join text                                      | John Doe                |
| `=TEXTJOIN(delimiter, ignore_empty, text1, ...)` | Join with delimiter, skip blanks | "Apple, Banana, Cherry" |
| `=LEFT(text, num_chars)`  | First characters<br>`=LEFT("Excel",3)`                     | Exc                     |
| `=RIGHT(text, num_chars)` | Last characters                                            |                         |
| `=MID(text, start, num_chars)` | Middle characters                                    |                         |
| `=TRIM(text)`             | Remove extra spaces                                        | "Hello World"           |
| `=SUBSTITUTE(text, old_text, new_text)` | Replace text                                   |                         |
| `=UPPER()` / `=LOWER()` / `=PROPER()` | Case conversion                                  |                         |
| `=TEXT(value, format_text)` | Format numbers/dates as text<br>`=TEXT(A1,"₹#,##0.00")` | ₹1,234.56               |

## 5. Date & Time Functions

| Function                  | Description / Example                                      | Example Result          |
|---------------------------|------------------------------------------------------------|--------------------------|
| `=TODAY()`                | Current date                                               | 21-Jan-2026             |
| `=NOW()`                  | Current date & time                                        | 21-Jan-2026 17:45       |
| `=DAY(date)` / `=MONTH()` / `=YEAR()` | Extract parts of date                              | 21 / 1 / 2026           |
| `=EOMONTH(start_date, months)` | Last day of month<br>`=EOMONTH(TODAY(),0)`         | 31-Jan-2026             |
| `=DATEDIF(start_date, end_date, "unit")` | Difference (Y=years, M=months, D=days)            |                         |
| `=NETWORKDAYS(start, end, [holidays])` | Working days (excl. weekends)                        |                         |
| `=WORKDAY(start_date, days, [holidays])` | Date after X working days                            |                         |

## 6. Dynamic Array Functions (Excel 365 / 2021+)

| Function                  | Description                                                | Example Result          |
|---------------------------|------------------------------------------------------------|--------------------------|
| `=FILTER(array, include)` | Filters rows that meet condition                           | Spill range             |
| `=SORT(array)`            | Sorts range dynamically                                    | Spill range             |
| `=UNIQUE(range)`          | Returns unique values                                      | Spill range             |
| `=SEQUENCE(rows, [columns], [start], [step])` | Creates number sequence<br>`=SEQUENCE(10)` | 1 to 10                 |
| `=RANDARRAY(rows, columns)` | Random numbers between 0–1                               | Spill range             |

## 7. Financial Functions (Common)

| Function                  | Description                                                | Example                 |
|---------------------------|------------------------------------------------------------|--------------------------|
| `=PMT(rate, nper, pv)`    | Loan payment amount                                        | EMI calculation         |
| `=FV(rate, nper, pmt, [pv])` | Future value                                           |                         |
| `=PV(rate, nper, pmt)`    | Present value                                              |                         |
| `=NPER(rate, pmt, pv)`    | Number of periods                                          |                         |

## Quick Tips & Shortcuts

- **Absolute reference**: `$A$1` (F4 key to toggle)
- **AutoSum**: `Alt + =`
- **Paste values only**: `Ctrl + Alt + V` → `V`
- **Name a range**: Formulas → Name Manager
- **Array formula (legacy)**: `Ctrl + Shift + Enter` (not needed in dynamic arrays)
