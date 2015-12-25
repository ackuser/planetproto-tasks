Your submission results compared to the expected:

                 ACTUAL                                 EXPECTED
────────────────────────────────────────────────────────────────────────────────

   "[] == [] => true"                  ==    "[] == [] => true"
   "[] == [] => true"                  ==    "[] == [] => true"
   "[] == [] => true"                  ==    "[] == [] => true"
   "[] == [] => true"                  ==    "[] == [] => true"
   "[ 'core' ] == [ 'core' ] => true"  ==    "[ 'core' ] == [ 'core' ] => true"
   "[] == [] => true"                  ==    "[] == [] => true"
   "[ 'fly' ] == [ 'fly' ] => true"    ==    "[ 'fly' ] == [ 'fly' ] => true"
   "[ 'fly' ] == [ 'fly' ] => true"    ==    "[ 'fly' ] == [ 'fly' ] => true"
   ""                                  ==    ""

────────────────────────────────────────────────────────────────────────────────

✓ Submission results match expected
[] == [] => true
[] == [] => true
[] == [] => true
[] == [] => true
[ 'core' ] == [ 'core' ] => true
[] == [] => true
[ 'fly' ] == [ 'fly' ] => true
[ 'fly' ] == [ 'fly' ] => true
✓ exports Robot
✓ exports robby
✓ exports cranky
✓ Robot is a function
✓ robby is an instance of Robot
✓ cranky is an instance of Robot
✓ an instance of Robot defines parts
✓ an instance of Robot defines capabilities
✓ parts is an array
✓ capabilities is an array
✓ parts is initially empty
✓ finds an item in robby.parts
✓ first item in robby.parts is core
✓ finds zero items in cranky.parts
✓ capabilities is not directly added to robby
✓ capabilities is not directly added to cranky
✓ finds one item in robby.capabilities
✓ finds one item in cranky.capabilities
✓ finds fly in robby.capabilities
✓ finds fly in cranky.capabilities

# PASS

Your solution to 100 Function prototype passed!

Here's the official solution in case you want to compare notes:

────────────────────────────────────────────────────────────────────────────────
    function Robot() {
        this.parts = [];
    }

    Robot.prototype.capabilities = [];

    var robby = new Robot();
    var cranky = new Robot();

    claim(robby.parts, []);
    claim(cranky.parts, []);
    claim(robby.capabilities, []);
    claim(cranky.capabilities, []);

    robby.parts.push('core');
    robby.capabilities.push('fly');

    claim(robby.parts, ['core']);
    claim(cranky.parts, []);
    claim(robby.capabilities, ['fly']);
    claim(cranky.capabilities, ['fly']);

    module.exports = {
        Robot:  Robot,
        robby:  robby,
        cranky: cranky
    }

────────────────────────────────────────────────────────────────────────────────

You've finished all the challenges! Hooray!
