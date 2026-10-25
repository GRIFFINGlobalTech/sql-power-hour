# Average Population

> **Topic:** Aggregation<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/average-population/problem?isFullScreen=true>

## Intuition / Approach

Appoach

1. TABLE: CITY
2. COLUMNS: POPULATION
3. ROUND: round off to the closest/nearest integer

## My Solution

```sql
SELECT ROUND(AVG(POPULATION), 0)
FROM CITY;
```

## Reflection

I learned to ROUND off to the nearest integer using 0, specific decimal places, nearest ten/hundred
1. Nearest Integer; ROUND(number, 0)
2. Specific decimal places; ROUND(number, 2) - two decimal places
3. Nearest ten/hundred; ROUNDU(number, -1)
