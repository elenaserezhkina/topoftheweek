# 🧠 topoftheweek  🧠



## Basic Java Script 
# Variables
#### 📦 Variables are containers for storing data values

### Declering variables : 
- unique name (identifiers)
- descriptive and short
- can contain letters, digits, underscores, and dollar signs.
- must begin with a letter
- or begin with $ and _ 
- case sensitive (y and Y are different variables)
- eserved words (like JavaScript keywords) cannot be used as names

### Data types :
- string
- number 
- boolean
- objects and more

### Declering variables 
### LET
this keyword signals that the variable can be re-assigned a different value (CAN be changed)
### CONST
CAN *NOT* be reassigned 
variables can be declared without a value

##### String concatanation with variables 
               let myName = "Melina";
               console.log("My name is "+ myName + " .");

##### String interpolation 
               const myName = "Linn";
               console.log( ` My name is ${myName} ` );


## ⭐ SCOPE ⭐
- defines where variable can be accessed or referenced

{...}block - cod found inside a set of curly brackets. Blocks help to group 1 or more statements together. 
### ⭐ 1. Global scope (global variables)
variables declared *outside* of the block. (can be accesed by any code in the program)

### ⭐ 2. Block scope (local variables)
variable defined *inside* of the block, it's only accesable from inside the block () withing curly brackets.(good practice)



### ✨✨Scope polution ✨✨
too many global variables in the global scope. Messy code



## Manipulating the DOM 
#### (Document Object Model) -the data representation of the objects that comprise the structure and content of a document on the web

### Selecting elements from HTML 

### 1. by ID
let element = document.getElementById("id")

### 2. by tag name
let elements = document.getElement*s*ByTagName("name")

### 3. by class 
let elements = document.getElement*s*ByClassName("name")

### Most useful  : 
 ❗   documents.querySelectorAll(".class")
return all elements withing that class (a collection, need to use loop to go through every element)

 ❗  documents.querySelectorAll("#tag")

### To manipulate html content 
ex:
- .innerHTML() - adding html tags
- .textContent() 
- .createElement()
- .removeChild()
- .appendChild()





## Arrays 
📦 = [🥝, 🍌, 🥚, 🍩];

Used to store multiple values in a single variable, in square brackets, can be storred in a variable.

0️⃣❗Arrays are zero-indexed: the first element of an array is at index 0 , and the last element is at the index equal to the value of the array's length property minus 1

Any type of data can be included in an Array :

          let myArray = ["example", 3, true, "another example but longer", 666 ]

### Accessing elements : 
      
               let myArray = ["example", 3, true, "another example but longer", 666 ]
               myArray[2] = true,
               myArray[4] = "666",
               (If you try to acces element on index 5 it will be undefined.)

### Accessing individual character :
          let hello = "welcome"
          console.log( hello[6] ) // output = e

### Update element : 

          let groceries = ["banana", "egg", "milk"];
          groceries[1] = "avocados";
          console.log(groceries)  // output = ["banana", "avocados", "milk"]
     
Most popular array methods (actions that can be used on arrays)
- .length
- .push()
- .pop()
- .shift()
- .unshift()
- .slice()
- .indexOf()
- .splice()

### List of methods :
https://www.w3schools.com/js/js_array_methods.asp

### Nested arrays - arrays containing other arrays 
ex:

              const myArray = [
                [1,2],
                [3,4],
                [5,6]
                [true, false],
                ["yes","no"]
            ];
            console.log(myArray[3,1])  // output true
            
            
            

more info : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array            






## Objects 
🚗: 
{🔑:100€,
🔑:red,
🔑🏎️: no};

#### store various keyed collections, almost everything can be an object, regular expressions, arrays, functions, objects are also objects :) 


Objects have *properties* (it can be a string, number, boolen etc ) and *methods* (actions that can be used on objects).

### syntax 
       let/const objectname = { 
              key : property ,
        };

Example :

          let avocado = {
                color inside : "white" ,
                color outside : "brown" ,
                origin: "New Zeland" ,
                taste: "omg"
           };

               let kiwi = {
                 color inside : "green" ,
                 color outside : "brown",
                 origin: "New Zeland",
                 taste: "yummy"
               };

#### Object methods include 
- Object.keys(), 
- Object.values(), 
- Object.create, 
- Object.assign() 
etc.

#### More on the topic : 
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object


### ⭕ Looping through objects (FOR ... IN LOOP) ⭕
example : 

                const student = {
                   name : "Yannic",
                   age : 25,
                   nationality : "swedish",
                   class2020 : true
                 };
 
                     for (const propName in student){
                            console.log(propName);
                      };
 
 more info: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for...in
 
 
 
 
 Useful links :) 
 1. https://developer.mozilla.org/en-US/
 2. https://www.w3schools.com/
 3. https://caniuse.com/#
 4. https://htmlcheatsheet.com/js/
 
 
 
 
 
 
 
 
 
 
 
 
