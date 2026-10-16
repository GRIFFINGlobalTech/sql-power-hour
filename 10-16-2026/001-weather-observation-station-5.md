# Weather Observation Station 5

> **Topic:** BASIC SELECT QUERY<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/weather-observation-station-5/problem?isFullScreen=true>

## Intuition / Approach

Approach:

1. TABLE: STATION
2. COLUMNS: CITY and CITY length
3. Order items in ascending and descending manners

## My Solution

```sql
(SELECT CITY, LENGTH(CITY) FROM STATION
ORDER BY LENGTH(CITY) ASC, CITY ASC
LIMIT 1
)
UNION ALL
(SELECT CITY, LENGTH(CITY) FROM STATION
ORDER BY LENGTH(CITY) DESC, CITY ASC
LIMIT 1);
```

## Reflection

I learned how to orders items in ascending and descending manners using ORDER BY
Also learned to calcute the lenght of an item using LENGTH.
Learned as well to combine results with UNION and UNION ALL, for UNION, there are no duplicates but for UNION ALL we include every rows/results
