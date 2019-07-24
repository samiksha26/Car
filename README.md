# Car
index.htm
<!DOCTYPE html>
<html lang="en">
<head>
  <title>SAM</title>
  
</head>
<body>

<div class="container" style="">

  <button  type="button" class="btn btn-dark"><a href="form.htm">New</a></button>
  <button type="button" class="btn btn-light"><a href="show1.php">Search</a></button>
  
</div>

</body>
</html>


form.htm
<!DOCTYPE HTML>
<html>
<head>
  <title>Register Form</title>
  
  
</head>
<body>
<h1 style="text-align: center"> CarModels </h1>		 
 <form action="database.php" method="POST">
  <table>
   <tr>
    <td>Seller Name :</td>
    <td><input type="text" name="username" required></td>
   </tr>
   <tr>
    <td>Email :</td>
    <td><input type="email" name="email" required></td>
   </tr> 
   <tr>
    <td>Address :</td>
    <td><input type="text" name="Address" required></td>
   </tr>
   <tr>
    <td>City:</td>
    <td><input type="text" name="City" required></td>
   </tr>
   <tr>
    <td>Phone no :</td>
    <td>
    <input type="tel" pattern="^\(?(\d{3})\)?[-\. ]?(\d{3})[-\. ]?(\d{4})( x\d{4})?$" name="phone"  required>
	Acceptable formats: 123-123-1234, or (123)123-1234)
	</td>
   </tr>
    <tr>
    <td>Vechile Make :</td>
    <td><input type="text" name="Make" required></td>
   </tr>
       <tr>
    <td>Vechile Model :</td>
    <td><input type="text" name="Model" required></td>
   </tr>
       <tr>
    <td>Vechile Year :</td>
    <td><input type="Number" name="Year" required></td>
   </tr>
   <tr>
    <td><input type="submit" value="Submit"></td>
   </tr>
  </table>
 </form>
 <div class="container" style="margin-left:px">

  <button  type="button" class="btn btn-dark"><a href="index.htm">Back</a></button>
  <button type="button" class="btn btn-light"><a href="show1.php">Display</a></button>

</div>
	 
</body>
</html>
