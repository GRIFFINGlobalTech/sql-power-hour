# Population Density Difference

> **Topic:** Aggregation<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/population-density-difference/problem?isFullScreen=true>

## Intuition / Approach

Approach:

1. TABLE: CITY
2. COLUMN: POPULATION
3. MAX & MIN: get the maximum and minimum populations

## My Solution

```sql
SELECT MAX(POPULATION) - MIN(POPULATION)
FROM CITY;
```

## Reflection

I learned how to get the maximun and minimum values using the MAX and MIN functions.
