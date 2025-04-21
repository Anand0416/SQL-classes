# SQL-classes-1
Here You will find all basic SQL Classes leacture
Database is Moviedatabase. 
USE moviesdb;

-- 1. Select all columns from the Movies table
SELECT * FROM movies;

-- 2. Select Title and Industry from Movies
SELECT title, industry FROM movies;

-- 3. Find all Bollywood movies using WHERE clause
SELECT * FROM movies
WHERE industry = 'Bollywood';

-- 4. Get all distinct industries
SELECT DISTINCT industry FROM movies;

-- 5. Find all movies with 'thor' in the title (case-insensitive search depending on DB collation)
SELECT * FROM movies
WHERE title LIKE '%thor%';

-- Note: '%' is used as a wildcard for flexible text search.
-- '%Word%' matches any title containing 'Word' anywhere in it.

-- 6. Select all movies where the studio field is empty
SELECT * FROM movies
WHERE studio = '';
