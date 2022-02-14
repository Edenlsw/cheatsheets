# DATABASES

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

## CRUD

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
