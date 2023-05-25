# simple-phone-credit-app
DB: sqlite3
Program Language: PHP

# What I Do:
1. Create Database: sqlite3 <db-name>
2. Create Table:

CREATE TABLE data (                                                                            
id INTEGER NOT NULL PRIMARY KEY AUTOINCREMENT,                                                 
phone_number TEXT NOT NULL,                                                                    
product TEXT NOT NULL,                                                                         
package TEXT NOT NULL,                                                                         
date_time DATETIME DEFAULT (datetime('now','localtime')) 
);

3. Insert Data to Table:

insert into data ( phone_number, product, package ) values ( '+6281230010399', 'P', '50000' );

4. Show Table Data:

select * from <table-name>

5. sqlite3 command:
.schema <table-name> to see the table schema
.tables to see the table list 
.mode <column-or-list> to set the sqlite view mode column or list
.quit to quit the sqlite3
.header <on-or-off> to show or hide the table header
