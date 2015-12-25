Understanding JavaScript prototypes
─────────────────────────────────────
050 Arrays and Objects
Exercise 5 of 10


## Arrays and objects in prototypes

Arrays and objects may not behave as you expect them to behave.

Let's see what happens when you modify an array:

   var alien = {
       skills: ['morph']
   };

   var zorg = {};
   zorg.__proto__ = alien;

   zorg.skills.push('clone');

   console.log(zorg.skills);
   //=> morph, clone
   // we expected this

   console.log(alien.skills);
   //=> morph, clone
   // maybe we didn't expect this, but it works like that
   // because we have modified the array in the prototype object.

When you change an array or an object you make the change directly on the object.

## Challenge

Follow the instructions in the boilerplate file created.
A file 050.js with the necessary boilerplate has been created for you.


» To print these instructions again, run: planetproto print
» To execute your program in a test environment, run: planetproto run program.js
» To verify your program, run: planetproto verify program.js
» For help run: planetproto help
