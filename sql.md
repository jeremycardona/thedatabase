# SQL
So what we learned with the with the relational algebra language is not useless after all, it gets us started with the type of operations and rules we have when doing SQL. So what is SQL? it stands for Structured Query Language which is a type of language to program databases. A thing to note is that sql is not case sensitive.
### creating tables
creating tables is an important part of programming databases because we much take to practice the design rules to avoid anomalies.
for example, when creating the Beer relation
```
CREATE TABLE Beer(
  id SERIALIZABLE PRIMARY KEY,
  name VARCHAR(30),
  brewery VARCHAR(30,
  adv NUMERIC(2),
  style VARCHAR(20)
);
```
### querying tables
querying tables are made with the SELECT FROM WHERE command
SELECT makes a selection of the attributes to be returned from the query
FROM make a selection of the table
WHERE make the condition
```
SELECT name
FROM Beer
WHERE adv > 5;
```

### modifications
modifications allows us to insert, update and delete from tables
*insert*: INSERT INTO table_name (column1, column2, column3, ...) VALUES (value1, value2, value3, ...); 
*update*: UPDATE table_name SET column1 = value1, column2 = value2, ... WHERE condition;
*delete*: DELETE FROM table_name WHERE condition;
