---
layout: post
title: Creating Mysql PHP project on Ubuntu
date: 2018-5-17
---
This using Ubuntu 12.04 to run mysql php project either by creating one or already run the project on Windows.  
These one by create it on Ubuntu.  
The project place on File System > var > www  
Create a folder there.  
For connection to mysql database file.  
config/hub.php  
<?php  
$hub = new PDO('mysql:host=localhost;
dbname=note7;charset=utf8;',
'root', 'thepswrd');  
?>  
Database name is note7 you need to create it on mysql before.  
Write the host as localhost not 127.0.0.1  
To add or insert data using prepared statement.  
op/add.php  
<?php  
$text = $_POST['text'];  

include "../config/hub.php";  

$q = $hub->prepare("insert into notes (content) values(?)");  
$q->execute( array($text) );  

if($q){  
header("Location:/opnote/");  
}  
?>  
The table inside note7 is notes. The fields are kd as int primary key auto_increment and content as text. It is wise if you want to add timestamp field.  
Showing data and the form.  
index.php  
<?php  
include "config/hub.php";  
$q = $hub->query("select * from notes");  

foreach($q as $r){ ?>  
<p>
<?php echo nl2br( $r['content'] ); ?>
</p>

<?php  
}  
?>  
<form method='POST' action='op/add.php'>  
	<textarea name='text'></textarea>  
	<input type='submit'>  
</form>  
The example above to create the mysql php project on Ubuntu should work well.
