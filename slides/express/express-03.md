##  Express

    app.get('/dogs', function(req, res) {
      dogService.list(function(err, dogs) {
        res.json(dogs);
      });
    });
