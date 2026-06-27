# Task-8
Task 8 (Search task)


The DELETE statement removes rows from a table One of its main advantages is that it supports the WHERE clause so you can delete only specific records

For example:

DELETE FROM Patient
WHERE Age < 18;

This query deletes only patients whose age is less than 18, while keeping all other records

Now, let's look at TRUNCATE

The TRUNCATE statement removes all rows from a table at once. It does not support the WHERE clause, so you cannot delete specific rows

For example:

TRUNCATE TABLE Patient;

This command deletes every record from the Patient table but keeps the table structure

Now, let's compare them

DELETE can remove selected rows, while TRUNCATE removes all rows
DELETE supports the WHERE clause, but TRUNCATE does not
TRUNCATE is much faster because it removes data by deallocating pages instead of deleting rows one by one
DELETE does not reset the identity value, while TRUNCATE resets the identity counter if the table has one

In conclusion, use DELETE when you want to remove specific records, and use TRUNCATE when you want to quickly remove all records from a table
