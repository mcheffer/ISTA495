1. Download and install PostgreSQL database (it is available at https://www.postgresql.org)
2. Create a database and name it as ISTA495.practicum
3. Ctreat the following table:
  - table name: world
  - table columns: id, country, population, area, migrants,fertility,medianage,urbanpopulation(id is a number, everything else is a string). 
4. Populate the world table using the csv file included in this folder

<<<<<<< HEAD
my solution
=======
Hint:

* [How to import CSV file into PostgreSQL table](https://www.postgresqltutorial.com/import-csv-file-into-posgresql-table/)

* [How to import a selected number of the columns of a csv file](https://stackoverflow.com/questions/12618232/copy-a-few-of-the-columns-of-a-csv-file-into-a-table/49906327)
>>>>>>> e24388818c80d8a710860d161196d26620ccf531

3.

CREATE TABLE world (
  id integer NOT NULL,
  country text,
  population integer,
  yearlychange real,
  netchange integer,
  area integer,
  migrants integer,
  fertility real,
  medianage integer,
  urbanpopulation real,
  PRIMARY KEY (id)
);

4. Used pgAdmin Import/Export data feature to import world.csv

ALTER TABLE world
DROP COLUMN yearlychange;

ALTER TABLE world
DROP COLUMN netchange;