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