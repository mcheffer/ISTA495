Which countries receive the most migrants? List the name and the migrants number of the top 10.

SELECT country, migrants 
FROM world
WHERE migrants IS NOT NULL 
ORDER BY migrants DESC;