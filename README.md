
<html>
<head>
<title>new register Validation</title>
<script type="text/javascript">
function validate()
{
if (document.myForm.Name.value == "" )
{
alert( "Please provide your name!" );
document.myForm.Name.focus();
return false;
}
if (document.myForm.EMail.value == "" )
{
alert( "Please provide your Email!" );
document.myForm.EMail.focus() ;
return false;
}
if (document.myForm.Address.value == "" )
{
alert( "Please provide your Address!" );
document.myForm.Address.focus() ;
return false;
}
if (document.myForm.Country.value == "-1" )
{
alert( "Please provide your country!" );
return false;
}
13
if (document.myForm.Mobile.value == "" ||isNaN(
document.myForm.Mobile.value )
||document.myForm.Mobile.value.length != 10 )
{
alert ("Provide Your valid Mobile Number");
document.myForm.Mobile.focus() ;
return false;
}
alert("Registration Successful..Thank you!");
return true;
}
</script>
</head>
<body>
<h1>Welcome Guest...Register With US!!</h1><br><br>
<form action="FormValidation.html" name="myForm"
onsubmit="return validate()">
<table border="0">
<tr>
<td>Name</td>
<td><input type="text" name="Name" size="30" /></td>
</tr>
<tr>
<td>E-Mail</td>
<td><input type="text" name="EMail" size="30"/></td>
</tr>
<tr>
<td>Address</td>
<td> <textarea rows="4" cols="50"
name="Address"></textarea> </td>
</tr>
<tr>
<td>Country</td>
<td>
<select name="Country">
<option value="-1" selected>Select</option>
<option value="1">USA</option>
<option value="2">UK</option>
<option value="3">INDIA</option>
</select>
</td>
</tr>
<tr>
<td>Mobile Number</td>
14
<td><input type="text" name="Mobile" Size="30"/></td>
</tr>


<tr>
<td align="right"></td>
<td><input type="submit" value="Register" /></td>
</tr>

</table>
</form>
</body>
</html>
