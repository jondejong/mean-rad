## Mongo
### Native driver

    mongoClient.connect(config.mongo.url, function(err, db) {
      if (err) {
        console.log('error connecting to MongoDB', err);
      } else {
        // Access the db
      }
    });
