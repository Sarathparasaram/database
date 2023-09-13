# Introduction to PostgreSQL through pgAdmin

## PostgeSQL Essentials
  Creating a database of books.

SQL commands:
		
  	CREATE DATABASE "Books"
	WITH OWNER = postgres
	ENCODING = 'UTF8'
    CONNECTION LIMIT = -1;

Creating table.

SQL commands:
	
 	CREATE TABLE public.myauthors
	(
	    author_id integer NOT NULL,
	    first_name character varying(100),
	    middle_name character varying(50),
	    last_name character varying(100),
	    PRIMARY KEY (author_id)
	);
 
 Using an Alter command.

	ALTER TABLE public.myauthors
	    OWNER to postgres;

To see all Table data for further work:

	SELECT * FROM public.myauthors
	ORDER BY author_id ASC 	


