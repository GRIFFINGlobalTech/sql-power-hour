# Weather Observation Station 3

> **Topic:** SELECT QUERY<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/weather-observation-station-3/problem?isFullScreen=true>

## Intuition / Approach

Approach:

1. TABLE: STATION
2. COLUMNS: CITY 
3. ROWS: one where they have even ID numbers
4. Exclude Dplicates: use DISTINCT

## My Solution

```sql
SELECT DISTINCT CITY
FROM STATION
WHERE MOD(ID, 2) = 0;
```

## Reflection

I have learned to use DISTINCT to avoid duplicates i.e DISTINCT CITY.
Also learned to use MOD to find modulus i.e MOD(ID, 2)
