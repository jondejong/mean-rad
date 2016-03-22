## Mongo
### Mongoose

    dogController.list = function(req, res) {
      Dog.find(req.query, function(err, list){
        res.json(list);
      });
    };

    dogController.save = function(req, res) {
      var dog = new Dog();
      dog.name = req.body.name;
      dog.breed = req.body.breed;
      dog.age = req.body.age;

      dog.save(function(err) {
        res.json({
            message: dog.name + ' has been added.'
          });
      });
    };
