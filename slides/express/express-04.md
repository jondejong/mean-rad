##  Express

    app.get('/dogs/:id', function(req, res) {
      var id = req.params.id;

      dogService.fetch(id, function(err, dogs) {
        res.json(dogs);
      });
    });
