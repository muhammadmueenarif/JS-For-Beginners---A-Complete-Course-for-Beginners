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

