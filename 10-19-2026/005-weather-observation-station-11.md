# Weather Observation Station 11

> **Topic:** SELECT QUERY<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/weather-observation-station-11/problem?isFullScreen=true>

## Intuition / Approach

Approach:

1. TABLE: STATION
2. COLUMNS: DISTINCT CITY
3. ROWS: WHERE and OR clauses, one which does not end or start with vowels

## My Solution

```sql
SELECT DISTINCT CITY
FROM STATION
WHERE UPPER(SUBSTR(CITY, 1, 1)) NOT IN ('a','e','i','o','u') OR
UPPER(SUBSTR(CITY, -1, 1)) NOT IN ('a','e','i','o','u');
```

## Reflection

I learned the OR operator. Which simply means either.
