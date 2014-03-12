phpdatabasedriver
=================

PHP MySQL Database Driver with chaining capabilities.

Works similar to CodeIgniters database driver.

#####Instructions:

Enter database credentials in database.config.php

Open database.php and make sure the config file is being referenced correctly in the constructor.

Include the file via require()
require('path/to/database.php');

#####Initialize the object
$db = new Database();

#####Read through the file to pull all functions. Here are some of the more common ones:

#####Selecting from a table
$results = $db->select(['fieldname','anotherfieldname])->from('tablename')->get();

#####Selecting all from a table
Method one - with select()
$results = $db->select('*')->from('tablename')->get();

Method two - with selectAllFrom()
$results = $db->selectAllFrom('tablename')->get();

#####Updating a record
$db->update('tablename',['columnname'=>'columnvalue']);

