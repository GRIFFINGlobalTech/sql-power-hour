# Weather Observation Station 7

> **Topic:** SELECT QUERY<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/weather-observation-station-7/problem?isFullScreen=true>

## Intuition / Approach

Approach:

1. TABLE: STATION
2. COLUMN: CITY with DISTINCT name
3. ROW: one which ends with vowels, a, e, i, o . u

## My Solution

```sql
SELECT DISTINCT CITY
FROM STATION
WHERE UPPER(SUBSTR(CITY, -1, 1)) IN('a','e','i','o','u');
```

## Reflection

I learned how to filter last characters from a word. Using SUBSTR you can provide the starting position and the length of the character to select.
