You've written select queries

subqueries (including correlated subqueries and derived tables)

Window functions

Common table expressions

You've written, INSERT, UPDATE and DELETE statements (including truncate where appropriate)

You've used temp tables

You've used control flow statements (IF/ELSE)

You've used CASE statements

You've used various join types (INNER, OUTER, LEFT, RIGHT, FULL, CROSS JOIN (and explain the rare circumstances where CROSS joins are needed))

You know the difference between UNION AND UNION ALL



For DDL skills

You've created 3NF schemas or denormalized schemas

You've written stored procedures, triggers and/or functions

You've created views



For environment skills

Performance tuning

Index creation and maintenance

Index hints




CREATE TRIGGER trigger_name
{BEFORE | AFTER} {INSERT | UPDATE| DELETE }
ON table_name FOR EACH ROW
trigger_body;


CREATE TRIGGER rong_t1
 AFTER INSERT 
ON employees FOR EACH ROW
INSERT INTO offices
 SET action = 'update',
     officeCode = 1000,
     city = "CC";
SHOW TRIGGERS;