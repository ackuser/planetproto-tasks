
Your submission results compared to the expected:

                 ACTUAL                                 EXPECTED
────────────────────────────────────────────────────────────────────────────────

   ""                                  ==    ""

────────────────────────────────────────────────────────────────────────────────

✓ Submission results match expected
✓ exports a Robot variable
✓ Robot.new is defined
✓ Robot.new is a function
✓ Robot.new returns an object
✓ Robot is the prototype of robby

# PASS

Your solution to 070 Dot New passed!

Here's the official solution in case you want to compare notes:

────────────────────────────────────────────────────────────────────────────────
    var Robot = {
        new: function () {
            return Object.create(this);
        }
    }

    module.exports = {
        Robot: Robot
    }

────────────────────────────────────────────────────────────────────────────────

You have 3 challenges left.
Type 'planetproto' to show the menu.
