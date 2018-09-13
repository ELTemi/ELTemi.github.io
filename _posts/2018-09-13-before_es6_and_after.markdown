---
layout: post
title:      "Before ES6 and After"
date:       2018-09-13 16:12:39 +0000
permalink:  before_es6_and_after
---


If you ever struggled with what Javascript  ES6 was about, here are some of the new features. Some of them are modifications from previous versions and some are new features.

**A. Type of Variables(var, let & const)**

Before ES6, you could only declare a variable using  *var*  like 

     `var name = "Temi"`
		 
With ES6, you can declare a variable using *let*  and *const* inside a block, 

`{
    let name = "Joseph" 
}`

            OR

`{
    const name = "Mary"
	}`
	
	Outside the block, the variable name retains the initial value 
	
	`name = "Temi"`
	
**B. 	Set Default Argument Values**

You can now set default parameter values when defining functions. 

```
function greeting(name = "Temi") {
    // name is Temi if not passed or undefined
    return `Hello ${name}`;
}
greeting(); // will return Hello Temi
greeting("Joseph"); // will return Hello Joseph
```

**C. Use Array.find()**

Array.find() returns the first result in an array based on the condition stated in the function.

```
var names = ["Temi", "Joseph", "John"];

function findName(value, index, array) {
    return value == "Temi";
}

names.find(findName) = Temi;
```

**D. Use Array.findIndex()**

Array.findIndex() returns the index of the array based on the condition stated in the function.

```
var names = ["Temi", "Joseph", "John"];

function findNameIndex(value, index, array) {
    return value == "Joseph";
}

names.findIndex(findNameIndex) = 1;
```

**E. Number.isInteger()**

The Number.isInteger() method returns a boolean if depending on the argument value

```
Number.isInteger("5") = false;

NumberisInteger(5) = true;
```

**F. Arrow Functions**

Before ES6, you would have to define a function using the *'function'* keyword. With ES6, a function can be expressed as ;

```
const nameFunction= (name) =>  { return `My name is ${name}`};

nameFunction("Adora") = My name is Adora;

```

They must be defined before they are executed. However, Arrow functions are not suitable for defining Object methods or classes because they do not have their own 'this'.



