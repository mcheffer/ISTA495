Which countries have a low population density, low fertility rate and hig migrants? List the top 10. 

SELECT country, CAST(population AS real)/CAST(area AS real) AS "population_density", fertility, migrants
FROM world
WHERE population IS NOT NULL AND area IS NOT NULL AND fertility IS NOT NULL AND migrants IS NOT NULL
ORDER BY population_density ASC, fertility ASC, migrants DESC
LIMIT 10;