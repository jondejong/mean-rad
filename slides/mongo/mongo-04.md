## Mongo
### Native driver

    db.collection = db.collection(collectionName);

    collection.find({_id: new ObjectId(id)}).toArray(function (err, docs) {
      // Use the docs
    });

    var newDoc = {...};
    collection.insert(newDoc, function(err) {...});

    collection.update({name: 'Jonny'}, {$set: {name: 'Jon'}}, function(err){...});
