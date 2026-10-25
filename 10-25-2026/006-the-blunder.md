# The Blunder

> **Topic:** Aggregation<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/the-blunder/problem?isFullScreen=true>

## Intuition / Approach

Approach:

1. TABLE: EMPLOYEES
2. COLUMNS: Salary
3. CEIL & REPLACE: replace characters and get the next integer

## My Solution

```sql
SELECT CEIL(AVG(Salary) - AVG(REPLACE(Salary, '0', '')))
FROM EMPLOYEES;
```

## Reflection

I learned how to get the next integer with CEIL and replace characters with REPLACE function.
