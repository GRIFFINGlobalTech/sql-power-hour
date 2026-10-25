# Japan Population

> **Topic:** Aggregation<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/japan-population/problem?isFullScreen=true>

## Intuition / Approach

Approach:

1. TABLE: CITY
2. COLUMNS: POPULATION
3. ROWS: one which the COUNTRYCODE is JPN

## My Solution

```sql
SELECT SUM(POPULATION)
FROM CITY
WHERE COUNTRYCODE = 'JPN';
```

## Reflection

Reminded myself to calculate the sum.
