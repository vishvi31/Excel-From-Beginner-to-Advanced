# Day 2 - Notes

Author: Vish
Date: 2026-07-14

---

## VLOOKUP

=VLOOKUP(lookup_value, table_array, col_index_num, [range_lookup])

Example: =VLOOKUP(A2, Sheet2!A:D, 3, 0)
- Looks for A2 in Sheet2 column A
- Returns the value from column 3
- 0 means exact match

LIMITATION: Can only look RIGHT. Cannot look left!

---

## XLOOKUP (Better than VLOOKUP)

=XLOOKUP(lookup_value, lookup_array, return_array)

Example: =XLOOKUP(A2, Sheet2!A:A, Sheet2!C:C)
- Looks for A2 in Sheet2 column A
- Returns value from Sheet2 column C
- Can look LEFT or RIGHT

---

## INDEX + MATCH (Most Powerful)

=INDEX(return_column, MATCH(lookup_value, lookup_column, 0))

Example: =INDEX(Sheet2!C:C, MATCH(A2, Sheet2!A:A, 0))
- MATCH finds the ROW number of A2 in Sheet2 column A
- INDEX returns the value from that row in column C
- Works in any direction, faster than VLOOKUP

---

## VLOOKUP vs XLOOKUP vs INDEX+MATCH

| Feature | VLOOKUP | XLOOKUP | INDEX+MATCH |
|---|---|---|---|
| Direction | Right only | Any | Any |
| Speed | Slow on big data | Fast | Fastest |
| Error handling | Manual | Built-in | Manual |
| Excel version | All | 2019+ | All |

---

Built by Vish - github.com/vishvi31
