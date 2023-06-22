# LoginTest
 
# Steps run locally 
1. In App.config, please cset up connection peoperties properly,
   for example, in App.config there is a <appSettings> block, which is providing "keys" for connection
   		<add key="ConnectionString" value="Server=localhost;Database=gas;Uid=root;Pwd=88888888"/>
3. Run Login.cs
4. Type email and password to test.

# Changes might have to conduct on AWS DB.
Based on [to](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/create_deploy_NET.rds.html)AWS Adding an Amazon RDS DB instance to your .NET application environment
In App.config, set up properties.

# GOALS
1. Succesful Login

# DATA
It might come in handy, here is the sql create table schema and test data insert schema

## For creating table
CREATE TABLE manager_account (
  Manager_ID INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
  Email VARCHAR(100) NOT NULL,
  Password VARCHAR(45) NOT NULL
);

## For insert test data
INSERT INTO manager_account (Email, Password)
VALUES
  ('oo', 'oo'),
  ('ooo', 'ooo'),
  ('o', 'o');
