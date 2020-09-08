Write a SQL solution to output the 10 countries who have the highest land share.

SELECT country, (CAST(area AS real)/CAST(population AS real)) AS "world_land_share"
FROM world
ORDER by world_land_share DESC
LIMIT 10;