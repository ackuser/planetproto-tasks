Your submission results compared to the expected:

                 ACTUAL                                 EXPECTED
────────────────────────────────────────────────────────────────────────────────

   "true == true => true"              ==    "true == true => true"
   "true == true => true"              ==    "true == true => true"
   "{} === {} => true"                 ==    "{} === {} => true"
   ""                                  ==    ""

────────────────────────────────────────────────────────────────────────────────

✓ Submission results match expected
true == true => true
true == true => true
{} === {} => true
✓ exports a machine variable
✓ exports a robot variable
✓ exports a robby variable
✓ machine is the prototype of robot
✓ robot is the prototype of robby

# PASS

Your solution to 060 Object Create passed!

Here's the official solution in case you want to compare notes:

────────────────────────────────────────────────────────────────────────────────
    var machine = {}

    var robot = Object.create(machine);
    var robby = Object.create(robot);

    // -> What is the result of `machine.isPrototypeOf(robby)`?
    claim(machine.isPrototypeOf(robby), true);

    // -> What is the result of `robot.isPrototypeOf(robby)`?
    claim(robot.isPrototypeOf(robby), true);

    // -> Which object is the direct prototype of robby?
    claim.same(Object.getPrototypeOf(robby), robot);

    // ------------------------------------------------
    module.exports = {
        machine:  machine,
        robot:    robot,
        robby:    robby
    }

────────────────────────────────────────────────────────────────────────────────

You have 4 challenges left.
Type 'planetproto' to show the menu.
