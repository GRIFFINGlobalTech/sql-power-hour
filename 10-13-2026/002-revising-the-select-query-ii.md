# Revising the Select Query II

> **Topic:** SELECT QUERY<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/revising-the-select-query-2/problem?isFullScreen=false>

## Intuition / Approach

Approach: Three questions.

Table: CITY
Columns: only NAME (the problem says “the NAME field”, so no *)
Rows: COUNTRYCODE = 'USA' and POPULATION > 120000, joined with AND

## My Solution

```sql
SELECT NAME
FROM CITY
WHERE COUNTRYCODE = 'USA'
  AND POPULATION > 120000;
```

## Reflection

**Learned:** `SELECT` picks which columns to show: `*` for all, or a column name for just that one. The filter logic in `WHERE` is independent of that choice.

**Revisit:** selecting several specific columns, separated by commas (Lesson 3.1).
