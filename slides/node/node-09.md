#  Node
## Roll Your Own
### thing.processor.js

    var process = function(thing) {
      thing.value = thing.value * 2;
    };

    module.exports = {
      process: process
    };

### Use

    var thing = {value: 2};
    require('./thing.processor').process(thing);
    console.log(thing.value); //4
