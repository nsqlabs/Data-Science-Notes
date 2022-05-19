- Write a query that returns songs that ranked between 10 and 20 (inclusive) in 1993, 2003, or 2013.
- Order the results by year and rank.

```SQL
SELECT song_name, year, year_rank
FROM tutorial.billboard_top_100_year_end
WHERE (year_rank BETWEEN 10 AND 20) AND (year IN  (1993, 2003, 2013))
ORDER BY year, year_rank;
```