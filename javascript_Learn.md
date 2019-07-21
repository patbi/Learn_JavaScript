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
* JavaScript in <head> or <body>.

You can place any number of scripts in an HTML document.
Scripts can be placed in the <body>, or in the <head> section of an HTML page, or in both.


* External JavaScript.

Scripts can also be placed in external files



## JavaScript in <head>

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


## JavaScript in <body>

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


