# javscript-sound-byte-answers

1	What are the possible ways to create objects in JavaScript
  *Object constructor:var object = new Object();
  *Object's create method:var object = Object.create(null);
  *Object literal syntax:var object = {};
  *Function constructor:
  function Person(name){
   this.name=name;
   this.age=21;
}
var object = new Person("name");
  *ES6 Class syntax:
  class Person {
   constructor(name) {
      this.name = name;
   }
}
var object = new Person("name");
*Singleton pattern:
var object = new function(){
   this.name = "Sudheer";
}

2	What is prototype chain 
3	What is the difference between Call, Apply and Bind
  *Call invokes the function and allows you to pass in arguments one by one.
  *Apply invokes the function and allows you to pass in arguments as an array.
  *Bind returns a new function, allowing you to pass in a this array and any number of arguments.

4	What is JSON and its common operations
  JSON is the  text-based data format following JavaScript object syntax.it is used for transmit data across network.
  operations: JSON.stringify - used to convert object to string.
  JSON.parse - used to convert string to object.
  
5	What is the purpose of the array slice method
     slice() method returns the selected elements in an array as a new array object. 
     It selects the elements starting at the given start argument, and ends at the given optional end argument.
     it does not change original array.
     
6	What is the purpose of the array splice method
    splice() method is used either adds/removes items to/from an array, and then returns the removed item. 
    The first argument specifies the array position for insertion or deletion whereas the optional second argument indicates the number of elements to be deleted. 
    Each additional argument is added to the array.
    it modifies original array and return deleted elements.
    
7	What is the difference between slice and splice
8	How do you compare Object and Map
9	What is the difference between == and === operators
    * == performs type coercion and compare variables and return result.
    *=== does not  performs type coercion and compare variables.
    
10	What are lambda or arrow functions
    An arrow function is a shorter syntax for a function expression and does not have its own this, arguments, super, or new.target
    
11	What is a first class function
12	What is a first order function
      First-order function is a function that doesn’t accept another function as an argument and doesn’t return a function as its return value.

13	What is a higher order function
      Higher-order function is a function that accepts another function as an argument or returns a function as a return value or both.

14	What is a unary function
      Unary function (i.e. monadic) is a function that accepts exactly one argument. It stands for a single argument accepted by a function.
15	What is the currying function
      
16	What is a pure function
      Pure Function is a function that always returns the same result if the same arguments are passed.
      its only depends on input arugments.
      
17	What is the purpose of the let keyword
      The let statement declares a block scope local variable.it only accessed by its block of statement.
      
18	What is the difference between let and var
19	What is the reason to choose the name let as a keyword
20	How do you redeclare variables in switch block without an error
    we can create block inside the case block to declare block scoped variable with out causing error.
    
21	What is the Temporal Dead Zone
    in JavaScript that occurs when declaring a variable with the let and const keywords, but not with var.
    The time span when that happens, between the creation of a variable’s binding and its declaration, is called the temporal dead zone.
    
22	What is IIFE(Immediately Invoked Function Expression)
    IIFE (Immediately Invoked Function Expression) is a JavaScript function that runs as soon as it is defined.
    example:(function (){
              console.log('this is IIFE');
              })
              
23	How do you decode or encode a URL in JavaScript?
    *encodeURL() function is used to encode an URL. This function requires a URL string as a parameter and return that encoded string. 
    *decodeURI() function is used to deocde an URL. This function requires an encoded URL string as parameter and return that decoded string.

24	What is memoization
        Memoization is a programming technique which attempts to increase a function’s performance by caching its previously computed results.
        Each time a memoized function is called, its parameters are used to index the cache. 
        If the data is present, then it can be returned, without executing the entire function. 
        Otherwise the function is executed and then the result is added to the cache.
        
25	What is Hoisting
        Hoisting is a JavaScript mechanism where variables and function declarations are moved to the top of their scope before code execution.
         JavaScript only hoists declarations, not initialisation.
26	What are classes in ES6
        
27	What are closures
    A closure is the combination of a function and the lexical environment within which that function was declared.
    i.e, It is an inner function that has access to the outer or enclosing function’s variables. The closure has three scope chains
    *Own scope where variables defined between its curly brackets
    * Outer function’s variables
    *Global variables
    
28	What are modules
    Modules refer to small units of independent, reusable code.
29	Why do you need modules
     Below are the list of benefits using modules in javascript ecosystem
      *Maintainability
      *Reusability
      *Namespacing
30	What is scope in javascript
    Scope is the accessibility of variables, functions, and objects in some particular part of your code during runtime.
    scope determines the visibility of variables and other resources in areas of your code.
    
31	What is a service worker
    A service worker is a script that runs independently in the browser background.
    major features of service workers are Rich offline experiences(offline first web application development),like push notification
    
32	How do you manipulate DOM using a service worker
33	How do you reuse information across service worker restarts
     service worker is that it gets terminated when not in use, and restarted when it's next needed.
     you cannot rely on global state within a service worker's onfetch and onmessage handlers. 
     In this case, service workers will have access to IndexedDB API in order to persist and reuse across restarts.

34	What is IndexedDB
    indexedDB is a low-level API for client-side storage of larger amounts of structured data, including files/blobs. 
    This API uses indexes to enable high-performance searches of this data.
35	What is web storage
    web storage is the mechanism which we can store data in browser locally in key/value pair.there is two type of web storage are:
    *local storage 
    *session storage
    
36	What is a post message
    Post message is a method that enables cross-origin communication between Window objects.i.e, between a page and a pop-up that it spawned, or between a page and an iframe       embedded within it.
    
37	What is a cookie
      A cookie is a piece of data that is stored on your computer to be accessed by your browser. Cookies are saved as key/value pairs.
      
38	Why do you need a Cookie
      Cookies are used to remember information about the user profile(such as username). It involves two steps,
      *When a user visits a web page, the user profile can be stored in a cookie.
      *Next time the user visits the page, the cookie remembers the user profile.
      
39	What are the options in a cookie
      *the cookie is deleted when the browser is closed but you can change this by setting expiry date (in UTC time).
       example: document.cookie = "username=John; expires=Sat, 8 Jun 2019 12:00:00 UTC";
      *the cookie belongs to a current page.you can use it to other by using a path parameter.
       example: document.cookie = "username=John; path=/services";
        
40	How do you delete a cookie
      you can delete cookie by seeting expiry date.
      example:document.cookie = "username=; expires=Fri, 07 Jun 2019 00:00:00 UTC; path=/;";

41	What are the differences between cookie, local storage and session storage
42	What is the main difference between localStorage and sessionStorage
      session storage deleted after page session ends like closing the tab whereas localstorage not deleted until manually delete it.
      
43	How do you access web storage
      the window object contains objects for local and session storages to access it.
      you can set local or session storage using setItem method and retrive using getItem method.
      example:localStorage.setItem('logo', document.getElementById('logo').value);
      localStorage.getItem('logo');
      
44	What are the methods available on session storage
      setItem - set data
      getItem - retrive data
      removeItem  - delete data with specific key
      clear   - remove all data
      
45	What is a storage event and its event handler
46	Why do you need web storage
    it is more secure, and large amounts of data can be stored locally, without affecting website performance.
    the information is never transferred to the server.
    
47	How do you check web storage browser support
      if (typeof(Storage) !== "undefined") {
  // Code for localStorage/sessionStorage.
} else {
  // Sorry! No Web Storage support..
}

48	How do you check web workers browser support
      if (typeof(Worker) !== "undefined") {
  // code for Web worker support.
} else {
  // Sorry! No Web Worker support..
}

49	Give an example of web worker
50	What are the restrictions of web workers on DOM
51	What is a promise
 A promise is an object that produce single value some time in the future with either a resolved value or rejected value.
 it used to handle  asynchronous operations in JavaScript.

52	Why do you need a promise
    Promises are used to handle asynchronous operations. 
    They provide an alternative approach for callbacks by reducing the callback hell and writing the cleaner code.
    
53	What are the three states of promise
    *Pending: initial state of the Promise before an operation begins
    *Fulfilled:  the specified operation was completed.
    *Rejected:  the operation did not complete. In this case an error value will be thrown.

54	What is a callback function
    A callback function is a function passed into another function as an argument.
    This function is invoked inside the outer function to complete an action.
    
55	Why do we need callbacks
    it used to handle  asynchronous operations in JavaScript.
    javascript is event driven language, instead of waiting for a response javascript will keep executing while listening for other events.

56	What is a callback hell
    Callback Hell is an anti-pattern with multiple nested callbacks which makes code hard to read and debug when dealing with asynchronous logic.
    
57	What is server-sent events
    Server-sent events (SSE) is a server push technology enabling a browser to receive automatic updates from a server via HTTP connection. 
    These are a one way communications channel - events flow from server to client only. 
    This are used in Facebook/Twitter updates, stock price updates, news feeds etc.
    
58	How do you receive server-sent event notifications
    The EventSource object is used to receive server-sent event notifications.
    
59	How do you check browser support for server-sent events
60	What are the events available for server sent events
      *onopen -  used when connection to the server is opened
      *onmessage - used when message is received
      *onerrror - used when error occurs
      
61	What are the main rules of promise
      *A promise is an object that supplies a standard-compliant .then() method
      *A pending promise may transition into either fulfilled or rejected state
      *A fulfilled or rejected promise is settled and it must not transition into any other state.
      *Once a promise is settled, the value must not change.
      
62	What is callback in callback
      the nesting of callback inside callback.it is used to execute the actions sequentially one by one.
      
63	What is promise chaining
      the process of executing a sequence of asynchronous tasks one after another using promises is known as Promise chaining.
      
64	What is promise.all
      Promise.all is a promise that takes an array of promises as an input. 
      it gets resolved when all the promises get resolved or any one of them gets rejected.
      
65	What is the purpose of race method in promise
      Promise.race() method will return the promise instance which is firstly resolved or rejected
      
66	What is a strict mode in javascript
      Strict Mode is a new feature that prevents certain actions from being taken and throws more exceptions.
      
67	Why do you need strict mode
      Strict mode is useful to write "secure" JavaScript by notifying "bad syntax" into real errors. 
      For example, it eliminates accidentally creating a global variable by throwing an error
      
68	How do you declare strict mode
      he strict mode is declared by adding "use strict"; to the beginning of a script or a function.
      
69	What is the purpose of double exclamation
70	What is the purpose of delete operator
      The delete keyword is used to delete the property as well as its value.
      
71	What is typeof operator
      You can use the JavaScript typeof operator to find the type of a JavaScript variable. It returns the type of a variable or an expression.
72	What is undefined property
      The undefined property indicates that a variable has not been assigned a value. 
      The type of undefined value is undefined.
      Any variable can be emptied by setting the value to undefined.

73	What is null value
      The value null represents the intentional absence of any object value. 
      It is one of JavaScript's primitive values. The type of null value is object. 
      You can empty the variable by setting the value to null.

74	What is the difference between null and undefined
75	What is eval
    The eval() function evaluates JavaScript code represented as a string. 
    The string can be a expression, variable, statement, or sequence of statements.
    example:console,log(eval('1+3'));
    
76	What is the difference between window and document
77	How do you access history in javascript
      The window.history object contains the browser's history. 
      You can load previous and next URLs in the history using back() and next() methods.
      you can access history with out window prefix.
      
78	How do you detect caps lock key turned on or not
79	What is isNaN
    The isNaN() function is used to determine whether a value is an illegal number (Not-a-Number) or not. i.e, 
    This function returns true if the value equates to NaN. Otherwise it returns false.

80	What are the differences between undeclared and undefined variables
81	What are global variables      
      Global variables are those that are available throughout the length of the code without any scope.

82	What are the problems with global variables
83	What is NaN property
84	What is the purpose of isFinite function
85	What is an event flow
86	What is event bubbling
        the event handled from the innermost element of target to the outer parent element is event bubbling.
        
87	What is event capturing
         the event handled from the outermost element of target to the inner child element is event capturing.

88	How do you submit a form using JavaScript
89	How do you find operating system details
90	What is the difference between document load and DOMContentLoaded events
    The DOMContentLoaded event is fired when the initial HTML document has been completely loaded and parsed, without waiting for assets(stylesheets, images, and subframes) to        finish loading. 
    Whereas The load event is fired when the whole page has loaded, including all dependent resources(stylesheets, images).

91	What is the difference between native, host and user objects
92	What are the tools or techniques used for debugging JavaScript code
93	What are the pros and cons of promises over callbacks
94	What is the difference between an attribute and a property
95	What is same-origin policy
96	What is the purpose of void 0
97	Is JavaScript a compiled or interpreted language
98	Is JavaScript a case-sensitive language
99	Is there any relation between Java and JavaScript
100	What are events
      Events are "things" that happen to HTML elements. When JavaScript is used in HTML pages, JavaScript can react on these events.
      example:*webpage finished loading
              *button was clicked
              *Input field was changed

101	Who created javascript
      JavaScript was created by Brendan Eich in 1995 during his time at Netscape Communications. 
      Initially it was developed under the name Mocha, but later the language was officially called LiveScript when it first shipped in beta releases of Netscape.

102	What is the use of preventDefault method
      it cancels the event if cancelable ,i.e defalult action or behaviour of event is not occurs.
      example:form submission is cancelled on clicking on submit button. 
      
103	What is the use of stopPropagation method
        it is used to prevent bubbling up of its event chain.
104	What are the steps involved in return false
        *First it stops the browser's default action or behaviour.
        *It prevents the event from propagating the DOM
        *Stops callback execution and returns immediately when called.
        
105	What is BOM
        The Browser Object Model (BOM) allows JavaScript to "talk to" the browser. 
        It consists of the objects navigator, history, screen, location and document which are children of the window. 
        it can change based on different browsers.

106	What is the use of setTimeout
        The setTimeout() method is used to call a function or evaluate an expression after a specified number of milliseconds. 
        
107	What is the use of setInterval
        The setInterval() method is used to call a function or evaluate an expression at specified intervals (in milliseconds). 
        
108	Why is JavaScript treated as Single threaded
        javaascript is single threaded language because  it has only one call stack that is used to execute the program
109	What is an event delegation
        event delegation is a technique for listening to events where you delegate a parent element as the listener for all of the events that happen inside it.
        example:
        
110	What is ECMAScript
        ECMAScript is the scripting language that forms the basis of JavaScript. 
        ECMAScript standardized by the ECMA International standards organization in the ECMA-262 and ECMA-402 specifications. 
        The first edition of ECMAScript was released in 1997.
111	What is JSON
        
112	What are the syntax rules of JSON
          *The data is in name/value pairs
          *The data is separated by commas
          *Curly braces hold objects
          *Square brackets hold arrays
          
113	What is the purpose JSON stringify
          it is used to convert object to string
          
114	How do you parse JSON string
          you can use JSON.parse() method to convert string to object
          
115	Why do you need JSON
        in exchanging data between a browser and a server, the data can only be text.
        JSON is text only, it can easily be sent to and from a server.
        
116	What are PWAs
        Progressive web applications (PWAs) are a type of mobile app delivered through the web, 
        built using common web technologies including HTML, CSS and JavaScript. 
        These PWAs are deployed to servers, accessible through URLs, and indexed by search engines.

117	What is the purpose of clearTimeout method
         it is used to cancel the setTimeout functions.
          
118	What is the purpose of clearInterval method
         it is used to cancel the setInterval functions.

119	How do you redirect new page in javascript
        you can redirect to a new page using the location property of window object.
        example:   window.location.href = 'newPage.html';

120	How do you check whether a string contains a substring
121	How do you validate an email in javascript
122	How do you get the current url with javascript
        You can use window.location.href expression to get the current url path.
        example:console.log(window.location.href); 

123	What are the various url properties of location object
124	How do get query string values in javascript
125	How do you check if a key exists in an object
        *Using in operator: 'key' in object
        *Using hasOwnProperty method: object.hasOwnProperty("key");
        *Using undefined comparison: object.property !== undefined
        
126	How do you loop through or enumerate javascript object
127	How do you test for an empty object
128	What is an arguments object
        The arguments object is an Array-like object accessible inside functions that contains the values of the arguments passed to that function. 

129	How do you make first letter of the string in an uppercase
         string.charAt(0).toUpperCase() + string.slice(1);
130	What are the pros and cons of for loop
131	How do you display the current date in javascript
132	How do you compare two date objects
            we can use use getTime() and the use comparison operators like this
            date1.getTime() === date2.getTime()
            
133	How do you check if a string starts with another string
            we can use String.prototype.startsWith() method to check if a string starts with another string or not.
            example: "good morning".statsWith('good');
            
134	How do you trim a string in javascript
            you can use trim method to trim white space in stats and end of the string
            example:"  Hello World   ".trim();
            
135	How do you add a key value pair in javascript
136	Is the '!--' notation represents a special operator
137	How do you assign default values to variables
            you can assign default value by || operator 
            example:var a = b || c;

138	How do you define multiline strings
        You can define multiline string literals using the '\' character followed by line terminator.
        example: var str = "This is a \
                  very lengthy \
                  sentence!";
                  
139	What is an app shell model
      An application shell (or app shell) architecture is one way to build a Progressive Web App.
      that reliably and instantly loads on your users' screens, similar to what you see in native applications. 
      It is useful for getting some initial HTML to the screen fast without a network.

140	Can we define properties for functions
          function is also a object . e can set property to it as same as object
          
141	What is the way to find the number of parameters expected by a function
          You can use function.length syntax to find the number of parameters expected by a function
          
142	What is a polyfill
          A polyfill is a piece of JS code used to provide modern functionality on older browsers.
          
143	What are break and continue statements
        *The break statement is used to "jump out" of a loop. i.e, It breaks the loop and continues executing the code after the loop.
        *The continue statement is used to "jump over" one iteration in the loop. i.e, It breaks one iteration (in the loop), 
        if a specified condition occurs, and continues with the next iteration in the loop.
        
144	What are js labels
        The label statement allows us to name loops and blocks in JavaScript. 
        We can then use these labels to refer back to the code later.
        
145	What are the benefits of keeping declarations at the top
        *Gives cleaner code
        *It provides a single place to look for local variables
        *Easy to avoid unwanted global variables
        *It reduces the possibility of unwanted re-declarations
        
146	What are the benefits of initializing variables
        *It gives cleaner code
        *It provides a single place to initialize variables
        *Avoid undefined values in the code
        
147	What are the recommendations to create new object
148	How do you define JSON arrays
          JSON arrays are written inside square brackets and arrays contain javascript objects. 
          example:"users":[
  {"firstName":"John", "lastName":"Abrahm"},
  {"firstName":"Anna", "lastName":"Smith"},
  {"firstName":"Shane", "lastName":"Warn"}
]
149	How do you generate random integers
        You can use Math.random() with Math.floor() to return random integers
        
150	Can you write a random integers function to print integers with in a range
          s, you can create a proper random function to return a random number between min and max (both included)

function randomInteger(min, max) {
  return Math.floor(Math.random() * (max - min + 1) ) + min;
}
randomInteger(1, 100); 

151	What is tree shaking
           Tree shaking or dead code elimination means that unused modules will not be included in the bundle during the build process.
           it can be done by bundlers like rollup and webpacks.
           
152	What is the need of tree shaking
153	Is it recommended to use eval
154	What is a Regular Expression       
        A regular expression is a sequence of characters that forms a search pattern. 
        You can use this search pattern for searching data in a text. 
        used to perform all types of text search and text replace operations
        
155	What are the string methods available in Regular expression
        *The search() method uses an expression to search for a match, and returns the position of the match.
        *The replace() method is used to return a modified string where the pattern is replaced.

156	What are modifiers in regular expression
157	What are regular expression patterns
158	What is a RegExp object
159	How do you search a string for a pattern
          You can use the test() method of regular expression in order to search a string for a pattern, and return true or false depending on the result.
          example:var pattern = /you/;
          console.log(pattern.test("How are you?")); //true
          
160	What is the purpose of exec method
          The purpose of exec method executes a search for a match in a specified string and returns a result array, or null.
          
161	How do you change style of a HTML element
           Using style property: You can modify inline style using style property
          document.getElementById("title").style.fontSize = "30px";
          Using ClassName property: It is easy to modify element class using className property
          document.getElementById("title").className = "custom-title";

162	What would be the result of 1+2+'3'
163	What is a debugger statement
        the debugger statement invokes any available debugging functionality, such as setting a breakpoint.
        If no debugging functionality is available, this statement has no effect.
164	What is the purpose of breakpoints in debugging
            breakpoint will stop executing of code and let you examine the JavaScript values. 
165	Can I use reserved words as identifiers
166	How do you detect a mobile browser
167	How do you detect a mobile browser without regexp
168	How do you get the image width and height using JS
169	How do you make synchronous HTTP request
170	How do you make asynchronous HTTP request
171	How do you convert date to another timezone in javascript
172	What are the properties used to get size of window
176 What is the difference between proto and prototype
        The __proto__ object is the actual object that is used in the lookup chain to resolve methods, etc. 
        Whereas prototype is the object that is used to build __proto__ when          you create an object with new
 178 What is a freeze method
        The Object.freeze() method freezes an object that prevents new properties from being added to it. 
        This method prevents the modification of existing property, attributes, and values.
179 What is the purpose of freeze method
              it is used to make object immutable.
185 What is a rest parameter              
          The rest parameter syntax allows a function to accept an indefinite number of arguments as an array.
          example:function f(a, b, ...theArgs) {
  // ...
}
188 What is a spread operator
        Spread operator allows iterables( arrays / objects / strings ) to be expanded into single arguments/elements
        example:function calculateSum(x, y, z) {
  return x + y + z;
}
const numbers = [1, 2, 3];
console.log(calculateSum(...numbers)); // 6

193 What are the applications of assign method
        *It is used for cloning an object.
        *It is used to merge objects with the same properties.

195 What is the purpose of seal method
        The Object.seal() method is used to preventing new properties from being added to it and marking all existing properties as non-configurable. 
        But values of present properties can still be changed as long as they are writable. 
        
197 What are the differences between freeze and seal methods
        In Object.freeze() method objects properties become immutable and no changes can be made in them 
        whereas the Object.seal() method changes can be made in the existing properties of the object.      
        
200 What is the main difference between Object.values and Object.entries method
        The Object.values() method's behavior is similar to Object.entries() method but it returns an array of values instead [key,value] pairs.
        
201 How can you get the list of keys of any object
      you can use object.keys() to get list of keys of object.
      
214 What is an anonymous function
        An anonymous function is a function without a name! Anonymous functions are commonly assigned to a variable name or used as a callback function.       

223 What are primitive data types
*string
*number
*boolean
*null
*undefined
*bigint
*symbol

226 What is an error object
An error is a built in error object that provides error information when an error occurs. 
It has two properties: name and message.

