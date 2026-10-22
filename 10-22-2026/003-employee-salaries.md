# Employee Salaries

> **Topic:** Basic Select<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/salary-of-employees/problem?isFullScreen=true>

## Intuition / Approach

Approach:

1. TABLE: Employee
2. COLUMNS: name
3. ROWS: one which salary is great than 2000 and months less than 10

## My Solution

```sql
SELECT name
FROM Employee
WHERE salary > 2000 AND months < 10;
```

## Reflection

Refreshed on AND operator.
