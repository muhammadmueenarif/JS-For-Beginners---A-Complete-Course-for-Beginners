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


lec 43. Objects.

        var a= {
            name:"ali",
            class: "one",
            subj: "comp", 
            marks: "50"
        };
        document.write(a.subj);

now let's see how to pass function in array. and how to access it. 

 var a= {
            name:"ali",
            class: "one",
            subj: "comp", 
            marks: "50",
            friends:["ahsan", "umer", "usama", "saad", "haris"],

            income: function () {
                return 25000;
            },

        };
        document.write(a.income());

now this keyword. 
when we need to call any argument in object, we use this keyword in that function.

if we want to call a function in an object and return value of function by object then we use this
keyword. if we do not use this, it will show error. 

   var a= {
            name:"ali",
            class: "one",
            subj: "comp", 
            marks: "50",
            friends:["ahsan", "umer", "usama", "saad", "haris"],

            income: function () {
                return 25000;
            },

            Fun: function () {
                return this.name + " " + this.class; 
            }
        };
        document.write(a.Fun());


lec 44. array as object.
    var hello= [
        {
        name:"ali",
        age:"22"
    },
    {
        name:"kashan",
        age:"12"
    },
    {
        name:"haider",
        age:"25"
    },
    {
        name:"usman",
        age:"20"
    }
];
     console.log(hello);

we can use for loop on it as well. 
    var hello= [
        {
        name:"ali",
        age:"22"
    },
    {
        name:"kashan",
        age:"12"
    },
    {
        name:"haider",
        age:"25"
    },
    {
        name:"usman",
        age:"20"
    }
];
     for (var a=0; a<hello.length; a++) {
        document.write(hello[a].name + " " + hello[a].age + "<br/>");
     }

using for in loop. 

    var a=         
    {
        name:"ali",
        age:"22",
        class:"two",    
    };
     
    for(var key in a) {
        document.write(key + ": " + a[key] + "<br/>");
     }


lec 45. string and methods.
length, tolowercase, touppercase, includes, startswith, endswith, search, match, indexof, lastindexof, 
replace, trim, charat, concat, split, repeat, slice, substr, substring.

.length tells length of string. 
.tolowercase
.touppercase
.includes
.startswith
.endswith
.search. it gives index of particular character. if there are two characters like d used 2 times, 
it will show last index where d is used last time. 

.match. 
it will tell whether given character is in string or not. /g means global. whole string. 
var a= "Javascript is great language";
   var b= a.match(/a/g);
   document.write(b);
// this will give a as many time as it is used. a,a,a,a,a. 

.indexOf used to check index of word. like indexOf(is); //11. it gave where is used 1st time.
.lastIndexOf(is); //22 because used at 22 last time. 

.replace. this will replace is with are but only 1st. if we want to change all is to are, then use /is/g, "are";

var a= "Javascript is great language";
   var b= a.replace("is", "are");
   document.write(b);

.trim. if there are empty spaces at start of string then use this. 
.charat shows what character is that index. 
.charcodeat. it will show ascii code of that character. 
.fromcharcode. we enter ascii code and it shows the corresponding number. 
.concat. used to join string.
.split. used to split the string.
var a= "Javascript is great language";
   var b= a.split("i");
   document.write(b);
// it will split from all i in the string. 

.repeat. used to repeat string. a.repeat(5). it will print 5 times. 

.slice. a.slice(3). it will not print first 3 letters and print all till end. 
a.slice(1,6); from 1 to 5. not include 6.  

.substr. it will work like slice but it will include last value also. 
.tostring. it will convert any value to string data type. 


lec 46. number methods.

        var a= "100";
        var b= Number(a);
        document.write(b);
// coverted data type into number. 

.parseint. this will convert to int. 
.parsefloat. it will display in points. 
.isfinite. it will return true or false, it will tell whether number is finite or not.
        var a= 100;
        var b= isFinite(a);
        document.write(b);

.isinteger. it will tell whether number is integer or not. return true or false.
.tofixed. it will specify how many values shown after points, 

        var a= 100.23863490;
        var b= a.toFixed(3);
        document.write(b);

.toPrecision. same as tofixed. it will roundoff. 

        var a= 20.35768;
        var b= a.toPrecision(3);
        document.write(b); //20.4 output

lec 47. math methods. 
ceil, floor, round, trunc, max, min, sqrt, cbrt, pow, random, abs, pi.

.ceil. it shows upper value. 
var a= math.ceil(5.66); //6

.floor. it shows lower value.
var a= math.floor(7.56); //7

.round. it will roundoff.
var a= math.round(5.66); //6

.trunc. it will remove decimal part.
var a= math.trunc(5.66); //5

.max. it will show maximum value.
var a= math.max(5,6,7,8); //8

.min. it will show minimum value.
var a= math.min(5,6,7,8); //5

.sqrt. it will show square root.
var a= math.sqrt(25); //5

.cbrt. it will show cube root.
var a= math.cbrt(27); //3

.pow. it will show power. 2 values need. 1 is base, 2 is exponent.
var a= math.pow(2,3); //8

.random. it will show random value between 0 and 1.
var a= math.random(); //0.23456

.abs. it will show absolute value.
var a= math.abs(-5); //5

.pi. it will show pi value.
var a= math.pi; //3.14159



lec 48. date methods.
todatestring, getdate, getfullyear, getmonth, getday, gethours, getminutes, getseconds,
getmilliseconds, setdate, setfullyear, sethours, setmilliseconds, setminutes. 

new date(). it will show current date and time.
var a= new date();
document.write(a);
//output: current date and time. 

.getdate. it will show date.
var a= new date();
var b= a.getdate();
document.write(b);
//output: current date.

.getfullyear. it will show full year.
var a= new date();
var b= a.getfullyear();
document.write(b);
//output: current year.

.gethours. it will show hours.
var a= new date();
var b= a.gethours();
document.write(b);
//output: current hours.

.getmonth. it will show month. (0-11)
var a= new date();
var b= a.getmonth();
document.write(b);
//output: current month. (0-11)

.getseconds. it will show seconds.
var a= new date();
var b= a.getseconds();
document.write(b);
//output: current seconds.

.setdate. it will set date.
var a= new date();
a.setdate(25);
document.write(a);
//output: current date and time with date 25.

.setfullyear. it will set full year.
var a= new date();
a.setfullyear(2025);
document.write(a);
//output: current date and time with year 2025.

.sethours. it will set hours.
var a= new date();
a.sethours(12);
document.write(a);
//output: current date and time with hours 12.

.setminutes. it will set minutes.
var a= new date();
a.setminutes(30);
document.write(a);
//output: current date and time with minutes 30.

.setseconds. it will set seconds.
var a= new date();
a.setseconds(45);
document.write(a);
//output: current date and time with seconds 45.

.todatestring. it will show date in local format.
var a= new date();
document.write(a.todatestring());
//output: current date in local format.


Lec 49. DOM Model
Lec 50. DOM Other Objects.
We can target using id, class, and tag name. 
document.getelementbyid. document.getelementbyclassname. document.getelementbytagname. 

Lec 51. DOM Get methods.
.innertext, innerhtml, getattribute, getattributenodes, attributes.

.innertext
var a= document.getelementbyid("id");
document.write(a.innertext);
//output: text inside the element.

.innerhtml
var a= document.getelementbyid("id");
document.write(a.innerhtml);
//output: html inside the element.

.getattribute
var a= document.getelementbyid("id");
document.write(a.getattribute("class"));
//output: class attribute value.

.getattributenodes
var a= document.getelementbyid("id");
document.write(a.getattributenodes("style"));
//output: class attribute node.
this is not recommended to use. 

Lec 52. DOM Styling. 
var element;
element= document.queryselector("id").style.border;
console.log(element);
// it will show border if it has. //2px solid black.

if we want to change, then we will use 
element= document.queryselector("id").style.border= "2px solid red";

document.queryselector("id").classlist.add(header); // it will add class.
document.queryselector("id").classlist.remove(header); // it will remove class.

Lec 53. events and add events listener. 
onclick, onload. we discussed these in other videos. 
now add event listener.

document.getelementbyid("header").addeventlistener("click", function(){
    console.log("you clicked me");
    });
    
    // it will show message in console when we click on the element.
if you want to change background color or apply any other property using js, then you can do it also.


Lec 54. useCapture. 
it is only true or false. if we do not want to use any event then we use this. below is example.
for example we have one outer and one inner box. when we click on outer box, it alert inner box. 
but when we click on inner box, it first shows outer box then alert inner box. we want that when we 
click inner box, it should not alert outer box but only alert inner box. 
then we use useCapture.

document.queryselector(".inside").addeventlistener("click", function(params) {
    alert("this is inner box");
}, false
);

document.queryselector(".outside").addeventlistener("click", function(params) {
    alert("this is outside box");
}, false
);


Lec 55. classList Method.
if we create new class in css and want to add it in html respected tag, we can do this. 
    var news;
    document.getelementbyid("header").addeventlistener("click", fun);
    function fun (params) {
    document.getelementbyid("header").classList.add("newclass");
    }
// it will add newclass in header tag.
we can add multiple classes also by using ,. 

we can remove class also.
document.getelementbyid("header").classList.remove("newclass");

var again = document.getelementbyid("header").classList.length;
console.log(again);
// it will show how many classes are there in header tag.

var again = document.getelementbyid("header").classList.item(0);
console.log(again);
// it will show first class of header tag.

var again = document.getelementbyid("header").classList.contains("newclass");
console.log(again);
// it will show true or false whether newclass is there or not.

var again = document.getelementbyid("header").classList.toggle("newclass");
console.log(again);
// it will add class if it is not there and remove if it is there.


Lec 56. Parent Nodes
DOM Traversal methods. 
ParentNode. ParentElement. firstChild. firstElementChild. Children. childNodes. LastChild. 
lastElementchild. nextElementSibling, nextSibling, previousElementSibling, previousSibling, Document.domain

var one = document.getelementbyid("header").ParentElement;
console.log(one);
// it will show parent element of header tag.

var one= document.getelementbyid("header").ParentElement.style.background= "red";
console.log(one);
// it will change background color of parent element of header tag.


var one = document.getelementbyid("header").ParentNode;
console.log(one);
// it will show parent node of header tag.

var one = document.getelementbyid("header").firstChild;
console.log(one);
// it will show first child of header tag.

var one = document.getelementbyid("header").firstElementChild;
console.log(one);
// it will show first element child of header tag.

var one = document.getelementbyid("header").Children;
console.log(one);
// it will show all children of header tag.


var one= document.getelementbyid("header").Children[5];
console.log(one);
// it will show 5th child of header tag. it will show undefined error if there is no 5th child.

var one= document.getelementbyid("header").Children[2].style.background="blue";
// it will change background color of 2nd child of header tag.

var one = document.getelementbyid("header").childNodes;
console.log(one);
// it will show all child nodes of header tag.


var one = document.getelementbyid("header").childNodes[2].innerhtml;
console.log(one);
// it will show innerhtml of 2nd child node of header tag.


var one = document.getelementbyid("header").LastChild;
console.log(one);
// it will show last child of header tag.

var one = document.getelementbyid("header").lastElementChild;
console.log(one);
// it will show last element child of header tag.

var one = document.getelementbyid("header").nextElementSibling;
console.log(one);
// it will show next element sibling of header tag.

var one = document.getelementbyid("header").nextSibling;
console.log(one);
// it will show next sibling of header tag.

var one = document.getelementbyid("header").previousElementSibling;
console.log(one);
// it will show previous element sibling of header tag.

var one = document.getelementbyid("header").previousSibling;
console.log(one);
// it will show previous sibling of header tag.

var one = document.domain;
console.log(one);
// it will show domain of the document.

// Note: These methods are used to traverse the DOM tree. They are used to navigate through the
elements of the document. They are used to get the parent, child, sibling elements of a
particular element.


Lec 57. Create Element Text Node

var element=  document.createElement("h3");
console.log(element);
// it will create a new h3 element in html.

var element2=  document.createTextNode("Kashan Moin");
console.log(element);
// it will create a new text node with the text "Kashan Moin".

var element3=  document.createComment("This is JS Comment");
console.log(element);
// it will create a new comment node with the text "This is JS Comment".


Lec 58. Append child and insert before.
var parent = document.getElementById("header");
var child = document.createElement("h3");
child.textContent = "Kashan Moin"
parent.appendChild(child);
// it will append the child element to the parent element.

var target = document.getelementbyid("new");
target.insertBefore(element.target.childNodes);
// it will insert the element before the target element.

target.insertBefore(element.target.childNodes[4]);
// it will insert the element before the target element's 4th child node.


Lec 59. insert adjacent element and insert adjacent html.

appendChild and insertBefore methods only append.
insert adjacent element, insert adjacent html and insert adjacent text create and append. 

insertadjacentelement will use tag. <p></p>
insertadjacenttext will use textcontent. "this is text"
insertadjacenthtml will use innerhtml. <p>text</p>

    DOM insertAdjacent positions
    1.Beforebegin
    2.Afterbegin
    3.beforeend
    4.afterend

var element= document.createElement("h1");
var text= document.createTextNode("Kashan Moin");
var target= document.getElementById("div");
target.insertadjacentelement("Beforebegin", element);
//it will write before div


target.insertadjacentelement("Afterbegin", element);
//it will write after div

target.insertadjacentelement("Beforeend", element);
//it will write before div's end

target.insertadjacentelement("Afterend", element);
//it will write after div's end


var target= document.getelementbyid("div");
var element1= "<h2>Kashan Moin</h2>";
target.insertadjacenthtml("afterend", element1);

