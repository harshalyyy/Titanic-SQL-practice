# Titanic-SQL-practice
SQL project analyzing the Titanic dataset including passenger information, survival status, age, gender, and class. Queries include survival analysis, passenger statistics by class/gender, and other insights. Files:
CREATE DATABASE titanic_db;

SELECT COUNT(*) AS total_passengers FROM titanic;
SELECT Survived, COUNT(*) AS count
FROM titanic
GROUP BY Survived;

SELECT Pclass, COUNT(*) AS total_in_class
FROM titanic
GROUP BY Pclass;

SELECT AVG(Age) AS avg_age FROM titanic;

SELECT Sex, Survived, COUNT(*) AS count
FROM titanic
GROUP BY Sex, Survived;

SELECT Pclass, AVG(Fare) AS avg_fare
FROM titanic
GROUP BY Pclass;


