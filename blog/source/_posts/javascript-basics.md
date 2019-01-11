---
title: Javascript Basics
date: 2018-12-17 22:44:19
tags:
- javascript 
- es6 
- common js 
- object oriented programming
---
Javascript has undergone numerous changes since its inception in 1995. After being introduced as a complementary aspect of web development alongside HTML and CSS, Javascript engines are now found in a number of web technologies from server-side web servers and databases to full scale native mobile application development. We take a deeper dive into the growth of Javascript through the scope of CommonJS and ECMAScript 6. 

## Javascript: The Beginnings and The Future 
![Diagram1](https://raw.githubusercontent.com/Developer-Handshake/Developer-Handshake.github.io/org-page/img-media/javascript.png)

After its origins from the NetScape architecture, JavaScript underwent a form of standardization in order to make it a more applicable scripting language for modern and future web technologies. This is known as the ECMAScript Standard, and **ECMAScript Version 6** -- or more commonly referred to as [ES6](http://es6-features.org/#Constants) -- is the current industry standard. 

_ES6_ introduces a number of new features and syntax for creating efficient and readable code such as arrow functions, template strings, class destruction, modules and more. 

```javascript 
const myFunc = greeting => {
    return 'Hello ${greeting}'; 
}

console.log(myFunc('World! This is ES6!')) // output => Hello World! This is ES6!
```
---
### ES6 and Modern Web Development 
There are a number of advantages that the ES6 standard has brought to javascript programming. Despite web browsers not having full feature support for ES6, the new Javascript standard is compatible with certain compilers that enable ES6 to be translated into ES5 when the web page or web application is rendered. 

#### Compilers to get you started
* [Babel](https://babeljs.io/) - Babel is a toolchain that is mainly used to convert ECMAScript 2015+ code into a backwards compatible version of JavaScript in current and older browsers or environments 
* [Sucrase](https://sucrase.io/) - Sucrase is an alternative to Babel that allows super-fast development builds. Instead of compiling a large range of JS features to be able to work in Internet Explorer, Sucrase assumes that you're developing with a recent browser or recent Node.js version, so it focuses on compiling non-standard language extensions 

![Diagram1]()

#### Advantages for Web Development
**Default Function Parameters** 
The ES6 standard comes with functionality that allows developers to create modular environments for their code. For example the implementation of **Default Function Parameters** in the ES6 standard allows for formal parameters to be initialized with default values if no value or undefined is passed. Previously _default function parameters_ were employed as such: 

```javascript 
var link = function (height, color, url) {
    var height = height || 10
    var color = color || 'green'
    var url = url || 'developer-handshake.github.io'
    ...
} 
```

However certain values being passed through functions with this setup would result in error. Typically developers could handle these one-off-occurrences through logic loops, but now with ES6 a rational alternative has already been built into the scripting language. Simply declare your default parameters while implementing the function: 

```javascript 
var link = function(height = 10, color = 'green', url = 'developer-handshake.github.io') {
    ...
}
```

