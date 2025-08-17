## What is PostgreSQL?
PostgreSQL is an open source relational database management system that use SQL as query language. It has a strong coummunity for support and it supports JSON and advanced SQL features.

## What is the difference between the VARCHAR and CHAR data types?
Both <code>VARCHAR</code> and <code>CHAR</code> are data type for storing strings. But the key differences of them are, 
<table style="border: 1px solid">
    <thead>
        <tr> 
            <td><code>VARCHAR</code></td>
            <td><code>CHAR</code></td>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                Length is variable. 
            </td>
            <td>Length is fixed</td>
        </tr>
        <tr>
            <td>Adds no padding (no extra empty space)</td>
            <td>Adds padding if value is provide less then the defined length</td>
        </tr>
        <tr>
            <td>Use for variable size string, like name, emails etc</td>
            <td>Use for fixed size string, like blood group, CGPA etc</td>
        </tr>
    </tbody>
</table>

## Explain the purpose of the WHERE clause in a SELECT statement.
The <code>WHERE</code> clause in a <code>SELECT</code> statement is used to filter down rows from the targeted table based on the provided condition. For example,
```SQL
SELECT * FROM student 
    WHERE age > 18;
```
In this statement we are selecting rows of <code>student</code> table who are more than 18 years old. 

## How can you modify data using UPDATE statements?
To modify data using <code>UPDATE</code> we need to specify something, the <code>table name, column name, updated value of that column, row selection condition</code>. <br>
For example, let's say we have a table of students where each student has grade, status column along with name, id etc. So we want to update the status column value to 'Inactive' whom have their grade to 'F'. 

```SQL
UPDATE student
    SET "status" = 'Inactive'
    WHERE 'grade' = 'F';
```