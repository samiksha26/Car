<!DOCTYPE html>
<html>
<head>
  <title>Register Form</title>
  </head>
 <body>
<h1 style="text-align: center"> List of Car Model </h1>		
<div> 
<?php
$servername = "localhost";
$username1 = "root";
$password = "";
$dbname = "my_database";


$conn = new mysqli($servername, $username1, $password, $dbname);


if ($conn->connect_error) {
    die("Connection failed: " . $conn->connect_error);
} 


$sql = "SELECT username, email,Address,City,Make,Model,Year,phone,url FROM my_guest";
$result = $conn->query($sql);

if ($result->num_rows > 0) {
    
    while($row = $result->fetch_assoc()) {
		
        echo "<br> Seller Name:- " .  $row["username"]. "  Email:-   "  .   $row["email"]  . " Address:-  " .  $row["Address"]  . " City:-  "   .   $row["City"]  .  " Vechile Make:-  "   .   $row["Make"] . " Vechile Model:-  "   .   $row["Model"]  .  "  Vechile Year:- "   .   $row["Year"] ." Phone:-  " .  $row["phone"] ;
    echo "<a href='".$row["url"]."'> ".$row["url"]." </a><br>";


}
} else {
    echo "0 results";
}

$conn->close();
?> 
</div>
 <div class="container" style="margin-left:px">

  <button  type="button" class="btn btn-dark"><a href="index.htm">Home</a></button>
  <button type="button" class="btn btn-light"><a href="form.htm">New</a></button>

</div>
</body>
</html>
