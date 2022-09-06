#### Start server
- `sudo su -l postgres` to enter the pg shell
- `psql` to communicate with the server using `postgres` user
  
#### Database cmds
- `\l` list all the dbs 
- Create database  `CREATE DATABASE favfruit;`
- Enter database `\c favfruit`
- Create table in a db `CREATE TABLE fruit (FruitId int, FruitName char(20));`
- Insert rows in table `INSERT INTO fruit VALUES (1, 'apple'), (2, 'mango);'`
- Show table `SELECT * FROM fruit`

#### Primary key and Foreign key
- Primary - Uniqe key to indentify rows in a table
- Foreign - Relation key betweeen two tables
- Foreign key protects the inegrity of the data
- `CASCADE` means changing the primary key also changes the foreign key resp, so the relationship is maintained
   
#### schema
- To categorize database
- Default category: `public`
- Custom schema create using SQL query `CREATE SHCEMA human_resources AUTHORIZATION postgres;`   