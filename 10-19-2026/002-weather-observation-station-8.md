# Weather Observation Station 8

> **Topic:** SELECT QUERY<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/weather-observation-station-8/problem?isFullScreen=true>

## Intuition / Approach

Approach:

1. TABLE: STATION
2. COLUMNS: CITY with DISTINCT names 
3. ROWS: one which starts and ends with the vowels a, e, i, o, u using WHERE and AND

## My Solution

```sql
SELECT DISTINCT CITY
FROM STATION
WHERE UPPER(SUBSTR(CITY, 1, 1)) IN ('a','e','i','o','u')
AND UPPER(SUBSTR(CITY, -1, 1)) IN ('a','e','i','o','u');
```

## Reflection

I reminded myself how to combine queries with AND.
