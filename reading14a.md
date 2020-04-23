[README.MD](README.md)   
[Reference site](https://www.essentialsql.com/get-ready-to-learn-sql-database-normalization-explained-in-simple-english/)    

**Database Normalization**  
- _Database Normalization_ is a process used to organize a database into tables and columns.  The main idea with this is that a table should be about a specific topic and only supporting topics included.   
- By limiting a table to one purpose you reduce the number of duplicate data contained within your database. This eliminates some issues stemming from database modifications.  
- Three normal forms most databases adhere to using.  As tables satisfy each successive database normalization form, they become less prone to database modification anomalies and more focused toward a sole purpose or topic.   
**Reasons for Database Norm**  
- The first is to minimize duplicate data.  
- Second is to minimize or avoid data modification issues.   
- Third is to simplify queries.  
**Data Duplication and Mod Anomalies**  
- Duplicated information presents two problems.  
    - It increases storage and decreases performance.  
    - It becomes more difficult to maintain data changes.  
**Forms/ Data Norm**  
- The forms are progressive, meaning that to qualify for 3rd normal form a table must first satisfy the rules for 2nd normal form, and 2nd normal form must adhere to those for 1st normal form.  
    - _1st Norm Form_ The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.  
    -  _2nd Norm Form_ The table is in first normal form and all the columns depend on the table’s primary key.   
    - _3rd Norm Form_ The table is in second normal form and all of its columns are not transitively dependent on the primary key.   
