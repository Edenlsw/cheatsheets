# DATABASES

## What is SQL/ Sequel
SQL/Sequel - is a language that communicates with databases
</br>
SQL only talks to relational database

</br>
</br>
</br>


  <li>
    Databases are storage shelves for the digital world. 
  </li>
  <li>
    Every database has a DBMS (Database Management System) 
  </li>
  <li>
    DBMS structures how we organise and interact with the stored data.
  </li> 
  <br>
CRUD = 4 fundamental ways we interact with the database
  <ol>
    <li>
      CREATE
    </li>
    <li>
      READ
    </li>
    <li>
      UPDATE
    </li>
    <li>
      DELETE
    </li>
</ol>



### <ins>There 2 different types of DBMS</ins>

<ins>RELATIONAL</ins>

<li>
Organises data in tables made with columns and rows.
</li>
<li>
Columns = categories
</li>
<li>
Rows = holds data entry 
</li>
<li>
Very structured and strict with data types
</li>
<li>
Making it great for managing complex datasets.  
</li>
<li>
You talk to the database using SQL (Structured, Query, Language)
</li>
<li>
You arrange the pattern of rows, columns and tables using a schema. 
</li>

<br>
<ins>NON-RELATIONAL</ins>

<br>
<li>
AKA = ‘NoSQL’
</li>
<li>
Doesn’t use SQL to communicate. 
</li>
<li>
More flexible, not as strict with data types
</li>
<li>
Good for getting a database up and running quickly because you don’t have to create a schema ( which is usually strict) before adding data.
</li>
<li>
It’s also good for deploying data across decentralised distribution networks (data stored across different computers that all have coordinates with each other)
</li>


</br>
</br>
</br>






-----------------------------------------------------
###    <ins> PSQL Cheatsheet </ins>
</br>
<div>

#### How to list all databases

<ul>
  <li>
    postgres=#   \l
  </li>
</ul>

#### How to create a database
<ul>
  <li>
    admin=# CREATE DATABASE bookmark_manager;
  </li>
</ul>

#### How to change from one database to another 
<ul>
  <li>
    admin=# \c bookmark_manager;
  </li>
</ul>

#### How to show table contents 
<ul>
  <li>
    admin=# \c bookmark_manager;
  </li>
</ul>

#### How to inspect existing list of a table 
<ul>
  <li>
    admin=# \dt
  </li>
</ul>

<br>

## CRUD --- create, read, update, delete

<br>


#### How to view all contents in a table 
<ul>
  <li>
    bookmark_manager=# SELECT * FROM bookmarks;
  </li>
</ul>

#### Manual ID ( insert data table)
<ul>
  <li>
    bookmark_manager=# INSERT INTO bookmarks VALUES(1, 'http://www.makersacademy.com');

  </li>
</ul>

#### Automatic ID ( insert data table)
<ul>
  <li>
    bookmark_manager=# INSERT INTO bookmarks (url) VALUES ('http://www.makersacademy.com');

  </li>
</ul>


#### Delete Data
<ul>
  <li>
    DELETE FROM bookmarks WHERE url = 'http://www.twitter.com';
  </li>
</ul>

#### Update data
<ul>
  <li>
    UPDATE bookmarks SET url = 'http://www.destroyallsoftware.com' WHERE url = 'http://www.askjeeves.com';
  </li>
</ul>

</div>
