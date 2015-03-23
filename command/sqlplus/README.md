# sqlplus

sqlplus is the command line interface to an Oracle database.

Apart from the "connect" examples, the rest are done when logged in.


## Connect to database as SYSDBA

	sqlplus / as sysdba


## Quit sqlplus

	exit


## Sessions

Get count of current sessions.

	select count(*) from v$session;


## View table details

	describe my_table_name

Prints "Name", "Null?" and "Type".

From: [How do I list all the columns in a table?](https://stackoverflow.com/questions/1580450/how-do-i-list-all-the-columns-in-a-table)
