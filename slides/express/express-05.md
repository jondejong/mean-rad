##  Express

    app.get('/dogs/:id', function(req, res) {

      // Depends on bodyParser
      var dog = {
        name: req.body.name,
        breed: req.body.breed
      }

      dogService.save(dog, function(err, dogs) {
        res.json(dogs);
      });
    });
