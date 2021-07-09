# HackerRank-Sql-Practice-Answers
## Just seach the name of the question in via ctr+f and get your solution right in front of you.


Weather Observation Station 1

From <https://www.hackerrank.com/challenges/weather-observation-station-1/problem> 

SELECT CITY, STATE FROM STATION;


Weather Observation Station 3

From <https://www.hackerrank.com/challenges/weather-observation-station-3/problem> 



SELECT DISTINCT(CITY) FROM STATION WHERE MOD(ID, 2) = 0;


Weather Observation Station 4

From <https://www.hackerrank.com/challenges/weather-observation-station-4/problem> 

SELECT COUNT(CITY) - COUNT(DISTINCT(CITY)) FROM STATION;

Weather Observation Station 5

From <https://www.hackerrank.com/challenges/weather-observation-station-5/problem> 

SELECT *
FROM
    (SELECT CITY, LENGTH(CITY)
    FROM STATION
    ORDER BY LENGTH(CITY), CITY)
WHERE ROWNUM = 1
UNION
SELECT *
FROM
    (SELECT CITY, LENGTH(CITY)
    FROM STATION
    ORDER BY LENGTH(CITY) DESC, CITY)
WHERE ROWNUM = 1;

From <https://www.hackerrank.com/challenges/weather-observation-station-5/forum> 

Weather Observation Station 6

From <https://www.hackerrank.com/challenges/weather-observation-station-6/problem> 

SELECT CITY FROM STATION WHERE LOWER(SUBSTR(CITY,0,1)) IN ('a', 'e','i', 'o', 'u');


Weather Observation Station 7
From <https://www.hackerrank.com/challenges/weather-observation-station-7/problem> 

SELECT DISTINCT(CITY) FROM STATION WHERE LOWER(SUBSTR(CITY, -1,1)) IN ('a', 'e', 'i', 'o', 'u');

Weather Observation Station 8

From <https://www.hackerrank.com/challenges/weather-observation-station-8/problem> 

SELECT DISTINCT(CITY) FROM STATION WHERE LOWER(SUBSTR(CITY, 1,1)) IN ('a', 'e','i', 'o', 'u') AND LOWER(SUBSTR(CITY, -1,1)) IN ('a', 'e','i', 'o', 'u');
Weather Observation Station 9

From <https://www.hackerrank.com/challenges/weather-observation-station-9/problem> 

SELECT CITY FROM STATION WHERE LOWER(SUBSTR(CITY,0,1)) IN ('a', 'e','i', 'o', 'u');

Weather Observation Station 10

From <https://www.hackerrank.com/challenges/weather-observation-station-10/problem> 

SELECT CITY FROM STATION WHERE LOWER(SUBSTR(CITY,0,1)) IN ('a', 'e','i', 'o', 'u');

Weather Observation Station 11

From <https://www.hackerrank.com/challenges/weather-observation-station-11/problem> 


SELECT DISTINCT(CITY) FROM STATION WHERE LOWER(SUBSTR(CITY, 1,1)) not IN ('a', 'e','i', 'o', 'u') or LOWER(SUBSTR(CITY, -1,1)) not IN ('a', 'e','i', 'o', 'u');

Weather Observation Station 12

From <https://www.hackerrank.com/challenges/weather-observation-station-12/problem> 

SELECT DISTINCT(CITY) FROM STATION WHERE LOWER(SUBSTR(CITY, 1,1)) not IN ('a', 'e','i', 'o', 'u') and LOWER(SUBSTR(CITY, -1,1)) not IN ('a', 'e','i', 'o', 'u');

Higher Than 75 Marks

From <https://www.hackerrank.com/challenges/more-than-75-marks/problem> 

SELECT Name
FROM Students
WHERE Marks > 75
ORDER BY SUBSTR(Name, - 3), Id ASC;

Employee Names

From <https://www.hackerrank.com/challenges/name-of-employees/problem> 

SELECT NAME FROM EMPLOYEE ORDER BY NAME ASC;

Employee Salaries

From <https://www.hackerrank.com/challenges/salary-of-employees/problem> 

SELECT NAME FROM EMPLOYEE WHERE SALARY > 2000 AND MONTHS < 10 ORDER BY EMPLOYEE_ID ASC;

Revising Aggregations - Averages

From <https://www.hackerrank.com/challenges/revising-aggregations-the-average-function/problem> 

SELECT SUM(POPULATION)/COUNT(POPULATION) FROM CITY WHERE DISTRICT = 'California';

Revising Aggregations - The Count Function

From <https://www.hackerrank.com/challenges/revising-aggregations-the-count-function/problem> 

SELECT COUNT(ID) FROM CITY WHERE POPULATION > 100000;

Revising Aggregations - The Sum Function

From <https://www.hackerrank.com/challenges/revising-aggregations-sum/problem> 

SELECT SUM(POPULATION) FROM CITY WHERE DISTRICT = 'California';

Average Population

From <https://www.hackerrank.com/challenges/average-population/problem> 

SELECT ROUND(SUM(POPULATION)/COUNT(POPULATION)) FROM CITY;

Japan Population

From <https://www.hackerrank.com/challenges/japan-population/problem> 

SELECT SUM(POPULATION) FROM CITY WHERE COUNTRYCODE = 'JPN';

Population Density Difference

From <https://www.hackerrank.com/challenges/population-density-difference/problem> 

SELECT MAX(POPULATION)-MIN(POPULATION) FROM CITY;



![image](https://user-images.githubusercontent.com/50817974/125046825-00fd3600-e0bc-11eb-8421-18adbc6abc34.png)
Weather Observation Station 3

From <https://www.hackerrank.com/challenges/weather-observation-station-3/problem> 



SELECT DISTINCT(CITY) FROM STATION WHERE MOD(ID, 2) = 0;


Weather Observation Station 4

From <https://www.hackerrank.com/challenges/weather-observation-station-4/problem> 

SELECT COUNT(CITY) - COUNT(DISTINCT(CITY)) FROM STATION;

Weather Observation Station 5

From <https://www.hackerrank.com/challenges/weather-observation-station-5/problem> 

SELECT *
FROM
    (SELECT CITY, LENGTH(CITY)
    FROM STATION
    ORDER BY LENGTH(CITY), CITY)
WHERE ROWNUM = 1
UNION
SELECT *
FROM
    (SELECT CITY, LENGTH(CITY)
    FROM STATION
    ORDER BY LENGTH(CITY) DESC, CITY)
WHERE ROWNUM = 1;

From <https://www.hackerrank.com/challenges/weather-observation-station-5/forum> 

Weather Observation Station 6

From <https://www.hackerrank.com/challenges/weather-observation-station-6/problem> 

SELECT CITY FROM STATION WHERE LOWER(SUBSTR(CITY,0,1)) IN ('a', 'e','i', 'o', 'u');


Weather Observation Station 7
From <https://www.hackerrank.com/challenges/weather-observation-station-7/problem> 

SELECT DISTINCT(CITY) FROM STATION WHERE LOWER(SUBSTR(CITY, -1,1)) IN ('a', 'e', 'i', 'o', 'u');

Weather Observation Station 8

From <https://www.hackerrank.com/challenges/weather-observation-station-8/problem> 

SELECT DISTINCT(CITY) FROM STATION WHERE LOWER(SUBSTR(CITY, 1,1)) IN ('a', 'e','i', 'o', 'u') AND LOWER(SUBSTR(CITY, -1,1)) IN ('a', 'e','i', 'o', 'u');
Weather Observation Station 9

From <https://www.hackerrank.com/challenges/weather-observation-station-9/problem> 

SELECT CITY FROM STATION WHERE LOWER(SUBSTR(CITY,0,1)) IN ('a', 'e','i', 'o', 'u');

Weather Observation Station 10

From <https://www.hackerrank.com/challenges/weather-observation-station-10/problem> 

SELECT CITY FROM STATION WHERE LOWER(SUBSTR(CITY,0,1)) IN ('a', 'e','i', 'o', 'u');

Weather Observation Station 11

From <https://www.hackerrank.com/challenges/weather-observation-station-11/problem> 


SELECT DISTINCT(CITY) FROM STATION WHERE LOWER(SUBSTR(CITY, 1,1)) not IN ('a', 'e','i', 'o', 'u') or LOWER(SUBSTR(CITY, -1,1)) not IN ('a', 'e','i', 'o', 'u');

Weather Observation Station 12

From <https://www.hackerrank.com/challenges/weather-observation-station-12/problem> 

SELECT DISTINCT(CITY) FROM STATION WHERE LOWER(SUBSTR(CITY, 1,1)) not IN ('a', 'e','i', 'o', 'u') and LOWER(SUBSTR(CITY, -1,1)) not IN ('a', 'e','i', 'o', 'u');

Higher Than 75 Marks

From <https://www.hackerrank.com/challenges/more-than-75-marks/problem> 

SELECT Name
FROM Students
WHERE Marks > 75
ORDER BY SUBSTR(Name, - 3), Id ASC;

Employee Names

From <https://www.hackerrank.com/challenges/name-of-employees/problem> 

SELECT NAME FROM EMPLOYEE ORDER BY NAME ASC;

Employee Salaries

From <https://www.hackerrank.com/challenges/salary-of-employees/problem> 

SELECT NAME FROM EMPLOYEE WHERE SALARY > 2000 AND MONTHS < 10 ORDER BY EMPLOYEE_ID ASC;

Revising Aggregations - Averages

From <https://www.hackerrank.com/challenges/revising-aggregations-the-average-function/problem> 

SELECT SUM(POPULATION)/COUNT(POPULATION) FROM CITY WHERE DISTRICT = 'California';

Revising Aggregations - The Count Function

From <https://www.hackerrank.com/challenges/revising-aggregations-the-count-function/problem> 

SELECT COUNT(ID) FROM CITY WHERE POPULATION > 100000;

Revising Aggregations - The Sum Function

From <https://www.hackerrank.com/challenges/revising-aggregations-sum/problem> 

SELECT SUM(POPULATION) FROM CITY WHERE DISTRICT = 'California';

Average Population

From <https://www.hackerrank.com/challenges/average-population/problem> 

SELECT ROUND(SUM(POPULATION)/COUNT(POPULATION)) FROM CITY;

Japan Population

From <https://www.hackerrank.com/challenges/japan-population/problem> 

SELECT SUM(POPULATION) FROM CITY WHERE COUNTRYCODE = 'JPN';

Population Density Difference

From <https://www.hackerrank.com/challenges/population-density-difference/problem> 

SELECT MAX(POPULATION)-MIN(POPULATION) FROM CITY;

Type of Triangle

From <https://www.hackerrank.com/challenges/what-type-of-triangle/problem> 

SELECT CASE WHEN A + B <= C OR A + C <= B OR B + C <= A THEN 'Not A Triangle'
            WHEN A = B AND B = C THEN 'Equilateral'
            WHEN A = B OR A = C OR B = C THEN 'Isosceles'
            ELSE 'Scalene'
        END
FROM TRIANGLES

The PADS

From <https://www.hackerrank.com/challenges/the-pads/problem> 

SELECT Name || '(' || SUBSTR(Occupation, 1, 1) || ')'
FROM OCCUPATIONS
ORDER BY Name;
SELECT 'There are a total of ' || Count(Name) || ' ' || LOWER(Occupation) || 's.'
FROM Occupations
GROUP BY Occupation
ORDER BY Count(Name), Occupation;


