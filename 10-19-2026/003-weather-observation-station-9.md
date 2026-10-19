# Weather Observation Station 9

> **Topic:** SELECT QUERY<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/weather-observation-station-9/problem?isFullScreen=true>

## Intuition / Approach

Approach:

1. TABLE: STATION
2. COLUMNS: DISTINCT CITY
3. ROWS: WHERE clause, one which does not start with vowels.

## My Solution

```sql
SELECT DISTINCT CITY
FROM STATION
WHERE UPPER(SUBSTR(CITY, 1, 1)) NOT IN ('a','e','i','o','u');
```

## Reflection

I learned to negate IN by using NOT IN.
