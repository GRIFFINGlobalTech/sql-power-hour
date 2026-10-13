# Select All

> **Topic:** SELECT QUERY<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/select-all-sql/problem?isFullScreen=false>

## Intuition / Approach

Approach:

1. Table: CITY
2. Columns: all, so *
3. Rows: every row, so no WHERE

## My Solution

```sql
SELECT *
FROM CITY;
```

## Reflection

**Learned:** No `WHERE` means no row filter. `SELECT *` with no `WHERE` returns the whole table.

**Revisit:** why `SELECT *` is risky in real projects (Lesson 3.1).
