#h1 x) Read and summarize

#h1 OWASP Top 10 (2021)

#h2 A01:2021 – Broken Access Control

- As I get, it means when users can do stuff they not supposed to do like see or change other people data.

- Mostly happens when devs forgot to check who is allowed for what.

- It could be really bad because attackers can access to personal data or maybe even admin functions.

  #h2 A05:2021 – Security Misconfiguration

- Mostly happens when devs makes the setup wrong or left in default.

- Like default password there are too much error info, or leaving stuff open.

- This problem is very common because configs are really complicated.

#h2 A06:2021 – Vulnerable and Outdated Components

-  This problem uses old libraries or frameworks with known bugs.

-  Old versions are bad because hackers already knows the exploits.

-  Best way is to keep your system or program updated but most people doesn't does it

  #h2 A03:2021 – Injection

  - When user input goes directly to interpreter

  - Attackers could steal or delete data in this situation.

  - The main fix to this is parameter queries or cleaning input.

#h2 Munroe: xkcd 327 – Exploits of a Mom

- Comic where mom types "; DROP TABLE users;-- as name.

- Shows how dangerous it is if input not checked.

- It shows simple input can break whole system.

#h1 a) Goat. Install WebGoat 2023.4.

I had problems while installing it unfortunetly.

#h1 b) F12. Solve Webgoat 2023.4: General: Developer tools.

#h1 c) Not outdated. Update all operating system and all applications in your Linux.

- I got my updates with sudo apt-get update command.

#h1 d) Sequel. Solve SQLZoo:

#h2 0 SELECT basics:

1.SELECT population FROM world
  WHERE name = 'Germany'

2.SELECT name, population FROM world
  WHERE name IN ('Sweden', 'Norway','Denmark');

3.SELECT name, area FROM world
  WHERE area BETWEEN 200000 AND 250000

#h2 2 SELECT from World: First two subtasks: "1. You can use WHERE..." and "2. Find the countries...".:

1.SELECT name, continent, population FROM world

2.SELECT name FROM world
WHERE population >= 200000000

3.SELECT name, gdp/population from world
Where population >= 200000000

4.SELECT name, population/1000000 FROM world
WHERE continent = 'South America'

5.SELECT name, population FROM world
WHERE name IN ('France', 'Germany', 'Italy')

6.SELECT name From world
WHERE name LIKE '%United%'

7.SELECT name, population, area FROM world
WHERE area >= 3000000 OR population > 250000000

8.SELECT name,population,area FROM world
WHERE (area > 3000000 OR population > 250000000)
  AND NOT (area > 3000000 AND population > 250000000)



10.SELECT name, ROUND(gdp/population, -3) FROM world
Where gdp >= 1000000000000

11.SELECT name, capital FROM world
WHERE LENGTH(name) = LENGTH(capital);

12.SELECT name, capital FROM world
WHERE LEFT(name, 1) = LEFT(capital, 1)
  AND name <> capital;

13.SELECT name FROM world
WHERE name LIKE '%a%'
  AND name LIKE '%e%'
  AND name LIKE '%i%'
  AND name LIKE '%o%'
  AND name LIKE '%u%'
  AND name NOT LIKE '% %';

#h1 e) Solve Portswigger Labs: Lab: SQL injection vulnerability in WHERE clause allowing retrieval of hidden data. Explain how and why! How can you find the vulnerabitiy? What each part of the exploit does?

I just stuck at the exploit part.
