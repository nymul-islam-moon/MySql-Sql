# This is the documentation for MySqlServer

# Commands

## 1. Database

### 1. Show all the database list in mysql

- SHOW ALL DATABASES
    
    ```SQL
        SHOW DATABASES
    ```

### 2. CREATE DATABASE command creats a new database of that name.

- CREATE DATABASE database_name

    ```SQL
        CREATE DATABASE database_name
    ```

### 3. DROP DATABASE command drop the database.

- DROP DATABASE database_name

    ```SQL
        DROP DATABASE database_name
    ```

## 2. Table

<br>

### 1. CREATE TABLE

```SQL
    CREATE TABLE table_name
    (
        id int,
        name varchar(255),
        gender varchar(255),
        age varchar(255),
        gpa varchar(255),
        city varchar(255),
        PRIMARY KEY (id)
    );
```

### 2. DROP TABLE

```SQL
    DROP TABLE table_name
```

### 3. Rename table_name

```SQL
    RENAME TABLE old_name TO new_name
```

## DWM (Data Manipulation Language) -> INSERT, UPDATE, DELETE, SELECT

<br>

### 4. INSERT DATA INTO TABLE

- System one 
    
    ```SQL
    
        INSERT INTO table_name ('id', 'name', 'value') 
        VALUES (1,'test_name','test_value');
    
    ```
- System two 

    ```SQL
        INSERT INTO table_name VALUES (1,'test_name','test_value');
    ```

- Insert multiple rows

    ```SQL
        INSERT INTO table_name VALUES 
        (1,'test_name_1','test_value'),
        (2,'test_name_2','test_value'),
        (3,'test_name_3','test_value');
    
    ```

### 5. SELECT statement

1. Select statement helps to find data.
    
    - FIND SPECIFIC COLUMN DATA FROM TABLE

        ```SQL
            SELECT name FROM table_name;
        ```

    - FIND SPECIFIC COLUMNS FROM TABLE

        ```SQL
            SELECT name,id FROM table_name
        ```
    
    - FIND ALL COLUMNS FROM TABLE OF SPECIFIC ID

        ```SQL
            SELECT * FROM table_name WHERE id=1
        ```
    
### 6. DISTINCT statement/key word 

suppose you have to see all the citis from your database table but not the dublicate ones. Means you want to see all the unique cities in your database table. Here DISTINCT statement helps you find all the cities. It removes duplicates values.

```SQL
    SELECT DISTINCT city FROM table_name
```
    
### 7. LIMIT statement/key word 

- It helps to see specifit numbers of datas when you want to see all the data from your database table.

    ```SQL
        SELECT * FROM table_name LIMIT 5
    ```

- It helps you to see specific data list from your table as all data is 100 and you want to see number 5 to 50 all datas.

    ```SQL
        SELECT * FROM
    ```

