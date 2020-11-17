# **JavaScript: Client-Side Scripting**

## **What is Javascript?**

* JS runs inside the browser
* JS is dynamically typed 
* JS is OOP and almost everything is an object

### **Client-Side Scripting**

1. client -> GET /vacation.html
2. server -> vacation.html
3. client -> execute any JS if required
4. client -> display to the browser

### **PROS of Client-Side Scripting**
* reduce the load on the server
* browser can respond more quickly than making a new request to the server
* JS can interact with the HTML element in a way that a server cannot, creating an user experience more like desktop software than simple HTML ever could. 

### **CONS of Client-Side Scripting**

* No garantee that the client has JS enabled    
* The idiosyncrasies between various browsers and operating systems make it difficult to test for all potential client configurations. What works in one browser, may generate an error in another.
* JavaScript-heavy web applications can be complicated to debug and maintain. 

### **HTTP request-response loop**

1. client: GET /form.php
2. server: returns form.php
3. client: select one option on dropdown and clicks update
4. client: request GET /form.php?country=canada
5. server: returns updated form with updated states/provinces for the form

> In details, <br>
> 1. Request  <br>
> 2. Response <br>
> 3. After the browser receives a response to its HTTP request, it blanks the browser window and... <br>
> 4. ... renders the just-recieved HTML in the browser window. <br>
> 5. Request <br>
> 6. Response <br>
> 7. Another new response has been received, so browser window is blanked and... <br>
> 8. ...renders the just-received HTML in the browser window. 



### **JavaScript in Modern Times**
* JavaScript became a much more important part of web dev in the mid 2000s with AJAX.
* AJAX = Acronym & General Term
    * Asynchronous JavaScript And XML.
    * The most inmportant feature of AJAX sites is the asynchronous data requests. 


### **Asynchronous Data Request**

1. Request
2. Response
3. Browser blanks and renders the HTML received
4. User clicks update buton on form
5. Via JS, browser makes asynchronous request for data
6. Server respond a XML or JSON data 
7. JS updates the form


### **Layers**

* Presentation layer = Classes focused on the user interface.
* Business layer = Classes that model real-world entities, such as customers, products and sales
* Data layer = Classes that handle the interaction with the data sources
<br>

### **JavaScript Overview** ###

* Everything type sensitive. 
* Scope of variables are all global.
* === operator checks for equality in value and type.
* ```Null``` and ```undefined``` are different states for a variable
* Semicolons are not required but encouraged 
* No integer type, only float point numbers


## **Variables**

* Dinamically typed
* ```var``` is the keyword
* Assignment can happen can happen at declaration time by appending the value to the declaration, or at runtime with a simple right-to-left assingment 

#### Example ####

```JavaScript
var x ;   // a variable x is defined 
var y = 0;  // y is defined and initialized with 0 
y = 4;     // y is assigned the value of 4.

/*conditional assignment*/

x = (y==4) ? "y is 4" : "y is not 4";

```

## **Logical Operators**

```Javascript
//and
&& 
// or
||
// not 
!
```

## **Conditionals**

```Javascript 
var hourOfTheDay; 
var greeting;

if (hourOfTheDay > 4 && hourOfDay < 12){
    greeting = "Good Morning";
}

```


## **Loops**

```Javascript
var i=0; // initialize the Loop Control Variable

while(i<10){//test the control variable
    i++; //increment control variable
}
```

```Javascript
for (var i=0 ; i<10 ; i++){
    //do someting here
}
```

## **Functions**

