12/29/20
Search for term using “/”, then enter visual mode to select it
Installed macvim, open with ctrl-cmd-v
Write quit from mac vim and it will copy automatically to clip board
ZZ saves and quits from normal mode

12/28/20
“Don’t save” shortcut on mac is command-backspace
⌘-p to open specific file vscode
⌘-. To open code actions in vscode, like the red squigglies
control-C goes back to normal mode in VIM
Control symbol is “^”
O “zero” to move to beginning of line, “$” to move to end
Can use visual mode with vimium in chrome
Visual mode selects text, like with a mouse
`dd` cuts an entire line, `p` pastes 


 
12/23/20
Installed fzf fuzzy finder
Installed git theme for bash

12/22/20
Dollar sign bash variables
Installed Coc and various vim javascript syntax highlighting / formatting
Installed tmux, Check this out for tmux commands

12/17/20
Need a different repository interface for every Entity (table)
Setting up ESLint and format on save
Eslint setup in create-react-app
What does Prettier do? It says it enforces consistent code style.
Cypress ESlint plugin
import cy from 'cypress' for error message eslint. UPDATE: DON’T DO THIS, IT BREAKS CYPRESS TESTS
Difference between Enzyme shallow wrapper and wrapper.instance()



12/16/20
`npm -D <package>` is a shortcut for `--save-dev`
Check out chapter 3, 4, 10 in this book for Git rebasing
12/15/20
Shortcut to initialize a hashmap in Java:


12/14/20
ERD is entity relationship model

12/11/20
Bluejay and StarUML best ways to learn java

12/10/20
Database transaction is a unit of work performed in a database
`PUT` is for updating an entire resource, `PATCH` is for updating certain attributes of a resource
Display last commit comment in git
Need single quotes for adding values in mysql insert statement
Communications link failure for mysql tests in java intellij
Create JSON-formatted string from java object
How to ignore properties on POJO on deserialization, check second answer and change to allowSetters=true so we can actually set the properties:
@JsonIgnoreProperties(value={ "password" }, allowSetters = true)
Working with multiple git user names SSH on mac

12/9/20
REPL stands for Read Eval Print Loop, and it’s a top level language shell
`describe <table name>` will show all columns from that table
`use <db name>` to connect to database from mysql rpl
`mysql -u<user name> <db name> < <file name>.sql` to run a file from shell
JPA is Java Persistence API and is an ORM for Spring to work with the database
Alt-D to quit mysql shell
mysql -u<user name> <db name> -e "<sql query WITH ;" to execute a single command and quit shell from the command line
Fintech is “financial technology”

12/7/20
cURL stands for Client URL
Command-7 in intellij to show methods in sidebar for class you are navigating
A Java class can implement many interfaces
A Java class can only inherit from one superclass, but can implement multiple interfaces
Having a “primary constructor” can simplify your constructor code. Just have all your various constructors refer to each other, from simplest to most complicated, by calling `this(...)` in each, until you arrive at your primary constructor
This primary constructor pattern removes code duplication and makes code easier to maintain
The primary constructor will never call `this`
You can generate a constructor with the generate shortcut in intellij
Data Access Object (DAO) is like a layer below an ORM
We use dependency injection to remove the `new` keyword as much as possible and we can make changes and decouple code in a very flexible way
Spring is an open source app framework for Java that offers an Inversion of Control Container.
Spring uses the @RestController and @RequestMapping annotations to build a controller layer of web apps
Usually you write declarative code for Spring, often with annotations and Spring figures out how to put it together.
Spring offers the web MVC framework.
Now, Spring Boot makes it easy to develop Spring. It has a bunch of pre configured build.gradle files, that for instance, have great test starter code that works out of the box.
The Spring Boot web starter brings in the Spring Web MVC.
Spring app initializer
Gradle bootRun starts the app with additional Spring Boot features, as contrasted with gradle run command
Http is the protocol
Google.com is the host (domain name)
#header is a hash, or anchor, not used in server side programming
/something/47 is the path, and sort=name&dir=desc is the query string
Query string comes after a ?
Ports are omitted in public facing URLs
Path starts with the /

Cookies are stored in the header
Data serialization is where you convert complex data structure objects in a byte stream for storage or for network transmission, like JSON.stringify()
Body of a server response could include the actual HTML
Images would be binary data

12/6/20
looks like app.listen() is just a wrapper for http.createServer() and doesn’t need to be at the end of the file. It just sets up an event listener on the event loop.

12/5/20
REST says you will always get the same piece of data from the same URL

12/4/20
In DevSecOps field, build time of less than 10 minutes considered good
Continuous Integration Continuous Delivery
`long` data type is 8 bytes. Use when you want a wider range of values than `int`
From a feature branch: `git push -u origin HEAD`. HEAD is reference to the current branch. `-u` sets upstream to remote specified (`origin`, here) so that whenever  the head is pointed to the feature/add-manager, you can just run `git push`
Static code analysis analyzes your code without running it



12/3/20
Classes in Java do not need to be defined with a constructor.
The constructor method is a special method that’s only called once (looks like you use the `this` keyword), and can set the fields of the instantiated object
If you have a constructor with arguments and you don’t pass arguments to an instantiated object, the compiler will throw an error
You can also set other fields in the class, even if they aren’t passed as arguments to the constructor
Unlike JavaScript, primitive variables are passed to methods as references, so they are only altered within the method. So, an int in a higher scope will not be changed in the scope from within a method
ArrayList is a dynamic array and can be resized, like a JavaScript array
An ArrayList is passed as a reference and will be modified on the outer scope if accessed from within a method’s inner scope
REST is an API architecture, CRUD is a database lifecycle pattern for supporting persistent data
Java this keyword references an internal field of the class
GraphQL is analogous to REST
A “like” on FaceBook will make HTTP requests
Looks like you can update a counter in state like this?

Java “getters” and “setters” are just normal instance methods that allow you to get and set private fields within an instance
Java classes can have multiple constructors, and you can call another constructor of the same class from within a constructor…
The above multiple constructors point looks like it’s an example of overloading methods, where you can have multiple methods within a class with the same name as long as they have different parameter lists
Maybe not a great idea to use overloaded methods for the sake of readability
Intellij: navigate - class => include non-project classes. You can check out a class like `Object` from the Java language. It’s like viewing the constructor for the class?
Java objects can only inherit from ONE superclass, but can inherit from multiple interfaces?
All Java top-level classes inherit from the Object class, and you can test this with `instanceof`



12/2/20
Use react.createElement('div', {className: 'App'}) to demonstrate why JSX is important:
Single responsibility for components in React
Import a css file into React
Java variables point to values, not other variables, just like JavaScript.
When you create a variable in Java, Java creates a stack frame that holds the actual bits bound to the variable name you gave it. When you create another variable and set it equal to the first variable, it will find the value of that first variable, and create a new stack frame for the second variable with the bit representation of that value, creating a new space in memory for the value, even though it’s the same. Thus, when you modify the first variable, the second variable’s value still points to the old, original value, unchanged.
Java Object types store a reference to the object. So if an object changes, all references will reflect that change.
Note: Java strings are immutable
When you create an object in Java, a new object is created on the heap
Variables you create, are just pointers to the objects location in memory. The variables don’t contain the actual object
Primitives start lowercase, Objects upper case
To build: ./gradlew build
Then,  you can run java -jar build/....path-to-jar.jar arg1 arg2
You need to instantiate a class in order to use a method contained within
Variables declared in a class are called fields. Declared traditionally private (only available within the class, not outside of it), like: `private String name = “John”;`
Class methods can access the private fields within a class, however.
An instance’s state is a snapshot of the current characteristics of an object
Whereas behavior describes what the object can do.
Intellij has a `toString` shortcut to give a class that method
Since we make the state private, you can only change the state via behaviors (methods)
12/1/20
You have to compile Java before you can run it. Write source code, compile it, run it.
Npx allows you to execute an npm package without modifying anything you already have installed
Yarn is a package manager like npm, but Facebook made it
I used ./gradlew build to build the project instead of gradle build
Java is statically typed, meaning that the compiler checks that your variable values match their declared types
String is an object type in Java. Use .equals to compare objects.
PlatformONE isn’t designed to create software devs. Platform ONE is a pipeline, infrastructure for deploying DOD software.
Platformone is like the military cloud.
CATO- continuous authority to operate. So you don’t have to get every change of code approved. Precursor to continuous deployment or delivery.

11/30/20
Value of i++ is the value of i BEFORE the increment
Java Spring is a server-side technology like Node.js
Node.js is a runtime, not a framework
Express is the web app framework for Node.js
Differences between Node.js and Spring boot
Node.js is non-blocking and single threaded. It relies on asynchronous code so that processes can operate while waiting on other processes to finish
Using a single thread means low memory usage.
Sounds like since Java Spring is better for CPU intensive tasks, whereas Node.js might be better for an app that has a lot of I/O because of it’s non-blocking nature
Java can be verbose and has a lot of boilerplate



11/25/20
`Array.apply() will call the Array constructor with the `this` context and arguments provided. The first argument here is length, so it will create an array of length 10. 
Array() can be used without the `new` keyword, and will create a new array based on what you pass in.
Great SO on this
Looks like apply() is parsing the arguments array by looking at the length (even though we are passing an object that we are giving a length property). WEIRD:



Function.call, of course, calls the given function with separate arguments provided with the given this value. Check it out: 

Naive implementation of .map. There IS a (Function.call).call there!
This concept is explained here
Function.call ITSELF inherits the .call method from Function.prototype!!!
The second .call() REBINDS the first one, so the following two code snippets are identical:

The above is basically saying “invoke .call with the context of console.log, providing null as the first argument and ‘test’ as the second, so: `console.log.call(null, ‘test’);
Explained in some of these answers.
The stupid Colt Steele code `array.map(Function.call, Math.random)`, Math.random() doesn’t even take arguments, so it’s literally just returning a random num between 0 and 1 for each element of the array. Why wouldn’t he just do: `array.map((e) => Math.random());`???? Puzzling. 
11/24/20
JS native sort, without a compare function, will convert array elements to string and compare their native unicode code values

11/22/20
Use `for of` loop (usually used for non-objects) with Object.entries (which returns key/value pairs) to shorthand declare key/value pairs when iterating through an object:

Check out how it returns an array of arrays of Key/value pairs:

Array.concat() returns a NEW ARRAY!!! Doesn’t modify the old array
Spread operator (`...` used in a function invocation like `array.push(...values)` used with an iterable will ‘spread’ out the arguments: `...[‘hello’, ‘world’] === ‘hello’, ‘world’`
The reason `array.push(...anotherArray)` works is because `array.push` takes multiple arguments!!

11/21/20
Array.concat() creates a NEW array. Doesn’t alter existing arrays.
Package.json should be single source of truth
^ in package.json updates to newest MINOR version

11/20/20
Mongo Compass is the Mongo GUI, also cloud
Can export the mongo db using CLI to JSON file
Mongo DB React Docker Express guide

11/18/20
Pop function off the call stack by `return`ing
Stack overflow, or maximum call stack size exceeded means you aren’t stopping a recursive call

11/17/20
JSON.parse and stringify are examples of recursive functions, along with getElementById
Call stack is a data structure (duh, a Stack)
Snippets are one shot, when you run something it is added to the page. Need to reload.
Maybe make an empty.html and edit it using Chrome filesystem to check code.
Restart frame with Dev Tools! Let’s you go back in time.

11/16/20
Jamboard for whiteboard, alternative to aww app.

11/15/20
Subtraction takes precedence over addition `1 - 2 + 1 !== 1 - (2 + 1)`
11/14/20
Wifi calling on ipad popup. Tried turning off setting on iphone and restarting ipad.
Using 2 pointers if you are given a sorted array. Move the pointers when you reach a certain condition, since the array is sorted.

Previous example works from the far right side and the far left side toward the middle
Sliding window:



11/13/20
Feedback from practice teach at Galvanize:
Cold calling students, making sure everyone is participating. Amp up the interaction with the students a lot!
Using ES6 arrow-functions.
Sell students on why something is needed and important
Index, optional stuff is unnecessary toward achieving lesson objective, rather give the students a chance to write their own map function, maybe with a slightly different example
Don't let students rabbit hole me, we can talk about that after the lesson
"Great question. What do you think is going to happen?" - good things to say.
Don’t call them rules, always refer to the documentation. Even show them the documentation
Mongo will create a collection for you with `const <name> = mongoose.model(..., schema)

11/10/20
Great question reminding that variables point to values, not other variables, in JavaScript

11/9/20
Fed-proof VPN would be VPS in Switzerland and set up a VPN client there, something with decent encryption like WireGuard

11/8/20
`df -h` will show available disk space in a human readable format. Stands for ‘disk free’
Remove multiple directories with `rm -rf <dir1> <dir2> etc..`

11/7/20
Body parser is needed to decode form POST requests
Form is sent with header CONTENT TYPE is urlEncoded
Body parser will add this to the body property on the body



11/6/20
cURL creates network requests from the command line
Simply providing a URL will perform a GET request and cURL will output the body of the response
cURL basic info
`mysql -u root -p -h127.0.0.1`. Mysql command looks for temporary socket file to find where host is. Using -h overwrites the looking for host. This is only for entering shell from terminal. Node should be fine because you will be setting the host manually when connecting

11/5/20

Map for an object’s keys in native JS
Video about DNS
OSI Model
What is launchCTL with regards to mySQL?

11/4/20
What is the advantage of using a prototypal pattern over functional-shared methods? Other than being able to check what a constructor function’s prototype is?
The issue with functional shared methods is that objects already created with the functional shared pattern will have certain methods. If you update the methods after creation, these objects’ methods will NOT be updated? Prototypal uses the prototype chain, so you can update the methods and all objects, even those already created, will have updated methods

11/3/20
Terminated (deleted) AWS instances. Everything! I was still incurring charges for going over the 30gb a month storage.

11/2/20
`sudo service stop` on WSL instead of `systemctl` (system controller). WSL does have systemctl, but you start and stop services using `service` instead.
Clear terminal with `clear`
Systemctl is a systemd command. WSL runs with System V (systemd)
Systemctl is there, but not for running commands in the background.
Draw.io
Plantuml for diagrams
Ondras.zarovi.cz for sql diagrams (sql designer)



10/31/31
Galvanize tech interview apparently is OoP, create a class and add methods one-at-a-time to conform to tests, like sprints
Make sure to type out the whole variable name
Binary Search Tree: all left nodes are less than parent node, all right nodes are greater than parent node
`super()` calls the parent constructor with the supplied arguments
`get` sets a property on the object equal to a function. Basically, it binds a function to a property, so:  

Instead of assigning a function like: 

Super keyword calls parent constructor with given arguments
Using res.redirect or res.render, Looks like res.render is usually appropriate for your app, unless it is a login page.
Pseudoclassical inheritance: `ParentClass.call(this, [args for parent constructor])` in the constructor of the child:

`fs.readdir` to read the contents of a directory

10/30/20
`mysql -u root` logs me in without a password
Use `Array.from({length: n}, () => [])` to create an empty array of arrays. Uses the Array.from mapping parameter

10/29/20
Distributed system is one where the components are located on different networked computers that communicate with one another

10/27/20
Check out optional chaining for JS objects
RESTful meaning: stateless (session info kept entirely on client and all useful request information stored in request TO server (not on server)), Separate user interface from data storage concerns (client-server), Cacheable data in a response that can be reused later
Resource methods are sometimes conflated with HTTP methods like POST, PUT, DELETE, GET, etc. But the only RESTFUL constraint is that whatever method you are using is consistent. So if you want to update a resource with POST, that’s fine, just use that across the board.
HTTP is stateless meaning each request is understandable by itself.
Check how to implement a promise!
100ms or less server latency is good. Anything higher than 500ms is not acceptable.
SSR will not necessarily improve server RPS, scaling definitely WILL improve it.
Scrum sprints are usually longer than XP sprints
Scrum doesn’t prescribe engineering best practices. XP does, like pair programming, TDD, refactoring, automated testing, etc.
HTTP is RESTful, but REST doesn’t necessarily mean HTTP
HTTP is stateless, meaning the server doesn’t keep any data (state) between two requests
REST is design constraints for efficient, reliable, and scalable systems.
^^ Standardized client/ server interactions
However, beginners can associate HTTP with REST, even though HTTP doesn’t necessarily adhere to all REST principles
10/26/20
Difference between ARM and x86: x86 is usually for peak performance and ARM is for energy efficiency
10/25/20
Square number is another name for a perfect square
10/24/20
NGINX default configuration files precendence

10/23/20
Why would you choose/do you like JS for Server or Front End applications? First of all, what other choice is there for the front end - JavaScript is the most popular language in the world. For the back end, since JavaScript is single threaded, there are more performant languages if that is what you need it for. However, it is incredibly easy to get started with Node, very little boilerplate code to write, quick to get a full-stack app up and running.
`nvm default alias v12`, check for VSCode debugger. `nvm --help`.
All globals are per node version so you may need to install globals again if you switch
Node v12 is a stable version right now.


10/22/20
When you don’t know a particular technology X in an interview: Say “I’m not familiar with technology or concept x, can you tell me something else it’s similar to?”
How can you explain event delegation? Event handler will bubble up from child elements
Undefined is a type and null is an object
JS variables declared with `var` can be used before declaration

10/17/20
Restate problem in your own words
All JS types except strings are mutable

10/15/20
What is a priority queue?
Edit distance, O(n), classic dp problem needleman-musnch algo (bottom up approach). Opposite of recursive?
Dp: relate current problem to previous sub problems
KMP algo for “sliding window” String Matching problem
Anagram and palindromes: sort string and compare each letter or use a frequency counter
Palindrome: two pointers toward the middle
Bidirectional Breadth First Search for Meet in the Middle graph
Informed Search?
Learning tips: Make sure you understand the problem completely, don’t confuse two similar problems. Look for keywords (max min, minimum path), 
Extremely important to diagram thought process
Frequency is most important thing, a little bit every day
Study the algorithms
Udemy JS algorithms and data structures course

10/12/20
JS strings are immutable: Can’t do: var string = “aab”; string[0] = “c”; ⇐ won’t change string
Using prototype chain saves memory because you aren’t creating a function with every instance of the class
__proto__ is the actual object used in the lookup chain to resolve methods, etc.
Object.create() sets up prototype delegations just like `new` does, but without running the constructor function in the process

10/11/20
This amazing reduce function that reduces an array to an object:


10/10/20
Parse CSV into address book, add simple filters - separate concerns, separate into classes
Difference between VM and Docker container?
Difference between dual boot and VM?
“tell me about a time that your really struggled to understand something”
Stay away from front-end only “marketing agency” type jobs

10/9/20
O (log n) usually refers to O (log 2 n)
Slicing an array: O(n) time and space
Call stack made up of stack-frames, one for each function call
Recursive functions can quickly fill a call stack, while an iterative solution might take up O(1) space by contrast
In place function modifies the input passed into it. This means it modifies objects or data structures outside of it’s stack frame. Also called a destructive algorithm. In place is a good way to save time and space.
An in place function that modifies an array doesn’t even need to return it, since the original array was modified.

The previous picture’s console log would show that the array was mutated, even without a return statement
JavaScript arrays are dynamic arrays
10/8/20
Set up 15-20 minute meetings at companies that have Hack Reactor grads working for them
Conferences are now virtual and often free, like Chaos conference right now
Bullets for negotiating without any competing offers: Teaching experience, mentoring junior engineers, leadership from SDC and SEIRship.
Dallas Meetup
Practice typescript, hooks, angular, once for each week. For frontend
Practice algorithms if you want to do back-end
order of events when loading a page:
browser loads html
html says “go get javascript”
browser gets javascript
browser runs javascript
javascript says “make ajax call”
browser makes ajax call
browser gets json response
browser provides json response to javascript
javascript renders cool new stuff on to DOM based on whatever json response comes back
once all js is run, browser/javascript sit idly until a user interaction happens
fwiw localhost:3000/index.html cannot respond with BOTH the contents of index.html AND JSON info from the database unless SSR has been implemented
rule of thumb: an endpoint should do just 1 thing/respond with 1 thing, and 1 thing only
Time cost of a binary search is O(log 2) n
Sorting, best “worst” case is O(n log 2) n



10/7/20
2 independent loops (not nested) will by O(2n) time, and we drop the coefficient, so it’s still O(n) time
You choose the worst time complexity, so if something was O(n^3 + n + n/2), we would reduce it to O(n^3)
Each memory address in RAM holds 8 bits
8 bits is a byte
RAM is connected to the processor via a Memory Controller that has a direct connection to every memory address in RAM, so it doesn’t take any extra time to access distant addresses
Processor has a cache that stores things recently read from RAM, much faster to read than accessing RAM directly
Nearby memory addresses are sent to the processor cache along with the requested memory from the memory controller, so nearby memory addresses are quick to access from programs
Therefore, reading form sequential memory addresses is faster than jumping around, since they are stored in the processor cache
2^0 = 1, 2^1 = 2, 2^2 = 4, etc.
Unsigned is non-negative
Hex numbers are sometimes prefixed with 0x or #
With n bits, you can express 2^n possible numbers
4 bytes (32 bits),  8 bytes (64 bits)
RAM is basically an array
Basic math operation on fixed-width integers takes O(1) time
Looking up contents of an array index is O(1) time (since it’s a simple math operation on the memory address of the first index of the array)
Each item of the array needs to be the same size, and you need a block of uninterrupted memory to store the array
0000 0000 is a byte (8 bits)
Mapping of numbers to characters is a character encoding, like ASCII
String is just an array of 8-bit characters
We can store pointers, which are integers that represent another memory address, in an array so that we can store arbitrarily large items in an array. An array of pointers.
Pointer based array is slower than an array that holds all the actual values, since the pointer addresses aren’t cached, though this isn’t reflected in the O(1) time cost
Dynamic array can be resized when needed — this is what JavaScript uses for its arrays. Lower level languages like C need to declare how much space an array will take up when they are created
Strictly speaking dynamic array appends might not be O(1) time since their size may need to double to account for new times, but we say on average it is O(1) for a dynamic array append. However, some appends for dynamic arrays could end up being expensive
What is a data structure that has fast appends and doesn’t require you to say how big the structure will be ahead of time?
The `next` in a linked list is a pointer to a place in memory
Tail could be the end of the list, OR anything after the tail
To add to the tail, use the tail pointer to grab the last node in O(1) time, point the `next` of the previous last letter to the new last letter, and point the tail to the new last letter
So, adding to the tail is O(1) time since it doesn’t matter how big the string is
Linked list worst case append is 0(1), while dynamic array worst case is O(n) since it may need to double its size and copy all elements to the new address in memory
To append to the beginning of a linked list, you need to point the head to the new first node, and point the new first node to the old first node
Prepending to a dynamic array is always O(n) time because you always need to move the older elements over in memory to make room for the new beginning element
Linked list nodes can go anywhere in memory
However, lookup in a linked list is O(ith) item lookups



10/6/20
Binary Search Tree: left child has keys that are less than the parent node’s value. Right children have only values greater than the parent node:

Different than a min heap because the Min heap’s parent value is always less than it’s children

9/30/20
If you set an index on an array higher than the current max length, it will create `empty` spaces in the array:


9/29/20
string.replace() will replace the FIRST occurrence of a string, not all occurrences:

string.replace() also returns a NEW string. It doesn’t modify the original string.



9/28/20
Do you add to the tail of a linked list first (instead of adding to the head)?

If there’s only one node in the linked list, both the head and the tail will point to the same value

But when you add a second node, the tail will now point to that second node

9/26/20
Flux design has a single state object for sole source of truth in the app. Redux is an example of this paradigm
Thunk functions pass through a reducer function which defines how each action alters state.
A thunk is a function
Redux-thunk is a middleware that looks at every action passing through a system, and if it’s a function, it calls that function
Redux passes the `dispatch` function to thunk functions, so it can dispatch new actions if it needs to
Container components are smart components
Presentational components are dumb components
Connected component is a parent component that renders your component as a child
mapStateToProps generates some props for your component to use
mapDispatchToProps does anything to pass functions that are used directly as event handlers
Using fetch API with query string
Had use the response.json() method to read the response stream and parses body text as JSON
Fetch is like XMLHttpRequest (XHR) but it utilizes promises.
You shouldn’t mutate the state inside the reducer function
Redux builds a predictable state container
What is the difference between these two `Object.assign`s? Apparently the first one will not be an acceptable reducer in redux. Maybe has something to do with mutating?

Can NOT pass `undefined` as an action to a reducer, but CAN pass an empty {}

9/23/20
Followed these steps to remove folder from git history and git ignore, but still file is not greyed out in VScode
Installing yarn via homebrew
Installed but could not figure out debug visualizer for the time being



9/22/20
Add chrome extension to detach tab from window ALT X
Standard Operating Procedures

9/20/20
Installed vim bindings for chrome
Check out vim bindings at some point
https://github.com/philc/vimium/blob/master/README.md, check for chrome vim bindings 

9/19/20
Storing images and demos in repo

