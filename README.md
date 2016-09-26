# disk_db
JSON database interface based on diskDB


Instantiate
-----------
	db = require('diskdb');


Open a collection
-----------------
	db.connect('/path/to/db', ['collection_name']);


Save a collection
-----------------
	db.collection_name.save([article1, article2, article3]);


Access data
-----------
	db.collection_name.item;


Query data
----------
	db.collection_name.find();
	db.collection_name.find({item: "value"});

	db.collection_name.findOne({item: "value"});


Updates
-------
	db.collection_name.update(query, data, options);


Removal
-------
	db.collection_name.remove(query, multi);


Counting
--------
	db.collection_name.count();
