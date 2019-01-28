
<!-- ## Questions

1.  Return ALL the data in the 'movies' table. -->

SELECT * FROM movies;

<!-- 2.  Return ONLY the name column from the 'people' table --> -->

SELECT name FROM people;

<!-- 3.  Oops! Someone at CodeClan spelled Anthony's name wrong! Change it to reflect the proper spelling ('Anthatony Starkes' should be 'Anthony Starke'). -->

UPDATE people SET name = 'Anthony Starke' WHERE name = 'Anthatony Starkes';

<!-- 4.  Return ONLY your name from the 'people' table. -->

SELECT * FROM people WHERE name = 'Gabor Budai'


<!-- 5.  The cinema is showing 'Batman Begins', but Batman is DC, not Marvel! Delete the entry from the 'movies' table. -->

DELETE FROM movies WHERE title = 'Batman Begins';


<!-- 6.  Create a new entry in the 'people' table with the name of one of the instructors. -->

SELECT * FROM people;

<!-- 7.  Craig Morton has decided to hijack our movie evening, remove him from the table of people. -->

DELETE FROM people WHERE name = 'Craig Morton';

<!-- 8.  The cinema has just heard that they will be holding an exclusive midnight showing of 'Captain Marvel'!! Create a new entry in the 'movies' table to reflect this. -->

INSERT INTO movies (title) VALUES ('Captain Marvel');

<!-- 9.  The cinema would also like to make the Guardians movies a back to back feature. Find out the show time of "Guardians of the Galaxy" and set the show time of "Guardians of the Galaxy 2" to start two hours later. -->

UPDATE movies SET show_time = '23:55' WHERE title = 'Guardians of the Galaxy 2';

<!-- ## Extension

1.  Research how to delete multiple entries from your table in a single command. -->

DELETE FROM movies WHERE title = 'Iron Man' OR title = 'The Incredible Hulk' OR title = 'Iron Man 2';
