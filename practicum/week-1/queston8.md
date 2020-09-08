Write a SQL solution to output the population density of the world. That is, the sum of the population 
of all the countries divided by the sum of the land area of all the countries. 

SELECT (CAST(sum(population) AS real)/ CAST(sum(area) AS real)) AS "World Pop Density"
FROM world;