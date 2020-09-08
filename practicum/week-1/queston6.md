Write a SQL solution to output the 10 most dense countries.

SELECT country, (CAST(population as real)/CAST(area AS real)) AS "population_density"
FROM world
WHERE population > 0
AND area > 0
ORDER BY population_density DESC
LIMIT 10;