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

