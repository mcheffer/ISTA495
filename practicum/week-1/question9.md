Write a SQL solution to output the land share of all the countries. 
Land share = land area divided by the population

SELECT country, (CAST(area AS real)/CAST(population AS real)) AS "World Land Share"
FROM world;