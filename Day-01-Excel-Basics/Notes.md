# Day 1 - Notes

Author: Vish
Date: 2026-07-14

---

## Cell References

Relative Reference: A1 - changes when you copy the formula
Absolute Reference: $A$1 - stays fixed when you copy
Mixed Reference: $A1 or A$1 - fixes one direction only

Example:
=A1*B1         <- relative, both change
=A1*$B$1       <- B1 is fixed (e.g. tax rate)

---

## Key Formulas

=SUM(A1:A10)           Add A1 to A10
=AVERAGE(A1:A10)       Average of A1 to A10
=MAX(A1:A10)           Highest value
=MIN(A1:A10)           Lowest value
=COUNT(A1:A10)         Count numbers
=COUNTA(A1:A10)        Count non-empty
=ROUND(A1,2)           Round to 2 decimal places
=IF(A1>=40,'Pass','Fail')   Conditional
=IFS(A1>=90,'A',A1>=75,'B',A1>=60,'C',TRUE,'F')  Multiple conditions

---

## What I Practiced

- Student Performance sheet with grades
- Employee salary with bonus calculations
- Daily expenses with category totals

---

Built by Vish - github.com/vishvi31
