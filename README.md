# collection-map-js
A Map with additional utility methods for significantly improved performance and ease-of-use. Inspired by Discord.Js's collection, includes almost all of the function Discord.Js Collection (`.reduce()` is missing).

# Help, Issued & Support
If you have encountered a bug with the library, open a pull request

# Methods
The `Collection` extends `Map`.
`collection` is reffered as `const collection = new Collection();` where `Collection` is reffered as `const Collection = require("collection-map-js").Collection;`.

<!--<table style="width:100%">
  <tr>
    <th>Function Name</th>
    <th>Call</th> 
    <th>Description</th>
    <th>Output</th>
  </tr>
  <tr>
    <td>filter</td>
    <td>collection.filter(fn)</td> 
    <td>Filers all elements based on 'fn' function, 'fn' taked the value as parameter. If 'fn(value)' returns true, the value is added to a new collection which is returned at the end of iteration.</td>
    <td>Collection</td>
  </tr>
  <tr>
    <td>clone</td>
    <td>collection.clone()</td> 
    <td>Returns an exact copy of the 'collection'.</td>
    <td>Collection</td>
  </tr>
  </table> -->
  
  ```js
  // [Parameter] means that that parameter is optional, do not include []'s.
  
  collection.filter(function); // function takes in 'value'
  collection.clone(); // returns an exact same copy of current collection
  collection.first([count]); // returns first x or first value of the collection
  collection.firstKey([count]); // returns first x or first key of the collection
  collection.array(); // array of collection values
  collection.last([count]); // returns last x or first value of the collection
  collection.lastKey([count]); // returns last x or first key of the collection
  collection.deleteAll(); // calls delete method on all items of the collection
  collection.every(function); // returns boolean, true if every item of the collection makes function returns true, function takes in 'value'
  collecton.equals(collection2); // return boolean, true if collection2 and collection have a 100% key-vaue pairs matching
  collection.keyArray(); // array of collection keys
  collection.map(); // equal to Array.map();
  collection.partition(function); // returns array of 2 collections, first collection item that passed function and second collection items that failed function ([collection1, collection2] or [passed, failed]), function takes in value
  collection.random([count]); // returns array of 'count' random values from the collection, there can (and will be) duplicates (regardless of array length but more likely count represents a big portion of collection's size)
  collection.randomKeys([count]); // returns array of 'count' random keys from the collection, there can (and will be) duplicates (regardless of array length but more likely count represents a big portion of collection's size)
  collection.some(function); // returns true if at least 1 element of collection passed function, function takes in value
  collection.find(function); // filters the collection and returns the first item value passing function, function takes in value
  ```
