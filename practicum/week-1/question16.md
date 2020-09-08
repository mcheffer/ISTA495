Which country has the highest medium age and lowest fertility rate?

SELECT country, medianage, fertility
FROM world
WHERE medianage IS NOT null AND fertility IS NOT null
ORDER BY medianage DESC, fertility ASC
LIMIT 1;