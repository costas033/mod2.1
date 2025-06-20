<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>JavaScript Variable Demo</title>
    <script>
        // Ask the user for their first name and store it in the variable Fname
        let Fname = prompt("Please enter your first name:");

        // Display a welcome alert message that contains the name they entered
        alert("Welcome, " + Fname + "!");

        // Create the constant piValue to store the value of Pi to 7 significant digits
        const piValue = 3.1415926;

        // Ask the user to input their favorite number and store it in myFavNum
        let myFavNum = prompt("Enter your favorite number (this will be used as the radius of a circle):");

        // Convert the input to a number type
        myFavNum = parseFloat(myFavNum);

        // Calculate the area of a circle using the user's favorite number as the radius (A = πr²)
        let myArea = piValue * Math.pow(myFavNum, 2);

        // Output everything to the webpage
        document.addEventListener("DOMContentLoaded", function() {
            document.body.innerHTML += "<h2>Summary</h2>";
            document.body.innerHTML += "Hello <strong>" + Fname + "</strong>,<br>";
            document.body.innerHTML += "You entered <strong>" + myFavNum + "</strong> as your favorite number.<br>";
            document.body.innerHTML += "The constant Pi we used is <strong>" + piValue + "</strong>.<br>";
            document.body.innerHTML += "If your favorite number was the radius of a circle, the area would be <strong>" + myArea.toFixed(6) + "</strong>.";
        });
    </script>
</head>
<body>
</body>
</html>
