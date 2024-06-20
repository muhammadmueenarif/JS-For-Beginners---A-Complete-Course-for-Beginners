lec 01. intro and history.
lec 02. basic syntax.
lec 03. js implementation. 
lec 04. how to use html tags in js.
        document.write("<h1>Hy</h1>");

2nd method
var first = "<h1>How are you</h1>";
        document.write(first);

lec 05. var in js. 
let block scope. var global. const fixed. cannot be changes. 

lec 06. local and global variables.
lec 07. console.
console.log, .error, .table, .warn.
console.time at start of code and console.end at end of code. it will tell time taken.

lec 08. if statement.
lec 09. if else. 
lec 10. ternary operator.
lec 11. switch. 
lec 12. if else if. 
lec 13. break and continue. 

lec 14. data types. 

        var x= "hello world"; string
        var y=30. number 
        var z= true; boolean
        var arr = ["html", "css", "js"]; array
        var obj= { "name":"ali", "age":"25", "subj":"comp" } object
        var a; undefined
        var b= null; null

lec 15. arithmatic operators. 
+, -, *, /, %, ++, --, 

lec 16. assignment operator.
=, +=. -=, *=, /=, %=. 

lec 17. comparison operator.
==, ===, !=, !==, >, <, >=, <=.

lec 18. alert 
to show an alert message.
alert("how are you"). we can set condition of if also and show output in alert. 

lec 19. confirm box.
used for 2 options. 
var a= confirm("are you robot");
        if(a) {
            alert("thanks");
        }
        else {
            alert("its ok");
        }
this will give two choices. cancel and ok. 

lec 20. prompt box. 
used to get some input from user. 
        prompt("enter something");

lec 21. functions.
lec 22. function with parameter. 
lec 23. function with return.
lec 24. events in js. 

lec 25. loops. while loop. 
lec 26. do while. 
lec 27. for loop.
lec 28. nested loop. 
lec 29. arrays. 
lec 30. modify and delete arrays. 
lec 31. sort and reverse. 
lec 32. pop and push.
lec 33. shift and unshift. 
lec 34. concat and join. 
lec 35. slice and splice. 

lec 36. isArray method. 
it tells whether the passed value is array or not. 
var a= [10, 20, 30];
      var b= Array.isArray(a);
      document.write(b);

use if condition and show output it is an array if given value is array. else show not an array.


lec 37. indexof and lastindex methods. 

 var a =["ali", "ahsan", "nawaz", "umer", "haider"];
    var b= a.indexOf("ali");
    document.write(b);
// this will show index of ali. 0.

var a =["ali", "ahsan", "nawaz", "umer", "ali", "haider"];
    var b= a.lastIndexOf("ali");
    document.write(b);
// this will show last index of ali. that is 4.

lec 38. foreach.
this will work with array.
 var name= ["ali", "nawaz", "umer", "hassan", "kashan"];
    name.forEach(loop);
    function loop(value, index) {
        document.write(index + " " + value + "<br>");
    }

this code is not working. don't know why. 


lec 38. tostring, valueof, and fill methods. 

.tostring is used to change array into string. when we change array into string, we cannot use array
methods on it.
 var a= [10, 20, 30, 40, 50];
    document.write("Original Array: " + a + "<br>");
    a.toString();
    document.write("Array to String: " + a + "<br>");

.valueof is used to print the values of array. it does not work with specific index but full array. 

.fill method will write that word in full array. 
 var a= [10, 20, 30, 40, 50];
        a.fill("Hy");
        document.write(a);
it will print hy five times instead of assigned values.


lec 39. include method.
it is used when we create lengthy array and forget which value we used or not.
 var a= [10,20,30,40,50,60,70,80,90,100];
   document.write(a.includes(10));
// it will show true.


lec 40. some and every method.
it is used when we make arrays and want to check values in these arrays. it works with a function.

   var a= [10,20,30,40,50,60,70,80,90,100];
   document.write(a+ "<br/>");
   var b= a.some(checkvalue);
   document.write(b + "<br/>");
   function checkvalue(age) {
    return age>=18;
   }

it will check if there is value > 18 in the array and return true. else false. 

lec 41. find and findindex methods.
 var a= [10,20,30,40,50,60,70,80,90,100];
   document.write(a+ "<br/>");
   var b= a.find(checkvalue);
   document.write(b + "<br/>");
   function checkvalue(age) {
    return age>=18;
   }
find and findindex are same. find give us value but findindex give us index of that value.


lec 42. filter method. 
find and some gives only one first value in output. but filter will show all the values in output.

 var a= [10,20,30,40,50,60,70,80,90,100];
   document.write(a+ "<br/>");
   var b= a.filter(checkvalue);
   document.write(b + "<br/>");
   function checkvalue(age) {
    return age>=18;
   }

