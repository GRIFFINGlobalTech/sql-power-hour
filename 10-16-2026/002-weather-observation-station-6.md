# Weather Observation Station 6

> **Topic:** SELECT QUERY<br>
> **Difficulty:** Easy<br>
> **HackerRank:** <https://www.hackerrank.com/challenges/weather-observation-station-6/problem?isFullScreen=true>

## Intuition / Approach

## Approach

1. Split the question into the standard parts:
   - Table: STATION
   - Column: CITY
   - Rows: only cities starting with a vowel
   - Extra rule: no duplicates, so `DISTINCT`
2. Turn the fuzzy rule into a yes/no test on one piece of the row:
   "starts with a vowel" becomes "is the first letter one of A, E, I, O, U?"
3. Pick the tool by what I know about the value:
   - whole value: `=`
   - start, end, or middle piece: `LIKE` with `%`, or `SUBSTR`
   - a set of allowed values: `IN (...)`
4. Check by hand on a few rows before submitting.
5. Add finishing rules last (`DISTINCT`, `ORDER BY`).

## My Solution

```sql
SELECT DISTINCT CITY
FROM STATION
WHERE UPPER(SUBSTR(CITY, 1, 1)) IN ('a', 'e', 'i', 'o', 'u');
```

## Reflection

**Learned:** `LIKE` with `%` matches text patterns (starts with, ends with, contains). `SUBSTR(col, 1, 1)` extracts the first letter, and `IN (...)` replaces a chain of `OR`s. Check case when comparing text.

**Revisit:** `LIKE` and wildcards (Lesson 4.5), `IN` (Lesson 4.3), regular expressions (Lesson 4.6), and operator precedence (Lesson 4.2).
