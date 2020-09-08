Write a SQL solution to output the land share value of the wold (that is, the sum of the land area divided by the sum of the population).

SELECT (CAST(sum(area) AS real)/CAST(sum(population) AS real)) AS "world_land_share"
FROM world;