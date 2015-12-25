Your submission results compared to the expected:

                 ACTUAL                                 EXPECTED
────────────────────────────────────────────────────────────────────────────────

   "undefined == undefined => true"    ==    "undefined == undefined => true"
   "undefined == undefined => true"    ==    "undefined == undefined => true"
   "4 == 4 => true"                    ==    "4 == 4 => true"
   "4 == 4 => true"                    ==    "4 == 4 => true"
   ""                                  ==    ""

────────────────────────────────────────────────────────────────────────────────

✓ Submission results match expected
undefined == undefined => true
undefined == undefined => true
4 == 4 => true
4 == 4 => true
✓ exports a machine variable
✓ exports a robot variable
✓ exports a vehicle variable
✓ machine is the prototype of robot
✓ machine is the prototype of vehicle
✓ vehicle doesn't define motors directly
✓ robot doesn't define motors directly
✓ machine.motors is 4

# PASS

Your solution to 030 Dynamic lookups passed!

Here's the official solution in case you want to compare notes:

────────────────────────────────────────────────────────────────────────────────
    var machine = {}
    var vehicle = {}
    var robot = {}

    vehicle.__proto__ = machine;
    robot.__proto__ = machine;

    // What is vehicle.motors
    claim(vehicle.motors, undefined);
    // What is robot.motors?
    claim(robot.motors, undefined);

    machine.motors = 4;

    // -> What is `vehicle.motors` now?
    claim(vehicle.motors, 4);

    // -> What is `robot.motors`?
    claim(robot.motors, 4);

    // ------------------------------------------------
    module.exports = {
        machine: machine,
        vehicle: vehicle,
        robot:   robot
    }

────────────────────────────────────────────────────────────────────────────────

You have 7 challenges left.
Type 'planetproto' to show the menu.
