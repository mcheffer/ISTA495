Write a SQL solution to output the 10 least dense countries.

SELECT country, (CAST(population AS real)/CAST(area AS real) AS "population_density"
FROM world
WHERE population > 0
AND area > 0
ORDER BY population_density ASC
LIMIT 10;