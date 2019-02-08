Steps for accesing postgres database


1) Install pgadmin 4
https://www.pgadmin.org/download/pgadmin-4-windows/

2)In Pgadmin right click on servers > create > server

3) Provide database credentials

Host: ec2-23-21-86-22.compute-1.amazonaws.com
Database: de4jd0oee0au85
User: uevppsjaeearhc
Port: 5432
Password: 873cb39d89d29529ff3e8c943b81e3d3b3cabb22f75ad6023c2821e3c0209a00

4)search for database in given list of databases

5)Click on databse >schemas

6) From here you can access create, update, delete, fetch table/s 

=============================================================================================================================

INSERT INTO "Test" VALUES
    ('https://s3-us-west-1.amazonaws.com/visitor-management-app/tree.jpg');


    select * from salesforce.development__c;


/*pool.query('SELECT * FROM salesforce.development__c', (err, res) => {
              
              //console.log(err, res);
              console.log('error'+err);
              console.log('res salesforce------------'+JSON.stringify(res));
              pool.end()
            })*/


UPDATE films SET kind = 'Dramatic' WHERE kind = 'Drama';

//Change datatype of column

ALTER TABLE the_table ALTER COLUMN col_name TYPE integer USING (col_name::integer);

for displayig no of connections on heroku
heroku pg:ps

To kill connections
heroku pg:kill process number


To kill all connections

heroku pg:killall
//to get last insert ID

https://stackoverflow.com/questions/2944297/postgresql-function-for-last-inserted-id

