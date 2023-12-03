--Part 1--
/* 1. Find the title of each film */

SELECT Title
From movies;

/* 2. Find the director and year of each film */

SELECT director , year
From movies;

/* 3. Find all the information about each film */

SELECT*
From movies;

--Part 2--
/* 1. Find the movie with a row id of 6 */

SELECT id, title 
FROM movies 
WHERE id = 6;

/* 2. Find the movies released in the years between 2000 and 2010 */

Select title
from movies
where year between 2000 And 2010

/* 3. Find the first 5 Pixar movies and their release year */

Select title, year
from movies
limit 5

--Part 3--
/* 1. Find all the movies directed by John Lasseter */

SELECT title, director 
FROM movies 
WHERE director LIKE "John Lasseter";


/* 2. Find all the movies (and director) not directed by John Lasseter */

SELECT title, director 
FROM movies 
WHERE director not LIKE "John Lasseter";


