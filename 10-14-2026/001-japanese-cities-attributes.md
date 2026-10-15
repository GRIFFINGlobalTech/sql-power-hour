# Japanese Cities' Attributes

> **Topic:** SELECT QUERY<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/japanese-cities-attributes/problem?isFullScreen=true>

## Intuition / Approach

Approach:

1. TABLE: CITY
2. COLUMNS: all, so *
3. ROWS: the one where COUNTRYCODE equals to JPN

## My Solution

```sql
SELECT *
FROM CITY
WHERE COUNTRYCODE = 'JPN';
```

## Reflection

<!-- Note what you learned or what you would revisit. -->
