

Q1. Query all columns for all American cities in the CITY table with populations larger than 100000.
The CountryCode for America is USA.

	Ans - select * from CITY where COUNTRYCODE = 'USA' and POPULATION > 100000;


Q2. Query the NAME field for all American cities in the CITY table with populations larger than 120000.
The CountryCode for America is USA.

	Ans - select NAME from CITY where COUNTRYCODE = 'USA' and POPULATION > 120000;


Q3. Query all columns (attributes) for every row in the CITY table.

	Ans - select * from CITY;


Q4. Query all columns for a city in CITY with the ID 1661.

	Ans - select * from CITY where ID=1661;


Q5. Query all attributes of every Japanese city in the CITY table. The COUNTRYCODE for Japan is JPN.

	Ans - select * from CITY where COUNTRYCODE = 'JPN';


Q6. Query the names of all the Japanese cities in the CITY table. The COUNTRYCODE for Japan is
JPN.

	Ans - select DISTRICT from CITY where COUNTRYCODE = 'JPN';


Q7. Query a list of CITY and STATE from the STATION table.

	Ans - select City, State from Station;
	

Q8. Query a list of CITY names from STATION for cities that have an even ID number. Print the results in any order, but exclude duplicates from the answer.

	Ans - select Distinct City from Station where Id%2 = 0;


Q9. Find the difference between the total number of CITY entries in the table and the number of distinct CITY entries in the table.

	Ans - (select count(City) from Station) - (select count(distinct(City)) from Station)


Q10. Query the two cities in STATION with the shortest and longest CITY names, as well as their respective lengths (i.e.: number of characters in the name).
If there is more than one smallest or largest city, choose the one that comes first when ordered alphabetically.

	Ans - select City, length(City) from Station order by length(name) asc limit 1;
	      select City, length(City) from Station order by length(name) desc limit 1;


Q11. Query the list of CITY names starting with vowels (i.e., a, e, i, o, or u) from STATION. Your result
cannot contain duplicates.

	Ans - select City from Station where City like 'a%' OR City like 'e%' OR City like 'i%' OR City like 'o%' OR City like 'u%';


Q12. Query the list of CITY names ending with vowels (a, e, i, o, u) from STATION. Your result cannot contain duplicates.

	Ans - select distinct City from Station where City like '%a' OR City like '%e' OR City like '%i' OR City like '%o' OR City like '%u';


Q13. Query the list of CITY names from STATION that do not start with vowels. Your result cannot contain duplicates.

	Ans - select City from Station where City not like 'a%' OR City not like 'e%' OR City not like 'i%' OR City not like 'o%' OR City not like 'u%';


Q14. Query the list of CITY names from STATION that do not end with vowels. Your result cannot contain duplicates.

	Ans - select City from Station where City not like '%a' OR City not like '%e' OR City not like '%i' OR City not like '%o' OR City not like '%u';


Q15. Query the list of CITY names from STATION that either do not start with vowels or do not end with vowels. Your result cannot contain duplicates.

	Ans - SELECT DISTINCT CITY FROM STATION WHERE (CITY NOT IN (SELECT CITY FROM STATION WHERE CITY LIKE '%a' OR CITY LIKE '%e' OR CITY LIKE '%i' OR CITY LIKE '%o' OR CITY LIKE '%u')) OR (CITY NOT IN (SELECT CITY FROM STATION WHERE CITY LIKE 'A%' OR CITY LIKE 'E%' OR CITY LIKE 'I%' OR CITY LIKE 'O%' OR CITY LIKE 'U%'));


Q16. Query the list of CITY names from STATION that do not start with vowels and do not end with vowels. Your result cannot contain duplicates.

	Ans - SELECT DISTINCT CITY FROM STATION WHERE (CITY NOT IN (SELECT CITY FROM STATION WHERE CITY LIKE '%a' OR CITY LIKE '%e' OR CITY LIKE '%i' OR CITY LIKE '%o' OR CITY LIKE '%u')) AND (CITY NOT IN (SELECT CITY FROM STATION WHERE CITY LIKE 'A%' OR CITY LIKE 'E%' OR CITY LIKE 'I%' OR CITY LIKE 'O%' OR CITY LIKE 'U%'));























