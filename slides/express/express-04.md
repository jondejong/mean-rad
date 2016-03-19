##  Express

    app.get('/dogs/:id', function(req, res) {
      var id = req.params.id;

      dogService.fetch(id, fucntion(err, dogs) {
        res.json(dogs);
      });
    });
