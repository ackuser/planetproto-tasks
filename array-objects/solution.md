Your submission results compared to the expected:

                 ACTUAL                                 EXPECTED
────────────────────────────────────────────────────────────────────────────────

   "[] == [] => true"                  ==    "[] == [] => true"
   "[] == [] => true"                  ==    "[] == [] => true"
   "{} == {} => true"                  ==    "{} == {} => true"
   "{} == {} => true"                  ==    "{} == {} => true"
   "[ 'core' ] == [ 'core' ] => true"  ==    "[ 'core' ] == [ 'core' ] => true"
   "[ 'core' ] == [ 'core' ] => true"  ==    "[ 'core' ] == [ 'core' ] => true"
   "{ fly: true } == { fly: true } => true" ==    "{ fly: true } == { fly: true } => true"
   "{ fly: true } == { fly: true } => true" ==    "{ fly: true } == { fly: true } => true"
   ""                                  ==    ""

────────────────────────────────────────────────────────────────────────────────

✓ Submission results match expected
[] == [] => true
[] == [] => true
{} == {} => true
{} == {} => true
[ 'core' ] == [ 'core' ] => true
[ 'core' ] == [ 'core' ] => true
{ fly: true } == { fly: true } => true
{ fly: true } == { fly: true } => true
✓ exports a machine variable
✓ exports a robot variable
✓ exports a vehicle variable
✓ machine is the prototype of robot
✓ machine is the prototype of vehicle
✓ machine has a parts property
✓ machine has a capabilities property
✓ machine.parts is an array
✓ machine.capabilities is an object
✓ robot doesn't own parts directly
✓ vehicle doesn't own parts directly
✓ robot doesn't own capabilities directly
✓ vehicle doesn't own capabilities directly
✓ parts has exactly one item
✓ found core in parts
✓ capabilities has a fly property
✓ capabilities.fly is true

# PASS

Your solution to 050 Arrays and Objects passed!

Here's the official solution in case you want to compare notes:

────────────────────────────────────────────────────────────────────────────────
    var machine = {
        parts: [],
        capabilities: {}
    };

    var vehicle = {};
    var robot = {};

    robot.__proto__ = machine;
    vehicle.__proto__ = machine;

    // -> What is `robot.parts`?
    claim(robot.parts, []);

    // -> What is `vehicle.parts`?
    claim(vehicle.parts, []);

    claim(robot.capabilities, {});
    claim(vehicle.capabilities, {});

    robot.parts.push('core');

    claim(robot.parts, ['core']);
    claim(vehicle.parts, ['core']);

    vehicle.capabilities.fly = true;

    claim(robot.capabilities, {fly: true});
    claim(vehicle.capabilities, {fly: true});

    module.exports = {
        machine:   machine,
        vehicle:   vehicle,
        robot:     robot
    }

────────────────────────────────────────────────────────────────────────────────

You have 5 challenges left.
Type 'planetproto' to show the menu.
