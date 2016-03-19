##  Express

    app.get('/api', function(req, res, next) {
      if(isValid(req)) {
        next();
      } else {
        req.sendStatus(422);
      }
    });

    app.get('/api/dogs', dogController.list);
