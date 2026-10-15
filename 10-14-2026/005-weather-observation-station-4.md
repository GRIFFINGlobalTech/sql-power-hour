# Weather Observation Station 4

> **Topic:** SELECT QUERY<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/weather-observation-station-4/problem?isFullScreen=true>

## Intuition / Approach

Approach:

1. TABLE: STATION
2. COLUMNS: CITY
3. Counting: Use COUNT

## My Solution

```sql
SELECT COUNT(CITY) - COUNT(DISTINCT CITY)
FROM STATION;
```

## Reflection

I have learned to use COUNT
