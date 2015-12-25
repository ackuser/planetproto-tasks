Your submission results compared to the expected:

                 ACTUAL                                 EXPECTED
────────────────────────────────────────────────────────────────────────────────

   "4 == 4 => true"                    ==    "4 == 4 => true"
   "true == true => true"              ==    "true == true => true"
   ""                                  ==    ""

────────────────────────────────────────────────────────────────────────────────

✓ Submission results match expected
4 == 4 => true
true == true => true
✓ exports a machine variable
✓ exports a robot variable
✓ exports a robby variable
✓ machine is the prototype of robot
✓ robot is the prototype of robby
✓ machine defines motors
✓ robot defines friendly
✓ friendly is defined in the robot object

# PASS

Your solution to 020 Proto passed!

Here's the official solution in case you want to compare notes:

────────────────────────────────────────────────────────────────────────────────
    var machine = {
        motors: 4
    };

    var robot = {
        friendly: true
    };

    var robby = {};

    robot.__proto__ = machine;

    robby.__proto__ = robot;

    claim(robby.motors, 4);

    claim(robby.friendly, true);

    module.exports = {
        machine: machine,
        robot:   robot,
        robby:   robby
    }

────────────────────────────────────────────────────────────────────────────────

You have 8 challenges left.
Type 'planetproto' to show the menu.
