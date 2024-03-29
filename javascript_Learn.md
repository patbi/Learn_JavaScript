# JavaScript Learn

## Mentor Patrick BIYAGA Course 

> Resume JavaScript W3Schools for the Program | ALC - Facilitator on on the Google mobile web specialist track 2019 for learners.

Website For Learn - https://www.w3schools.com/js/js_intro.asp

## JavaScript language
* JavaScript is the programming language of HTML and the Web.
* JavaScript is easy to learn.
* This tutorial will teach you JavaScript from basic to advanced.

>We will learn while having fun

```bash
# My First JavaScript

<html>
<body>
  <h2>My First JavaScript</h2>
  <button type="button"
      onclick="document.getElementById('demo').innerHTML = Date()">
      Click me to display Date and Time.
  </button>
  <p id="demo"></p>
</body>
</html> 

# Why Study JavaScript?

* HTML to define the content of web pages.
* CSS to specify the layout of web pages.
* JavaScript to program the behavior of web pages.

Web pages are not the only place where JavaScript is used. Many desktop and server programs use JavaScript. Node.js is the best known. Some databases, like MongoDB and CouchDB, also use JavaScript as their programming language.
```

## JavaScript Can Change HTML Content

One of many JavaScript HTML methods is getElementById().

This example uses the method to "find" an HTML element (with id="demo") and changes the element content (innerHTML) to "Hello JavaScript":

```bash
<!DOCTYPE html>
<html>
<body>
  <h2>What Can JavaScript Do?</h2>
  <p id="demo">JavaScript can change HTML content.</p>
  <button type="button" onclick='document.getElementById("demo").innerHTML = "Hello JavaScript!"'>Click Me!
  </button>
</body>
</html>
```


## JavaScript Can Change HTML Attribute Values

In this example JavaScript changes the value of the src (source) attribute of an <img> tag:


```bash
<!DOCTYPE html>
<html>
<body>
  <h2>What Can JavaScript Do?</h2>
  <p>JavaScript can change HTML attribute values.</p>
  <p>
    In this case JavaScript changes the value of the src (source) attribute of an image.
  </p>
  <button onclick="document.getElementById('myImage').src='pic_bulbon.gif'">
    Turn on the light
  </button>
  <img id="myImage" src="pic_bulboff.gif" style="width:100px">
  <button onclick="document.getElementById('myImage').src='pic_bulboff.gif'">
    Turn off the light
  </button>
</body>
</html>
```


## JavaScript Can Change HTML Styles (CSS)

Changing the style of an HTML element, is a variant of changing an HTML attribute:


```bash
<!DOCTYPE html>
<html>
<body>
  <h2>What Can JavaScript Do?</h2>
  <p id="demo">JavaScript can change the 
    style of an HTML element.
  </p>
  <button type="button" onclick="document.getElementById('demo').style.fontSize='35px'">Click Me!
  </button>
</body>
</html> 
```


## JavaScript Can Hide HTML Elements

Hiding HTML elements can be done by changing the display style:


```bash
<!DOCTYPE html>
<html>
<body>
  <h2>What Can JavaScript Do?</h2>
  <p id="demo">
    JavaScript can hide HTML elements.
  </p>
  <button type="button" onclick="document.getElementById('demo').style.display='none'">
    Click Me!
  </button>
</body>
</html> 
```


## JavaScript Can Show HTML Elements

Showing hidden HTML elements can also be done by changing the display style:


```bash
<!DOCTYPE html>
<html>
<body>
  <h2>What Can JavaScript Do?</h2>
  <p>JavaScript can show hidden 
    HTML elements.
  </p>
  <p id="demo" style="display:none">
    Hello JavaScript!
  </p>
  <button type="button" onclick="document.getElementById('demo').style.display='block'">
    Click Me!
  </button>
</body>
</html>  
```


## JavaScript Where To
* JavaScript in head or body.

You can place any number of scripts in an HTML document.
Scripts can be placed in the <body>, or in the <head> section of an HTML page, or in both.


* External JavaScript.

Scripts can also be placed in external files



## JavaScript in head

In this example, a JavaScript function is placed in the <head> section of an HTML page.

The function is invoked (called) when a button is clicked:


```bash
<!DOCTYPE html>
<html>
<head>
<script>
  const myFunction = _=> {
    document.getElementById("demo").innerHTML = "Paragraph changed.";
  }
</script>
</head>
<body>

<h1>A Web Page</h1>
<p id="demo">A Paragraph</p>
<button type="button" onclick="myFunction()">
    Try it
</button>

</body>
</html> 
```


## JavaScript in body

In this example, a JavaScript function is placed in the <body> section of an HTML page.

The function is invoked (called) when a button is clicked:


```bash
<!DOCTYPE html>
<html>
<body>

<h1>A Web Page</h1>
<p id="demo">A Paragraph</p>
<button type="button" onclick="myFunction()">Try it</button>

<script>
const myFunction = _=> {
    document.getElementById("demo").innerHTML = "Paragraph changed.";
  }
</script>

</body>
</html>
```


## External JavaScript

Scripts can also be placed in external files:


```bash
External JavaScript in myScript.js
<script>
const myFunction = _=> {
    document.getElementById("demo").innerHTML = "Paragraph changed.";
  }
</script>


<!DOCTYPE html>
<html>
<body>

  <h2>External JavaScript</h2>

  <p id="demo">A Paragraph.</p>

  <button type="button" onclick="myFunction()">Try it</button>

  <p>(myFunction is stored in an external file called "myScript.js")</p>

<script src="myScript.js"></script>

</body>
</html>
```


# External JavaScript Advantages

* It separates HTML and code.
* It makes HTML and JavaScript easier to read and maintain.
* Cached JavaScript files can speed up page loads.



## JavaScript Output | JavaScript Display Possibilities

JavaScript can "display" data in different ways:

* Writing into an HTML element, using innerHTML.
* Writing into the HTML output using document.write().
* Writing into an alert box, using window.alert().
* Writing into the browser console, using console.log().


## Using innerHTML

To access an HTML element, JavaScript can use the document.getElementById(id) method.

The id attribute defines the HTML element. The innerHTML property defines the HTML content:


```bash
<!DOCTYPE html>
<html>
<body>

  <h1>My First Web Page</h1>
  <p>My First Paragraph</p>

  <p id="demo"></p>

<script>
  document.getElementById("demo").innerHTML = 5 + 6;
</script>

</body>
</html>
```

## Using document.write()

For testing purposes, it is convenient to use document.write():


```bash
<!DOCTYPE html>
<html>
<body>

  <h1>My First Web Page</h1>
  <p>My first paragraph.</p>

<script>
  document.write(5 + 6);
</script>

</body>
</html>
```


## Using window.alert()

You can use an alert box to display data:


```bash
<!DOCTYPE html>
<html>
<body>

  <h1>My First Web Page</h1>
  <p>My first paragraph.</p>

<script>
  window.alert(5 + 6);
</script>

</body>
</html>
```


## Using console.log()

For debugging purposes, you can use the console.log() method to display data.


```bash
<!DOCTYPE html>
<html>
<body>

<script>
  console.log(5 + 6);
</script>

</body>
</html>
```


## JavaScript Statements

JavaScript statements are composed of:

Values, Operators, Expressions, Keywords, and Comments.

This statement tells the browser to write "Hello Dolly." inside an HTML element with id="demo":



```bash
<script>
  document.getElementById("demo").innerHTML = "Hello Dolly.";
</script>
```


* Semicolons ;

```bash
let a, b, c;     // Declare 3 variables
a = 5;           // Assign the value 5 to a
b = 6;           // Assign the value 6 to b
c = a + b;       // Assign the sum of a and b to c
```

When separated by semicolons, multiple statements on one line are allowed:


```bash
a = 5; b = 6; c = a + b;
```

* JavaScript White Space

JavaScript ignores multiple spaces. You can add white space to your script to make it more readable.

The following lines are equivalent:


```bash
const person = "Hege";
const person="Hege";
```

A good practice is to put spaces around operators ( = + - * / ):


```bash
const x = y + z;
```



* JavaScript Line Length and Line Breaks

For best readability, programmers often like to avoid code lines longer than 80 characters.

If a JavaScript statement does not fit on one line, the best place to break it is after an operator:


```bash
<script>
  document.getElementById("demo").innerHTML =
  "Hello Dolly!";
</script>
```


* JavaScript Code Blocks

JavaScript statements can be grouped together in code blocks, inside curly brackets {...}.

The purpose of code blocks is to define statements to be executed together.

One place you will find statements grouped together in blocks, is in JavaScript functions:


```bash
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Statements</h2>

<p>JavaScript code blocks are written between { and }</p>

<button type="button" onclick="myFunction()">Click Me!</button>

<p id="demo1"></p>
<p id="demo2"></p>

<script>
const myFunction = _=> {
  document.getElementById("demo1").innerHTML = "Hello Dolly!";
  document.getElementById("demo2").innerHTML = "How are you?";
}
</script>

</body>
</html>
```


## JavaScript Syntax

JavaScript syntax is the set of rules, how JavaScript programs are constructed:

```bash
let x, y, z;          // How to declare variables
x = 5; y = 6;      // How to assign values
z = x + y;         // How to compute values
```

* JavaScript Values

The JavaScript syntax defines two types of values: Fixed values and variable values.

Fixed values are called literals. Variable values are called variables.


* JavaScript Literals


The most important rules for writing fixed values are:

Numbers are written with or without decimals:The most important rules for writing fixed values are:

Numbers are written with or without decimals:


```bash
<!DOCTYPE html>
<html>
<body>
  <h2>JavaScript Numbers</h2>

  <p>Number can be written with or without decimals.</p>

  <p id="demo"></p>
<script>
  document.getElementById("demo").innerHTML = 19.50;
</script>

</body>
</html>
```

Strings are text, written within double or single quotes:


```bash
<!DOCTYPE html>
<html>
<body>
  <h2>JavaScript Strings</h2>

  <p>Strings can be written with double or single quotes.</p>

  <p id="demo"></p>
<script>
  document.getElementById("demo").innerHTML = 'Patrick BIYAGA';
</script>

</body>
</html>
```

* JavaScript Variables

In a programming language, variables are used to store data values.

JavaScript uses the var keyword to declare variables.

An equal sign is used to assign values to variables.

In this example, x is defined as a variable. Then, x is assigned (given) the value 4:


```bash
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Variables</h2>

<p>In this example, x is defined as a variable.
Then, x is assigned the value of 4:</p>

<p id="demo"></p>

<script>
  let x;
  x = 4;
  document.getElementById("demo").innerHTML = x;
</script>

</body>
</html>
```


* JavaScript Operators

JavaScript uses arithmetic operators ( + - * / ) to compute values:



```bash
<!DOCTYPE html>
<html>
<body>
<h2>JavaScript Operators</h2>

<p>JavaScript uses arithmetic operators to compute values (just like algebra).</p>

<p id="demo"></p>

<script>
  document.getElementById("demo").innerHTML = (5 + 6) * 10;
</script>

</body>
</html>
```

JavaScript uses an assignment operator ( = ) to assign values to variables:



```bash
<!DOCTYPE html>
<html>
<body>

<h2>Assigning JavaScript Values</h2>

<p>In JavaScript the = operator is used to assign values to variables.</p>

<p id="demo"></p>

<script>
  let x, y;
  x = 10;
  y = 9;
  document.getElementById("demo").innerHTML = x + y;
</script>

</body>
</html>
```


* JavaScript Expressions

An expression is a combination of values, variables, and operators, which computes to a value.

The computation is called an evaluation.

For example, 5 * 4 evaluates to 20:


```bash
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Expressions</h2>

<p>Expressions compute to values.</p>

<p id="demo"></p>

<script>
  document.getElementById("demo").innerHTML = 5 * 4;
</script>

</body>
</html>
```

Expressions can also contain variable values:


```bash
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Expressions</h2>

<p>Expressions compute to values.</p>

<p id="demo"></p>

<script>
  let x;
  x = 4;
  document.getElementById("demo").innerHTML = x * 10;
</script>

</body>
</html>
```

The values can be of various types, such as numbers and strings.

For example, "Patrick" + " " + "BIYAGA", evaluates to "Patrick BIYAGA":


```bash
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Expressions</h2>

<p>Expressions compute to values.</p>

<p id="claire"></p>

<script>
  document.getElementById("claire").innerHTML = "Patrick" + " "  + "BIYAGA";
</script>

</body>
</html>
```

* JavaScript Keywords

JavaScript keywords are used to identify actions to be performed.

The let keyword tells the browser to create variables:

```bash
<!DOCTYPE html>
<html>
<body>

<h2>The var Keyword Creates Variables</h2>

<p id="pat"></p>

<script>
  let x, y;
  x = 5 + 6;
  y = x * 10;
  document.getElementById("pat").innerHTML = y;
</script>

</body>
</html>
```

* JavaScript Comments  ## JavaScript Syntax

Not all JavaScript statements are "executed".

Code after double slashes // or between /* and */ is treated as a comment.

Comments are ignored, and will not be executed:

```bash
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Comments are NOT Executed</h2>

<p id="demo"></p>

<script>
  let x;
  x = 5;
  // x = 6; I will not be executed
  document.getElementById("demo").innerHTML = x;
</script>

</body>
</html>
```

* JavaScript Identifiers

Identifiers are names.

In JavaScript, identifiers are used to name variables (and keywords, and functions, and labels).

The rules for legal names are much the same in most programming languages.

In JavaScript, the first character must be a letter, or an underscore (_), or a dollar sign ($).

Subsequent characters may be letters, digits, underscores, or dollar signs.


* JavaScript is Case Sensitive

All JavaScript identifiers are case sensitive. 

The variables lastName and lastname, are two different variables:


```bash
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript is Case Sensitive</h2>

<p>Try change lastName to lastname.</p>

<p id="demo"></p>

<script>
  let lastname, lastName;
  lastName = "Claire";
  lastname = "Marie";
  document.getElementById("demo").innerHTML = lastName;
</script>

</body>
</html>
```

JavaScript does not interpret VAR or Var as the keyword var.


* JavaScript and Camel Case


Historically, programmers have used different ways of joining multiple words into one variable name:

- Hyphens:

first-name, last-name, master-card, inter-city.


- Underscore:

first_name, last_name, master_card, inter_city.

Upper Camel Case (Pascal Case):

FirstName, LastName, MasterCard, InterCity.

Lower Camel Case:

JavaScript programmers tend to use camel case that starts with a lowercase letter:

firstName, lastName, masterCard, interCity.


## JavaScript Comments

JavaScript comments can be used to explain JavaScript code, and to make it more readable.

JavaScript comments can also be used to prevent execution, when testing alternative code.


* Single Line Comments

Single line comments start with //.

Any text between // and the end of the line will be ignored by JavaScript (will not be executed).

This example uses a single-line comment before each code line:

EXAMPLE :



```bash
<!DOCTYPE html>
<html>
<body>

  <h1 id="myH"></h1>
  <p id="myP"></p>

<script>
  // Change heading:
  document.getElementById("myH").innerHTML = "JavaScript Comments";
  // Change paragraph:
  document.getElementById("myP").innerHTML = "My first paragraph.";
</script>

</body>
</html>
```


This example uses a single line comment at the end of each line to explain the code:


```bash
<!DOCTYPE html>
<html>
<body>
  <h2>JavaScript Comments</h2>

  <p id="demo"></p>

<script>
  let x = 5;    // Declare x, give it the value of 5
  let y = x + 2;  // Declare y, give it the value of x + 2 
  // Write y to demo:
  document.getElementById("demo").innerHTML = y;
</script>


</body>
</html>
```


* Multi-line Comments


Multi-line comments start with /* and end with */.

Any text between /* and */ will be ignored by JavaScript.

This example uses a multi-line comment (a comment block) to explain the code:

EXAMPLE



```bash
<!DOCTYPE html>
<html>
<body>

  <h1 id="myH"></h1>
  <p id="myP"></p>

<script>
  /*
  The code below will change
  the heading with id = "myH"
  and the paragraph with id = "myP"
  */
  document.getElementById("myH").innerHTML = "JavaScript Comments";
  document.getElementById("myP").innerHTML = "My first paragraph.";
</script>

</body>
</html>
```



* Using Comments to Prevent Execution

Using comments to prevent execution of code is suitable for code testing.

Adding // in front of a code line changes the code lines from an executable line to a comment.

This example uses // to prevent execution of one of the code lines:Using comments to prevent execution of code is suitable for code testing.

Adding // in front of a code line changes the code lines from an executable line to a comment.

This example uses // to prevent execution of one of the code lines:


EXAMPLE



```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript Comments</h2>

  <h1 id="myH"></h1>

  <p id="myP"></p>

<script>
  //document.getElementById("myH").innerHTML = "My First Page";
  document.getElementById("myP").innerHTML = "My first paragraph.";
</script>

  <p>The line starting with // is not executed.</p>

</body>
</html>
```


This example uses a comment block to prevent execution of multiple lines:

```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript Comments</h2>

  <h1 id="myH"></h1>

  <p id="myP"></p>


<script>
  /*
  document.getElementById("myH").innerHTML = "Welcome to my Homepage";
  document.getElementById("myP").innerHTML = "This is my first paragraph.";
  */
  document.getElementById("myP").innerHTML = "The comment-block is not executed.";
</script>


</body>
</html>
```


## JavaScript Variables

JavaScript variables are containers for storing data values.

In this example, x, y, and z, are variables:

Example

```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript Variables</h2>

  <p>In this example, x, y, and z are variables.</p>

  <p id="alc"></p>

<script>
  let x = 4;
  let y = 3;
  let z = x + y;
  document.getElementById("alc").innerHTML =
  "The value of z is: " + z;
</script>

</body>
</html>
```

From the example above, you can expect:

x stores the value 4
y stores the value 3
z stores the value 7


* Much Like Algebra

In this example, price1, price2, and total, are variables:

Example

```bash
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Variables</h2>

<p id="alc"></p>

<script>
  let price1 = 4;
  let price2 = 3;
  let total = price1 + price2;
  document.getElementById("alc").innerHTML =
  "The total is: " + total;
</script>

</body>
</html>
```

In programming, just like in algebra, we use variables (like price1) to hold values.

In programming, just like in algebra, we use variables in expressions (total = price1 + price2).

From the example above, you can calculate the total to be 7.


* JavaScript Identifiers

All JavaScript variables must be identified with unique names.

These unique names are called identifiers.

Identifiers can be short names (like x and y) or more descriptive names (age, sum, totalVolume).

The general rules for constructing names for variables (unique identifiers) are:


```bash
- Names can contain letters, digits, underscores, and dollar signs.
- Names must begin with a letter
- Names can also begin with $ and _ (but we will not use it in this tutorial)
- Names are case sensitive (y and Y are different variables)
- Reserved words (like JavaScript keywords) cannot be used as names

JavaScript identifiers are case-sensitive.
```

* The Assignment Operator

In JavaScript, the equal sign (=) is an "assignment" operator, not an "equal to" operator.

This is different from algebra. The following does not make sense in algebra:

```bash
  x = x + 4
```


In JavaScript, however, it makes perfect sense: it assigns the value of x + 5 to x.

(It calculates the value of x + 5 and puts the result into x. The value of x is incremented by 4.)


```bash
  The "equal to" operator is written like == in JavaScript.
```

* JavaScript Data Types


JavaScript variables can hold numbers like 100 and text values like "John Doe".

In programming, text values are called text strings.

JavaScript can handle many types of data, but for now, just think of numbers and strings.

Strings are written inside double or single quotes. Numbers are written without quotes.

If you put a number in quotes, it will be treated as a text string.


Example


```bash
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Variables</h2>

<p>Strings are written with quotes.</p>
<p>Numbers are written without quotes.</p>

<p id="alc"></p>

<script>
  let pi = 3.14;
  let person = "Marie Claire";
  let answer = 'Yes I am!';

  document.getElementById("alc").innerHTML =
  pi + "<br>" + person + "<br>" + answer;
</script>

</body>
</html>
```


* Declaring (Creating) JavaScript Variables

Creating a variable in JavaScript is called "declaring" a variable.

You declare a JavaScript variable with the let keyword:


```bash
let carName;
```

After the declaration, the variable has no value (technically it has the value of undefined).

To assign a value to the variable, use the equal sign:


```bash
carName = "Patrick";
```

You can also assign a value to the variable when you declare it:

```bash
let carName = "Patrick"; 
```


In the example below, we create a variable called carName and assign the value "Volvo" to it.

Then we "output" the value inside an HTML paragraph with id="alc":

Example


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript Variables</h2>

  <p>Create a variable, assign a value to it, and display it:</p>

  <p id="alc"></p>

<script>
  const carName = "Patrick";
  document.getElementById("alc").innerHTML = carName;
</script>

</body>
</html> 
```


```bash
It's a good programming practice to declare all variables at the beginning of a script.
```

* One Statement, Many Variables

You can declare many variables in one statement.

Start the statement with let and separate the variables by comma:


Example


```bash
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Variables</h2>

<p>You can declare many variables in one statement.</p>

<p id="alc"></p>

<script>
  let person = "Marie Claire", carName = "pat", price = 100;
  document.getElementById("alc").innerHTML = carName;
</script>

</body>
</html>
```


A declaration can span multiple lines:



```bash
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Variables</h2>

<p>You can declare many variables in one statement.</p>

<p id="alc"></p>

<script>
  let person = "Marie Claire",
  carName = "pat",
  price = 100;
  document.getElementById("alc").innerHTML = carName;
</script>

</body>
</html>
```


 * Value = undefined


 In computer programs, variables are often declared without a value. The value can be something that has to be calculated, or something that will be provided later, like user input.

A variable declared without a value will have the value undefined.

The variable carName will have the value undefined after the execution of this statement:


Example


```bash
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Variables</h2>

<p>A variable declared without a value will have the value undefined.</p>

<p id="alc"></p>

<script>
  let carName;
  document.getElementById("alc").innerHTML = carName;
</script>

</body>
</html>
```


* Re-Declaring JavaScript Variables


If you re-declare a JavaScript variable, it will not lose its value.

The variable carName will still have the value "Patrick" after the execution of these statements:


Example


```bash
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Variables</h2>

<p>If you re-declare a JavaScript variable, it will not lose its value.</p>

<p id="alc"></p>

<script>
  let carName = "Patrick";
  let carName;
  document.getElementById("alc").innerHTML = carName;
</script>

</body>
</html>
```


* JavaScript Arithmetic


As with algebra, you can do arithmetic with JavaScript variables, using operators like = and +:


Example


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript Variables</h2>

  <p>The result of adding 5 + 2 + 3:</p>

  <p id="alc"></p>

<script>
  let x = 5 + 2 + 3;
  document.getElementById("alc").innerHTML = x;
</script>

</body>
</html>
```

You can also add strings, but strings will be concatenated:


Example


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript Variables</h2>

  <p>The result of adding "Marie" + " " + "Claire":</p>

  <p id="alc"></p>

<script>
  let x = "Marie" + " " + "Claire";
  document.getElementById("alc").innerHTML = x;
</script>

</body>
</html>
```


Also try this:

Example


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript Variables</h2>

  <p>The result of adding "5" + 2 + 3:</p>

  <p id="alc"></p>

<script>
  x = "5" + 2 + 3;
  document.getElementById("alc").innerHTML = x;
</script>

</body>
</html>
```


```bash
If you put a number in quotes, the rest of the numbers will be treated as strings, and concatenated.
```


Now try this:


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript Variables</h2>

  <p>The result of adding 2 + 3 + "5":</p>

  <p id="alc"></p>

<script>
  var x = 2 + 3 + "5"
  document.getElementById("alc").innerHTML = x;
</script>

</body>
</html>
```



# JavaScript Operators


Assign values to variables and add them together:



```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript Operators</h2>

  <p>x = 4, y = 6, calculate z = x + y, and display z:</p>

  <p id="alc"></p>

<script>
  let x = 4;
  let y = 6;
  let z = x + y;
  document.getElementById("alc").innerHTML = z;
</script>

</body>
</html>
```


The assignment operator (=) assigns a value to a variable.


* Assignment


EXAMPLE : 

```bash
<!DOCTYPE html>
<html>
<body>

  <h2>The = Operator</h2>

  <p id="alc"></p>

<script>
  let x = 10;
  document.getElementById("alc").innerHTML = x;
</script>

</body>
</html>
```


The addition operator (+) adds numbers:


* Adding

EXAMPLE :


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>The + Operator</h2>

  <p id="alc"></p>

<script>
  let x = 5;
  let y = 2;
  let z = x + y;
  document.getElementById("alc").innerHTML = z;
</script>

</body>
</html>
```


The multiplication operator (*) multiplies numbers.

* Multiplying


EXAMPLE :

```bash
<!DOCTYPE html>
<html>
<body>

  <h2>The * Operator</h2>

  <p id="alc"></p>

<script>
  let x = 5;
  let y = 2;
  let z = x * y;
  document.getElementById("alc").innerHTML = z;
</script>

</body>
</html>
```

* JavaScript Arithmetic Operators

Link =>  https://www.w3schools.com/js/js_arithmetic.asp



* JavaScript Assignment Operators

Link =>   https://www.w3schools.com/js/js_assignment.asp



* JavaScript String Operators

EXAMPLE : 

```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript Operators</h2>

  <p>The + operator concatenates (adds) strings.</p>

  <p id="alc"></p>

<script>
  var txt1 = "John";
  var txt2 = "Doe";
  document.getElementById("alc").innerHTML = txt1 + " " + txt2;
</script>

</body>
</html>
```


* JavaScript Comparison Operators


Link =>  https://www.w3schools.com/js/js_comparisons.asp


* JavaScript Logical Operators

Logical operators are fully described in the   
  Link =>  https://www.w3schools.com/js/js_comparisons.asp


* JavaScript Type Operators


Type operators are fully described in the Link => https://www.w3schools.com/js/js_type_conversion.asp


* JavaScript Bitwise Operators


Bitwise operators are fully described in the => https://www.w3schools.com/js/js_bitwise.asp




# JavaScript Arithmetic


Arithmetic operators perform arithmetic on numbers (literals or variables).


* Arithmetic Operations  

A typical arithmetic operation operates on two numbers.

EXAMPLE : 

```bash
<!DOCTYPE html>
<html>
<body>

  <p>A typical arithmetic operation takes two numbers and produces a new number.</p>

  <p id="alc"></p>

<script>
  let x = 100 + 50;
  document.getElementById("alc").innerHTML = x;
</script>

</body>
</html>
```


* Operators and Operands


The numbers (in an arithmetic operation) are called operands.

The operation (to be performed between the two operands) is defined by an operator.


* Adding

The addition operator (+) adds numbers.

EXAMPLE :


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>The + Operator</h2>

  <p id="alc"></p>

<script>
  let x = 5;
  let y = 2;
  let z = x + y;
  document.getElementById("alc").innerHTML = z;
</script>

</body>
</html>
```



* Subtracting

The subtraction operator (-) subtracts numbers.

EXAMPLE :

```bash
<!DOCTYPE html>
<html>
<body>

<h2>The - Operator</h2>

<p id="alc"></p>

<script>
  let x = 5;
  let y = 2;
  let z = x - y;
  document.getElementById("alc").innerHTML = z
</script>

</body>
</html>
```


* Multiplying

The multiplication operator (*) multiplies numbers.

EXAMPLE :


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>The * Operator</h2>

  <p id="alc"></p>

<script>
  let x = 5;
  let y = 2;
  let z = x * y;
  document.getElementById("alc").innerHTML = z;
</script>

</body>
</html>
```


* Dividing

The division operator (/) divides numbers.

EXAMPLE :

```bash
<!DOCTYPE html>
<html>
<body>

  <h2>The / Operator</h2>

  <p id="alc"></p>

<script>
  let x = 5;
  let y = 2;
  let z = x / y;
  document.getElementById("alc").innerHTML = z;
</script>

</body>
</html>
```

* Remainder

The modulus operator (%) returns the division remainder.

EXAMPLE :

```bash
<!DOCTYPE html>
<html>
<body>

  <h2>The % Operator</h2>

  <p id="alc"></p>

<script>
  let x = 5;
  let y = 2;
  let z = x % y;
document.getElementById("alc").innerHTML = z;
</script>

</body>
</html>
```

* Incrementing

The increment operator (++) increments numbers.

EXAMPLE :


```bash
<!DOCTYPE html>
<html>
<body>

<h2>The ++ Operator</h2>

<p id="alc"></p>

<script>
  let x = 5;
  x++;
  let z = x;
  document.getElementById("let").innerHTML = z;
</script>

</body>
</html>
```

* Decrementing

The decrement operator (--) decrements numbers.

EXAMPLE :


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>The -- Operator</h2>

  <p id="alc"></p>

<script>
  let x = 5;
  x--;
  let z = x;
  document.getElementById("alc").innerHTML = z;
</script>

</body>
</html>
```

* Exponentiation

The exponentiation operator (**) raises the first operand to the power of the second operand.

EXAMPLE :

```bash
<!DOCTYPE html>
<html>
<body>

  <h2>The ** Operator</h2>

  <p id="alc"></p>

<script>
  let x = 5;
  document.getElementById("alc").innerHTML = x ** 2;
</script>

</body>
</html>
```

* Operator Precedence

Operator precedence describes the order in which operations are performed in an arithmetic expression.

EXAMPLE :

```bash
<!DOCTYPE html>
<html>
<body>

  <p>Multiplication has precedence over addition.</p>

  <p id="alc"></p>

<script>
  document.getElementById("alc").innerHTML = 100 + 50 * 3;
</script>

</body>
</html>
```


# JavaScript Assignment

Assignment operators assign values to JavaScript variables.

> The **= operator is an experimental part of the ECMAScript 2016 proposal (ES7). It is not stable across browsers. Do not use it.


Assignment Examples

The = assignment operator assigns a value to a variable.


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>The = Operator</h2>

  <p id="alc"></p>

<script>
  let x = 10;
  document.getElementById("alc").innerHTML = x;
</script>

</body>
</html>
```


# JavaScript Data Types


JavaScript variables can hold many data types: numbers, strings, objects and more:


> var length = 16;                               // Number
var lastName = "Johnson";                      // String
var x = {firstName:"John", lastName:"Doe"};    // Object


* The Concept of Data Types

In programming, data types is an important concept.

To be able to operate on variables, it is important to know something about the type.

Without data types, a computer cannot safely solve this:


> let x = 16 + "Volvo";


Does it make any sense to add "Volvo" to sixteen? Will it produce an error or will it produce a result? JavaScript will treat the example above as:

> let x = "16" + "Volvo";


** When adding a number and a string, JavaScript will treat the number as a string.


EXAMPLE : 


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript</h2>

  <p>When adding a number and a string, JavaScript will treat the number as a string.</p>

  <p id="alc"></p>

<script>
  let x = 16 + "Volvo";
  document.getElementById("alc").innerHTML = x;
</script>

</body>
</html>
```


* JavaScript Types are Dynamic

JavaScript has dynamic types. This means that the same variable can be used to hold different data types:


EXAMPLE : 

```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript Data Types</h2>

  <p>JavaScript has dynamic types. This means that the same variable can be used to hold different data types:</p>

  <p id="alc"></p>

<script>
  let x;         // Now x is undefined
  x = 5;         // Now x is a Number
  x = "John";      // Now x is a String

  document.getElementById("alc").innerHTML = x;
</script>

</body>
</html>
```


* JavaScript Strings

A string (or a text string) is a series of characters like "John Doe".

Strings are written with quotes. You can use single or double quotes:


EXAMPLE: 


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript Strings</h2>

  <p>Strings are written with quotes. You can use single or double quotes:</p>

  <p id="alc"></p>

<script>
  let carName1 = "Volvo XC60";
  let carName2 = 'Volvo XC60';

  document.getElementById("alc").innerHTML =
  carName1 + "<br>" + 
  carName2; 
</script>

</body>
</html>
```


* JavaScript Numbers

JavaScript has only one type of numbers.

Numbers can be written with, or without decimals:


EXAMPLE:


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript Numbers</h2>

  <p>Numbers can be written with, or without decimals:</p>

  <p id="alc"></p>

<script>
  let x1 = 34.00;
  let x2 = 34;
  let x3 = 3.14;

  document.getElementById("alc").innerHTML =
  x1 + "<br>" + x2 + "<br>" + x3;
</script>

</body>
</html>
```


* JavaScript Booleans

Booleans can only have two values: true or false.


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript Booleans</h2>

  <p>Booleans can have two values: true or false:</p>

  <p id="alc"></p>

<script>
  let x = 5;
  let y = 5;
  let z = 6;
  document.getElementById("alc").innerHTML =
  (x == y) + "<br>" + (x == z);
</script>

</body>
</html>
```


* JavaScript Arrays


JavaScript arrays are written with square brackets.

Array items are separated by commas.

The following code declares (creates) an array called cars, containing three items (car names):


EXAMPLE : 


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript Arrays</h2>

  <p>Array indexes are zero-based, which means the first item is [0].</p>

  <p id="alc"></p>

<script>
  const cars = ["Saab","Volvo","BMW"];

  document.getElementById("alc").innerHTML = cars[0];
</script>

</body>
</html>
```


> Array indexes are zero-based, which means the first item is [0], second is [1], and so on.


* JavaScript Objects

JavaScript objects are written with curly braces {}.

Object properties are written as name:value pairs, separated by commas.


EXAMPLE : 


```bash
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Objects</h2>

<p id="alc"></p>

<script>
  const person = {
    firstName : "John",
    lastName  : "Doe",
    age     : 50,
    eyeColor  : "blue"
  };

  document.getElementById("alc").innerHTML =
  person.firstName + " is " + person.age + " years old.";
</script>

</body>
</html>
```


> The object (person) in the example above has 4 properties: firstName, lastName, age, and eyeColor.

You will learn more about objects later in this tutorial.


* The typeof Operator

You can use the JavaScript typeof operator to find the type of a JavaScript variable.

The typeof operator returns the type of a variable or an expression:

```bash
typeof ""             // Returns "string"
typeof "John"         // Returns "string"
typeof "John Doe"     // Returns "string"
```


* Undefined

In JavaScript, a variable without a value, has the value undefined. The type is also undefined.

EXAMPLE : 


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript</h2>

  <p>The value (and the data type) of a variable with no value is <b>undefined</b>.</p>

  <p id="alc"></p>

<script>
  let car;
  document.getElementById("alc").innerHTML =
  car + "<br>" + typeof car;
</script>

</body>
</html> 
```


Any variable can be emptied, by setting the value to undefined. The type will also be undefined.



EXAMPLE : 

```bash
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript</h2>

<p>Variables can be emptied if you set the value to <b>undefined</b>.</p>

<p id="alc"></p>

<script>
  let car = "Volvo";
  car = undefined;
  document.getElementById("alc").innerHTML =
  car + "<br>" + typeof car;
</script>

</body>
</html>
```


* Empty Values

An empty value has nothing to do with undefined.

An empty string has both a legal value and a type.


EXAMPLE : 


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript</h2>

  <p>An empty string has both a legal value and a type:</p>

  <p id="alc"></p>

<script>
  let car = "";
  document.getElementById("alc").innerHTML =
  "The value is: " +
  car + "<br>" +
  "The type is: " + typeof car;
</script>

</body>
</html>
```


* Null

In JavaScript null is "nothing". It is supposed to be something that doesn't exist.

Unfortunately, in JavaScript, the data type of null is an object.


> You can consider it a bug in JavaScript that typeof null is an object. It should be null.


You can empty an object by setting it to null:


EXAMPLE : 


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript</h2>

  <p>Objects can be emptied by setting the value to <b>null</b>.</p>

  <p id="alc"></p>

<script>
  let person = {firstName:"Marie", lastName:"Claire", age:50, eyeColor:"blue"};
  person = null;
  document.getElementById("alc").innerHTML = typeof person;
</script>

</body>
</html> 
```


* Difference Between Undefined and Null


undefined and null are equal in value but different in type:


EXAMPLE : 


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript</h2>

  <p>Undefined and null are equal in value but different in type:</p>

  <p id="alc"></p>

<script>
  document.getElementById("alc").innerHTML =
  typeof undefined + "<br>" +
  typeof null + "<br><br>" +
  (null === undefined) + "<br>" +
  (null == undefined);
</script>

</body>
</html>  
```


* Primitive Data


A primitive data value is a single simple data value with no additional properties and methods.

The typeof operator can return one of these primitive types:


```bash
- string
- number
- boolean
- undefined  
```

EXAMPLE : 


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript typeof</h2>
  <p>The typeof operator returns the type of a variable or an expression.</p>

  <p id="alc"></p>

<script>
  document.getElementById("alc").innerHTML = 
  typeof "Marie" + "<br>" + 
  typeof 3.14 + "<br>" +
  typeof true + "<br>" +
  typeof false + "<br>" +
  typeof x;
</script>

</body>
</html>  
```


* Complex Data


The typeof operator can return one of two complex types:

> function

> object

The typeof operator returns "object" for objects, arrays, and null.

The typeof operator does not return "object" for functions.


EXAMPLE :


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript typeof</h2>
  <p>The typeof operator returns object for both objects, arrays, and null.</p>
  <p>The typeof operator does not return object for functions.</p>

  <p id="alc"></p>

<script>
  document.getElementById("alc").innerHTML = 
  typeof {name:'Marie', age:34} + "<br>" +
  typeof [1,2,3,4] + "<br>" +
  typeof null + "<br>" +
  typeof function myFunc(){};
</script>

</body>
</html>  
```

> The typeof operator returns "object" for arrays because in JavaScript arrays are objects.



# JavaScript Functions


A JavaScript function is a block of code designed to perform a particular task.

A JavaScript function is executed when "something" invokes it (calls it).


EXAMPLE 


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript Functions</h2>

  <p>This example calls a function which performs a calculation, and returns the result:</p>

  <p id="alc"></p>

<script>
  const myFunction = (p1, p2) => { return p1 * p2;}
  document.getElementById("demo").innerHTML = myFunction(8, 3);
</script>

</body>
</html>  
```


* JavaScript Function Syntax


A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses ().

Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).

The parentheses may include parameter names separated by commas:
(parameter1, parameter2, ...)

The code to be executed, by the function, is placed inside curly brackets: {}


// es5

```bash
function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
```


// es6 

```bash
const name = (parameter1, parameter2, parameter3) => {
  // code to be executed
}
```

> we will come back to a more detailed course on the modern js at the end of it



* Function Invocation

```bash
- When an event occurs (when a user clicks a button)
- When it is invoked (called) from JavaScript code
- Automatically (self invoked)
``` 


* Function Return


// es5 


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript Functions</h2>

  <p>This example calls a function which performs a calculation and returns the result:</p>

  <p id="alc"></p>

<script>
  var a = myFunction(4, 3);
  document.getElementById("alc").innerHTML = a;

  function myFunction(x, y) {
    return x * y;
  }
</script>

</body>
</html>
```


// es6 

```bash
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Functions</h2>

<p>This example calls a function which performs a calculation and returns the result:</p>

<p id="alc"></p>

<script>

  const chainedAddition = ( a,b ) => {
    return (a * b); 
  }

  const pat = chainedAddition(9, 4);
  document.getElementById('alc').innerHTML = pat;

</script>

</body>
</html>
```


* Why Functions?

You can reuse code: Define the code once, and use it many times.

You can use the same code many times with different arguments, to produce different results.


EXAMPLE : 

// es5


```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript Functions</h2>

  <p>This example calls a function to convert from Fahrenheit to Celsius:</p>
  <p id="demo"></p>

<script>
  function toCelsius(f) {
    return (5/9) * (f-32);
  }
  document.getElementById("demo").innerHTML = toCelsius(77);
</script>

</body>
</html>
```


// es6

```bash
<!DOCTYPE html>
<html>
<body>

  <h2>JavaScript Functions</h2>

  <p>This example calls a function to convert from Fahrenheit to Celsius:</p>
  <p id="demo"></p>

<script>
  const toCelsius = f => {return (5/9) * (f-32);}

  const pat = toCelsius(68);

  document.getElementById("demo").innerHTML = pat;
</script>

</body>
</html>
```



# JavaScript Objects

Real Life Objects, Properties, and Methods
In real life, a car is an object.

