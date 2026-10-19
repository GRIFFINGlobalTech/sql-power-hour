# Weather Observation Station 10

> **Topic:** SELECT QUERY<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/weather-observation-station-10/problem?isFullScreen=true>

## Intuition / Approach

Approach:

1. TABLE: STATION
2. COLUMNS: DISTINCT CITY
3. ROWS: WHERE clause, one which does not end in vowels

## My Solution

```sql
SELECT DISTINCT CITY
FROM STATION
WHERE UPPER(SUBSTR(CITY, -1, 1)) NOT IN ('a','e','i','o','u');
```

## Reflection

I reminded myselef how to filter last characters of a word and how to negate IN.
