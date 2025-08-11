# JavaScript
It is a scripting language which is used for client side validation of data 
### Javascript code for blank filled validation.
<!DOCTYPE html>
<html>
<head>
<script>
// check whether the fields are emptrty or not
function validateForm() {
    var x = document.forms["myForm"]["fname1"].value;
    var y = document.forms["myForm"]["fname2"].value;
    var z = document.forms["myForm"]["fname3"].value;

    if ((x==null || x=="") && (y==null || y =="")&&(z==null || z=="")) {
        alert("All fields are blank");
        document.forms["myForm"]["fname1"].focus();
        return false;//to prevent the message to go to server if the message is empty.
    }
if (x==null || x=="") {
    alert("First name missing");
    document.forms["myForm"]["fname1"].focus();
    return false;

}
if (y==null || y=="") {
    alert("You must filled the password");
    document.forms["myForm"]["fname2"].focus();
    return false;

}
if (z==null || z=="") {
    alert("Emailed must be filled out");
    document.forms["myForm"]["fname3"].focus();
    return false;
}   

}
</script>
</head>
<body>
<form name="myForm" action="" onsubmit="return validateForm()" method="post">
    First name:<input type="text" name="fname1">
    Password:<input type="password" name="fname2">
    Email:<input type="text" name="fname3">
    <input type="submit" value="Submit">
    <input type="reset" value="Reset">
</form>
</body>
</html>


### JS code for no. validation.
<html>
<head>
<script>
    function check(){
         var y=document.forms["myForm"]["fname2"].value;
         if (isNaN(y)==true || y==null || y=="") {
            alert("enter a valid age");
            document.forms["myForm"]["fname2"].value="";
            document.forms["myForm"]["fname2"].focus();
            return false;

         }
    }
</script>
</head>
<body>
    <form name="myForm" action="" onsubmit="return check()" method="post">
        Age:<input type="text" name="fname2">
        <input type="submit" value="Submit">
        <input type="reset" value="Reset">
    </form>
</body>
</html>


## js code for email validation
/^\w+([\.-]?\w+)@(\w+([\.-]?\w+))(\.\w{2,3})+$/;
1. /...../ this is entire statement.
2. ^: this represents the starting wword of the statement.
3. \: this means followed by
4. w: any alphanumeric word.
5. +: means occurence of the alphanumeric word multiple times.
6. .- :this represents dot or hypen or underscore
7. ? :repetations of special character multiple times 
8. *: repetations of special characters and alphanumeric words together multiple times 
9. @ : this character shold be there.
10. w{2,3}: this represents alpha numeric word of 2 to 3 characters long.
11. $: last word of your emailid.



#### js code for password and confirm password
## jdbc
jdbc stands for java database connectivity.
it is an api using which we can connect our java application to a particular database.
database- A database is a file which is used to store interrelated data together.
## DBMS(data base management system)
IT is a software using which we can manipulate the data stored in the database. e.g.-oracle,mySql,Db2
## RDBMS(relational data base management system):
RDBMS stands for relational data base management system. In this all the data are stored in tabular form. The term relation refers to table. The rows in a table are called as tuples and the columns in the tables are called fields or attributes or keys.
primary key: The columns which contains unique data elements are also termed as primary key. In primary key column we cannot have a null value.
Unique key:  It contains unique value and it also have null value.
Foreign key: If a primary key column of one table is present in another table than in the second table that column is called a foreign key.

### Steps for performing JDBC:
1. create a table which consists of blank fields.
2. Add Appropriate type 4 driver.
3. Write appropriate sql query in order to manipulate the data stored in the database. 


there are four types of sql query for dml
1. Insert
2. Update
3. Delete
4. fetch