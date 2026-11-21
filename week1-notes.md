# Week 1 notes: SQL basics

## Keywords I've learned
- SELECT:
    To Select query for a specific column
        SELECT column, another_column, …
        FROM mytable;
    To Select queries for all columns
        SELECT * 
        FROM mytable;
- FROM:
- WHERE: 
    To Select query with constraints
    SELECT column, another_column, …
    FROM mytable
P1:
    WHERE condition (=, !=, <, <=, >, >=, BETWEEN … AND …, NOT BETWEEN … AND …, IN (…), NOT IN (…))
            AND/OR another_condition
            AND/OR …;
P2:
    WHERE condition
1.      = Case sensitive exact string comparison (notice the single equals)	col_name = "abc",
2.     != or <>	Case sensitive exact string inequality comparison	col_name != "abcd", 
3.     LIKE Case insensitive exact string comparison	col_name LIKE "ABC",
4.     NOT LIKE	Case insensitive exact string inequality comparison	col_name NOT LIKE "ABCD",
5.     %	Used anywhere in a string to match a sequence of zero or more characters (only with LIKE or NOT LIKE)	col_name LIKE "%AT% (matches "AT", "ATTIC", "CAT" or even "BATS")
6.     _	Used anywhere in a string to match a single character (only with LIKE or NOT LIKE)	col_name LIKE "AN_" (matches "AND", but not "AN")
7.     IN (…)	String exists in a list	col_name IN ("A", "B", "C")
8.     NOT IN (…)	String does not exist in a list	col_name NOT IN ("D", "E", "F")

- ORDER BY:
- LIMIT:

## My queries
1. Find the movie with a row id of 6 
       SELECT *
       FROM movies
       WHERE id = 6;
3. Find the movies released in the years between 2000 and 2010
       SELECT *
       FROM movies
        WHERE year BETWEEN 2000 AND 2010;
4. Find the movies not released in the years between 2000 and 2010
       SELECT *
       FROM movies
       WHERE year NOT BETWEEN 2000 AND 2010;
5. Find the first 5 Pixar movies and their release year
       SELECT title, year
       FROM movies
       WHERE ID <=5;
## Check-in
- What I learned:
- What confused me:
- What to repeat next week:
