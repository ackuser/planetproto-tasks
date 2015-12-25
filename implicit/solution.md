Your submission results compared to the expected:

                 ACTUAL                                 EXPECTED
────────────────────────────────────────────────────────────────────────────────

   ""                                  ==    ""

────────────────────────────────────────────────────────────────────────────────

✓ Submission results match expected
✓ exports a Robot variable
✓ exports a Vehicle variable
✓ Robot is a function
✓ Vehicle is a function
✓ new Robot() returns an instance of Robot
✓ new Vehicle() doesn't return an instance of Vehicle

# PASS

Your solution to 090 Implicit this passed!

Here's the official solution in case you want to compare notes:

────────────────────────────────────────────────────────────────────────────────
    function Robot() {

    }

    function Vehicle () {
        return {};
    }

    module.exports = {
        Robot:    Robot,
        Vehicle:  Vehicle
    }

────────────────────────────────────────────────────────────────────────────────

You have one challenge left
Type 'planetproto' to show the menu.
