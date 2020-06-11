# SQL

---

### QUERIES

A **query** is a way to access a database's information. 

Different QUERY commands: 

```SQL
SELECT
INSERT
UPDATE
DELETE
```

Select all columns from a table where a specific condition is met:

`SELECT * FROM table_name WHERE data = 'condition'`

**NOTE** - name all SQL variables with underscore spacing. 

---

#### INSERT

`INSERT INTO table-name (column-name) VALUE 'value';`

---

### Command Line & PSQL

Connect to a database.

`\c (data-base-name)`

List all databases

`\l`

Disconnect from the DB.

`\q`

Remove a DB.

`DROP DATABASE (database-name);`

Connect to a DB and see tables.

`\dt`

Connect a file to a DB and run the file.
`-f` stands for 'file'.

`psql -f (file-name) -d (DB name)`

---
