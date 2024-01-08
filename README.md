Bash Database Management System
===============================

This Bash script serves as a simple Database Management System (DBMS) using SQL-like commands for managing databases and tables.

Features
--------

### Database Operations

-   Create Database: Allows users to create a new database.
-   List Databases: Lists all available databases.
-   Connect To Database: Enables users to connect to a specific database.
-   Drop Database: Deletes a selected database.

### Table Operations

-   Create Table: Permits the creation of tables within the connected database.
-   List Tables: Displays all tables within the connected database.
-   Drop Table: Deletes a selected table from the connected database.

### Data Operations

-   Insert into Table: Adds new records to a specified table.
-   Select From Table: Retrieves data from a specified table.
-   Delete From Table: Removes records from a specified table.
-   Update Table: Modifies existing records within a specified table.


Usage
--------

First, download this repository, unzip it in the directory you want, and cd to that directory. Open a terminal in that directory and run this command to open our program.

```console
[user@hostname ~]$ ./PenguinQuery
```

Then you can't use any of the **table operations** or **data operations** without being connected to a database first.

So if you run the project for the first time, you should create a database using this command.

**1. Create Database**

```console
[PenguinQuery]$ createDB [Your database name]
```

**Example**

```console
[PenguinQuery]$ createDB ITI
```

This command will check if the database directory exists or not. If not, it will create the directory.
Note: No database name can be redundant.

Then you can view the databases available in the directory using this command.

**2. List Databases**

```console
[PenguinQuery]$ listDB
```

After that, you still can't use any of the **table operations** or **data operations** unless you connect to a database using this command.

**3. Connect To Database**

```console
[PenguinQuery]$ . use [Your data base name]
```

**4. Drop Database**

```console
[PenguinQuery]$ drop database [Database Name]
```

*NOTE: You should be connected to that database to be able to drop it.*


**Example**

```console
[PenguinQuery]$ . use iti
```

Now you can use all the features of the program, whether it's a "table operation" or a "data operation".

Examples
--------

**5. Create Table**
   
```console
[PenguinQuery]$ createTB [Table Name] [column name 1] [column name 2] meta [data type of column 1] [data type of column 2]
```

*NOTE: You can enter any number of columns, but you still have to enter the same number of data types.*

**6. List Tables**

```console
[PenguinQuery]$ listTB
```

**7. Drop Table**

```console
[PenguinQuery]$ dropTB [Table Name]
```

**8. Insert Query**

```console
[PenguinQuery]$ insert into [Table Name] [Column Number 1] [Column Number 2] values [Value Number 1] [Value Number 2]
```

*NOTE: You can enter any number of columns to insert, but still, these columns should be in the table, and you also have to enter the same number of values as the number of columns.*


**9. Select Query**

  **- Select All The Table**

```console
[PenguinQuery]$ Select all from [Table Name]
```

**- Select Specific Row From The Table**

```console
[PenguinQuery]$ Select [Column Number 1] [Column Number 2] from [Table Name]
```

*NOTE: You can enter any number of columns to select.*


**10. Delete From Table**
  **- Delete One Value From The Table**

```console
[PenguinQuery]$ delete from [Table Name] where [Column Name For condition] = [Value of the condition]
```

  **- Delete All The Table**

  *Note: It will delete all the data and leave the columns as they are.*
  
```console
[PenguinQuery]$ delete all from [Table Name]
```

**11. Update Table**

```console
[PenguinQuery]$ updateTB [Table Name] set [Column Name 1] = [New Value 1] [Column Name 2] = [New Value 2] where [Column Name For condition] = [Value of the condition]
```

*NOTE: You can enter any number of columns to update, but still, the column names should be available in the table, and the same data types should be stored in the meta file.*

**Note: Any improvements or feedback are highly appreciated and accepted.**

### Video presentation for the project will be available soon.







