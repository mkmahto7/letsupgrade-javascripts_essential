# DAY 2 assignment
## Question1:
WriteaJavaScriptprogramtodisplaythecurrentdayandtimeinthefollowingformat.
SampleOutput:Todayis:Tuesday.
Currenttimeis:10PM:30:38


~~~

<!DOCTYPE html> 

<html> 

  

<head> 

    <title> 

        print current day and time 

    </title> 

</head> 

  

<body> 

    <script type="text/javascript"> 

        var myDate = new Date(); 

        var myDay = myDate.getDay(); 

        

        // Array of days. 

        var weekday = ['Sunday', 'Monday', 'Tuesday', 

            'Wednesday', 'Thursday', 'Friday', 'Saturday' 

        ]; 

        document.write("Today is : " + weekday[myDay]); 

        document.write("<br/>"); 

        

        // get hour value. 

        var hours = myDate.getHours(); 

        var ampm = hours >= 12 ? 'PM' : 'AM'; 

        hours = hours % 12; 

        hours = hours ? hours : 12; 

        var minutes = myDate.getMinutes(); 

        minutes = minutes < 10 ? '0' + minutes : minutes; 

        var myTime = hours + " " + ampm + " : " + minutes +  

            " : " + myDate.getMilliseconds(); 

        document.write("\tCurrent time is : " + myTime); 

    </script> 

</body> 

  

</html> 
~~~
## Question 2 :
Write a JavaScript program to print the contents of the current window.
~~~
<<!DOCTYPE html> 

<html> 

  

<head> 

    <title> 

        HTML | DOM Window Print() method 

    </title> 

  

    <script type="text/javascript"> 

    </script> 

  

</head> 

  

<body> 

  

    <h2>HI LETSUPGRADE USER'S</h2> 

    <form> 

        <input type="button" value="Print" 

               onclick="window.print()" /> 

    </form> 

  

</body> 

<html> 
~~~

## Question 3 :
Write a JavaScript program to get the current date.
Expected Output : mm-dd-yyyy, mm/dd/yyyy or dd-mm-yyyy, dd/mm/yyyy
create a html file

### practice.html
~~~
<!DOCTYPE html>
<html>
<head>
	<title>Java Script learning</title>

</head>
<body>
<p id="demo"></p>



<script type="text/javascript" 
	src="practice.js"> </script>
</body>
</html>
~~~
### create javascript file
~~~
var today = new Date();
var dd =today.getDate();
var mm =today.getMonth()+1;
var yyyy =today.getFullYear();
if(dd<10){
	dd ='0'+dd;
}
if(mm<10){
	mm='0'+mm;
}
today =mm+'-'+dd+'-'+yyyy;
console.log(today);

~~~
output will be
~~~
// You can print your code any one of the below format........................
01-09-2018
01/09/2018
09-01-2018
09/01/2018

~~~
