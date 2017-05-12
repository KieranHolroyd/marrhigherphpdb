You will find the meekrodb class file in the pupil shared area in the directory on the whiteboard.
Copy it into your web directory on the wamp server and add this code into a file called 'displayresults.php'

<?php include 'meekrodb.2.3.class.php';

DB::$host       = 'marr-wamp';
DB::$user       = 'YOURUSER';
DB::$password   = 'YOURPASSWORD';
DB::$dbName     = 'higher_readingdb';

$result = DB::query("SELECT * FROM displayresults ORDER BY id DESC");
$result_tree = array();

foreach ($result as $result) {
  $result_tree[$result['r1']][]=$result;
}
?>

You will then need to add in 2 foreach statements

<?php foreach ($result_tree as $result_group => $result_list) { ?>
<?php foreach ($result_list as $result) { ?>

and you will need to end both of them with this <?php } ?>

inside those brackets you can use some Mysql commands to read the data that is on the database

The current database items that can be copied are as follows:
 - r1
 - r2
 - r3
 - r4
 
 You can access them by using this php command
 <p><?php echo $result['DATABASEITEM'];?></p>
 
 and that will then make what ever item that was saved in the database for the id of the item appear on the screen
 
 example - http://marr-web/kieran/higherexample.php
 
 if there is any problems ask your teacher or contact me here
 Kieran@nitrexdesign.ga
