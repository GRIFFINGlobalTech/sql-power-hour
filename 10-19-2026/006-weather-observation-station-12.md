# Weather Observation Station 12

> **Topic:** SELECT QUERY<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/weather-observation-station-12/problem?isFullScreen=true>

## Intuition / Approach

Approach:

1. TABLE: STATION
2. COLUMNS: DISTINCT CITY
3. ROWS: WHERE and AND clauses, one which does not end and start with vowels

## My Solution

```sql
SELECT DISTINCT CITY
FROM STATION
WHERE UPPER(SUBSTR(CITY, 1, 1)) NOT IN ('a','e','i','o','u') AND
UPPER(SUBSTR(CITY, -1, 1)) NOT IN ('a','e','i','o','u');
```

## Reflection

I reminded myself the difference between AND and OR operators.
