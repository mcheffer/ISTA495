Write a SQL solution to output the population density (population per unit area) of all countries.

SELECT country, (population/area) AS 'Population Density'
FROM world
WHERE population > 0
AND area > 0;