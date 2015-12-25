Your submission results compared to the expected:

                 ACTUAL                                 EXPECTED
────────────────────────────────────────────────────────────────────────────────

   "true == true => true"              ==    "true == true => true"
   "2 == 2 => true"                    ==    "2 == 2 => true"
   ""                                  ==    ""

────────────────────────────────────────────────────────────────────────────────

✓ Submission results match expected
true == true => true
2 == 2 => true
✓ exports a Robot variable
✓ exports a robby variable
✓ Robot is a function
✓ robby is an instance of Robot
✓ robby has property motors
✓ robby.motors is 2
✓ defines robby.motors inside the constructor

# PASS

Your solution to 080 Constructor functions passed!

Here's the official solution in case you want to compare notes:

────────────────────────────────────────────────────────────────────────────────
    function Robot() {
        this.motors = 2;
    };

    var robby = new Robot();

    claim((robby instanceof Robot), true);
    claim(robby.motors, 2);

    module.exports = {
        Robot:   Robot,
        robby:   robby
    }

────────────────────────────────────────────────────────────────────────────────

You have 2 challenges left.
Type 'planetproto' to show the menu.
