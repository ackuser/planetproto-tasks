Your submission results compared to the expected:

                 ACTUAL                                 EXPECTED
────────────────────────────────────────────────────────────────────────────────

   "null == null => true"              ==    "null == null => true"
   "null == null => true"              ==    "null == null => true"
   "null == null => true"              ==    "null == null => true"
   "null == null => true"              ==    "null == null => true"
   "4 == 4 => true"                    ==    "4 == 4 => true"
   "null == null => true"              ==    "null == null => true"
   ""                                  ==    ""

────────────────────────────────────────────────────────────────────────────────

✓ Submission results match expected
null == null => true
null == null => true
null == null => true
null == null => true
4 == 4 => true
null == null => true
✓ exports a machine variable
✓ exports a robot variable
✓ export a vehicle variable
✓ machine is the prototype of robot
✓ machine is the prototype of vehicle
✓ machine defines an own property motors
✓ machine.motors is null
✓ robot has an own property motors
✓ robot.motors is 4

# PASS

Your solution to 040 Property assignments passed!

Here's the official solution in case you want to compare notes:

────────────────────────────────────────────────────────────────────────────────
    var machine = {
        motors: null
    };

    var vehicle = {};

    var robot = {};

    // -> Let's make machine the prototype of robot and vehicle
    vehicle.__proto__ = machine;
    robot.__proto__ = machine;

    claim(machine.motors, null);
    claim(robot.motors, null);
    claim(vehicle.motors, null);

    robot.motors = 4;

    claim(machine.motors, null);
    claim(robot.motors, 4);
    claim(vehicle.motors, null);

    module.exports = {
        machine: machine,
        vehicle: vehicle,
        robot:   robot
    }

────────────────────────────────────────────────────────────────────────────────

You have 6 challenges left.
Type 'planetproto' to show the menu.
