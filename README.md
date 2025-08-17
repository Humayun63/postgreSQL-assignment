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