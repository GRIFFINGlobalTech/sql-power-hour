# Higher Than 75 Marks

> **Topic:** Basic Select<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/more-than-75-marks/problem?isFullScreen=true>

## Intuition / Approach

Approach:

1. TABLE: STUDENTS
2. COLUMNS: Name
3. ROWS: one which has more than 75 marks, use WHERE clause
4. Order the results by the last three Digits using RIGHT (column_name, 3)

## My Solution

```sql
SELECT Name
FROM STUDENTS
WHERE Marks > 75
ORDER BY RIGHT(Name, 3), ID ASC;
```

## Reflection

I learned new term, RIGHT, which can use to select the no. of characters in a word/name.
