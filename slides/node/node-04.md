##  Node
### Error Callback

    var things = [];
    thingService.getThings(function(err, data) {
      if(err) {
        console.log('no good, very bad thing: ', err);
      } else {
        things = data;
      }
    });
