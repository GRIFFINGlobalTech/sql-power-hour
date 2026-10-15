# Japanese Cities' Names

> **Topic:** SELECT QUERY<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/japanese-cities-name/problem?isFullScreen=true>

## Intuition / Approach

Approach:

1. TABLE: CITY
2. COLUMNS: NAME
3. ROWS: one where the COUNTRYCODE equals to JPN

## My Solution

```sql
SELECT NAME
FROM CITY
WHERE COUNTRYCODE = 'JPN';
```

## Reflection

<!-- Note what you learned or what you would revisit. -->
