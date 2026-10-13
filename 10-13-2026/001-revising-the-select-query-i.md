# Revising the Select Query I

> **Topic:** SELECT QUERY<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/revising-the-select-query/problem?isFullScreen=false>

## Intuition / Approach

My approach was to translate the sentence into three questions, because every basic SQL query answers the same three:

1. Which table? “CITY table” → FROM CITY
2. Which columns? “All columns” → SELECT *
3. Which rows? “American” and “population larger than 100000” → WHERE, one condition per phrase, joined with AND because both must hold

## My Solution

```sql
SELECT *
FROM CITY
WHERE COUNTRYCODE = 'USA'
  AND POPULATION > 100000;
```

## Reflection

**Learned:** Every basic query answers three questions: which table (`FROM`), which columns (`SELECT`), which rows (`WHERE`). Text needs quotes (`'USA'`), numbers don't and take no commas. `AND` needs both conditions true.

**Revisit:** `OR`, `IN`, `BETWEEN`, and `NULL` behavior in `WHERE`.
