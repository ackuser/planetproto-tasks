Understanding JavaScript prototypes
─────────────────────────────────────
080 Constructor functions
Exercise 8 of 10


## Constructor Functions

Constructor functions are the most used way in JavaScript to construct prototype chains. The popularity of constructor functions comes from the fact that this was the only original way for constructing types initially.
Also many engines are highly optimized for constructor functions.

In JavaScript you can create an object like this:

   function Alien() {
       this.age = 10;
   }

   var zippy = new Alien();

When used with the keyword new functions behave like factories, meaning that they create new objects.
The new object they create is linked to the function by its prototype, more on this later. So in JavaScript we call this an instance of the function.

   // zippy is an instance of Alien
   console.log(zippy instanceof Alien); //=> true

## Challenge

Follow the instructions in the boilerplate file created.
A file 080.js with the necessary boilerplate has been created for you.


» To print these instructions again, run: planetproto print
» To execute your program in a test environment, run: planetproto run program.js
» To verify your program, run: planetproto verify program.js
» For help run: planetproto help
