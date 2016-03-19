##  Node
### Promises

    var handleSuccess = function() {
      console.log('good things happened');
    };

    var handleError = function() {
      console.log('bad things happened');
    };

    thingService.getThings().then(handleSuccess, handleError);
