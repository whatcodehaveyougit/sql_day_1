# SQL Homework

The Springfield Cinema is having a Marvel Movie Marathon! They have asked you to help maintain their database of movies with times and attendees.

## To access the database:

First, create a database called 'marvel'

```
# terminal
createdb marvel
```

Next, run the provided SQL script to populate your database:

```
# terminal
psql -d marvel -f marvel.sql
```

Use the supplied data as the source of data to answer the questions. Copy the SQL command you have used to get the answer, and paste it below the question, along with the result they gave.

## Questions

1.  Return ALL the data in the 'movies' table.
SELECT * FROM movies;
2.  Return ONLY the name column from the 'people' table
SELECT name FROM people;
* means everything so don't put that in!!

3.  Oops! Someone spelled Cody Abbott's name wrong! Change it to reflect the proper spelling.
UPDATE people SET name = 'Cody Abbot' WHERE id = '5';
Make sure to put it above the statement which prints the thing to the terminal

4.  Return ONLY Olivia Wright's name from the 'people' table.
SELECT * FROM people WHERE id = 15;

5.  The cinema is showing 'Batman Begins', but Batman is DC, not Marvel! Delete the entry from the 'movies' table.
DELETE FROM movies where title = 'Batman Begins';

6.  We forgot one of the main characters! Add Chris Fraser to the 'people' table
INSERT INTO people (name) VALUES ('Chris Fraser');

7.  John Smith has decided to hijack our movie evening, Remove him from the table of people.
DELETE FROM people where name = 'James Smith';

8.  The cinema has just heard that they will be holding an exclusive midnight showing of 'Avengers: Infinity War'!! Create a new entry in the 'movies' table to reflect this.
INSERT INTO movies (title, year, show_time) VALUES ('Avengers: Infinity War', 2000, '12.30');


9.  The cinema would like to make the Iron Man movies a triple billing. Find out the show time of "Iron Man 2" and set the show time of "Iron Man 3" to start two hours later.



## Extension

1.  Research how to delete multiple entries from your table in a single command.
