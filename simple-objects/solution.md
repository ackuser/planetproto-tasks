Your submission results compared to the expected:

                 ACTUAL                                 EXPECTED
────────────────────────────────────────────────────────────────────────────────

   "true == true => true"              ==    "true == true => true"
   ""                                  ==    ""

────────────────────────────────────────────────────────────────────────────────

✓ Submission results match expected
true == true => true
✓ exports a robot variable
✓ robot defines smart
✓ robot.smart is true

# PASS

Your solution to 010 Simple objects passed!

Here's the official solution in case you want to compare notes:

────────────────────────────────────────────────────────────────────────────────
    var robot = {
        smart: true
    }

    claim(robot.smart, true);

    module.exports = {
        robot: robot
    }

────────────────────────────────────────────────────────────────────────────────

You have 9 challenges left.
