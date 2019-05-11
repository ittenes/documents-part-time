# Mongo

## Lecture

- database
- rdbms vs object vs graph vs key/value
- collections
- documents
- relations
- data modeling/domains
- crud
- query
- atomic operations(update operators)

- draw diagram on the board, explaining what is mongo -> databases -> collections -> documents
- what is schemaless, mongo does not care how the data looks like
- we will add schemas on the nodejs, it will run on our express app
- the difference with sql and how it stores data in tables
  - examples being: mysql, postgres, mssql
  - when adding an incomplete row to sql it will not accept it
  - adding a new row can be done but is cumbersome
  - very restrictive, e.g (add phone number, ok, but if you want to add a second number, it's not easy)
    - solution is to add a new table for phones
- non-relational, relations are added through schemas and nodejs, not on mongo
- speed is a plus in mongo
- distributed as one of the best features vs sql, the data does not need to be all on the same computer
- talk about how it is not possible to do operations depending on each other
  - sql with 3 steps, will make sure it's able to do the three operations for it to be completed
  - mongo does not care, 2 might go through and the third not
    - this would be solved with a distributed database
  - with 2 operations from different users at the same time, you would need to read, edit and save, there might be an issue that it tries to save and it will overwrite the whole document. Atomic operations can fix this, where you directly give the instruction to edit and save
- data modeling is the act of designing how the data looks like in your database

## Research

- diagram
  - database
  - collections
  - documents
  - relations
  - data modeling
  - crud
  - domains

## Code Along

- crud user
- query operators
  - 'user collection' insert (name, country slug, age)
  - find by country
  - find by age

## Practice

- Lab: Advanced querying mongo @todo link and notes