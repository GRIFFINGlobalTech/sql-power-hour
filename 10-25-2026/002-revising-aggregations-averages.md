# Revising Aggregations - Averages

> **Topic:** Aggregation<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/revising-aggregations-the-average-function/problem?isFullScreen=true>

## Intuition / Approach

Approach:

1. TABLE: CITY
2. COLUMNS: POPULATION
3. ROWS: one which the District is California, using WHERE clause:
4. AVG: get the average of population using the AVG function.

## My Solution

```sql
SELECT AVG(POPULATION)
FROM CITY
WHERE DISTRICT = 'California';
```

## Reflection

I learned to calculate the average using AVG function
