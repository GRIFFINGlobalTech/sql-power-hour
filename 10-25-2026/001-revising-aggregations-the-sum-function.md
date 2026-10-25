# Revising Aggregations - The Sum Function

> **Topic:** Aggregation<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/revising-aggregations-sum/problem?isFullScreen=true>

## Intuition / Approach

Approach:

1. TABLE: CITY
2. COLUMNS: CITY
3. ROWS: one which the District is California, using the WHERE clause
4. SUM: use SUM to get summation of all cities where the district is California.

## My Solution

```sql
SELECT SUM(POPULATION)
FROM CITY
WHERE DISTRICT = 'California';
```

## Reflection

I learned how to sum up entries using SUM function.
