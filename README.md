MongoPagedList
=========

A PagedList extension that works with MongoCursor.

  - MongoCursor<T> Pagination
  - Type Conversion (using AutoMapper)

Version
----

1.0.0.1


Usage with Type Conversion
--------------

```sh
var cursor = Collection.Find(Query.EQ("Field", "Value"));
var pageNumber = 1;
var pageSize = 25;
var model = new MongoPagedList<TSource, TDestination>(cursor, pageNumber, pageSize);
```
Usage without Type Conversion
--------------

```sh
var cursor = Collection.Find(Query.EQ("Field", "Value"));
var pageNumber = 1;
var pageSize = 25;
var model = new MongoPagedList<T>(cursor, pageNumber, pageSize);
```

License
----

MIT


Author
----
Andrea Valla https://github.com/avalla

Thanks
----
PagedList https://github.com/troygoode/PagedList

AutoMapper https://github.com/AutoMapper/AutoMapper

    