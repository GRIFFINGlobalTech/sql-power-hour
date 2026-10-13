# Select By ID

> **Topic:** SELECT QUERY<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/select-by-id/problem?isFullScreen=false>

## Intuition / Approach

Approach:

1. Table: CITY
2. Columns: all, so *
3. Rows: the one where ID equals 1661

## My Solution

```sql
SELECT *
FROM CITY
WHERE ID = 1661;
```

## Reflection

**Learned:** `WHERE` with `=` on an ID column picks out a single row. Numbers take no quotes.

**Revisit:** primary keys, which guarantee an ID is unique (Lesson 13.3).
