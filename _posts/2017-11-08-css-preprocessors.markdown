---
title:  "CSS preprocessors"
date:   2017-11-08 10:17:54 +0100
categories: sass
image: images/sass.png
---
By using a css preprocessor, you can simplify the way you write your css. You can make your stylesheets more concise, easier to read and maintain. There are many different css processors out there, but sass, less and stylus are currently the most widely used. 

This blogpost will focus on sass, but the syntax and functionality for all three are pretty similar. Furthermore, sass has two different syntaxes, called sass and scss. I will focus on the scss syntax, which is most similar to regular css.

**sass**

sass is probably the most widely used css preprocessor today. A great way of figuring out if something is for you, is a pros and cons list, so here we go!
pros
* Variables. You can define and use variables. This proves very convenient when working with colors, as you can apply different shades of the same color throughout your code. It is also useful when working with fixed widths, or just simply for code reuse.
* All css is valid sass. This means you can start using sass in the midde of your project. Just move your css to a sass-file, and slowly start integrating more sass features as you go.
* Built in functions, such as the color functions “lighten” and “darken”. you can probably figure out what they do!
* Nesting css selectors. No more repeating the same selectors over and over.
* Mixins. Mixins can accept arguments and do calculations. They can then output a css rule, or many.
* Functions. Similar in nature to mixins, however the output from a function is a single value, which can be any valid sass datatype (number, string, color, boolean or list).
* Operators. Math operators like +, -, *, / and % simplify doing calculations.
* Linting. Since sass needs to compile down to css, it has to go through a compiler. This means that if you have any syntax errors in your sass, it won’t compile, and instead give you a useful error message. CSS on the other hand swallows errors and ignores anything that’s not valid css. Linting definitely speeds up development.

**cons**

* Another layer of abstraction. Your code needs to compile down to valid css before it can be displayed on your site. This introduces a build step, which adds complexity and waiting time.
* New syntax. Sass brings with it new syntax, which you need to learn and understand.
In the project made to create this site, I used all the points I listed under pros, in other words: variables, mixins, operators, nesting and functions.

