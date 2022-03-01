# minos.aggregate.snapshots.pg.readers module


### _class_ minos.aggregate.snapshots.pg.readers.PostgreSqlSnapshotReader(host, port, database, user, password, \*args, \*\*kwargs)
Bases: [`minos.aggregate.snapshots.pg.abc.PostgreSqlSnapshotSetup`](minos.aggregate.snapshots.pg.abc.md#minos.aggregate.snapshots.pg.abc.PostgreSqlSnapshotSetup)

PostgreSQL Snapshot class.

The snapshot provides a direct accessor to the `RootEntity` instances stored as events by the event repository
class.


#### \__init__(host, port, database, user, password, \*args, \*\*kwargs)

#### _property_ already_destroyed(_: boo_ )
Already Destroy getter.


* **Return type**

    `bool`



* **Returns**

    A boolean value.



#### _property_ already_setup(_: boo_ )
Already Setup getter.


* **Return type**

    `bool`



* **Returns**

    A boolean value.



#### cursor(\*args, \*\*kwargs)
Get a new cursor.


* **Parameters**

    
    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.AsyncContextManager`[`aiopg.connection.Cursor`]



* **Returns**

    A Cursor wrapped into an asynchronous context manager.



#### _async_ destroy()
Destroy miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ find(\*args, \*\*kwargs)
Find a collection of `RootEntity` instances based on a `Condition`.


* **Parameters**

    
    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.AsyncIterator`[[`minos.aggregate.entities.models.RootEntity`](minos.aggregate.entities.models.md#minos.aggregate.entities.models.RootEntity)]



* **Returns**

    An asynchronous iterator that containing the `RootEntity` instances.



#### _async_ find_entries(name, condition, ordering=None, limit=None, streaming_mode=False, transaction=None, exclude_deleted=True, \*\*kwargs)
Find a collection of `SnapshotEntry` instances based on a `Condition`.


* **Parameters**

    
    * **name** (`str`) – Class name of the `RootEntity`.


    * **condition** (`minos.aggregate.queries._Condition`) – The condition that must be satisfied by the `RootEntity` instances.


    * **ordering** (`typing.Optional`[`minos.aggregate.queries._Ordering`]) – Optional argument to return the instance with specific ordering strategy. The default behaviour
    is to retrieve them without any order pattern.


    * **limit** (`typing.Optional`[`int`]) – Optional argument to return only a subset of instances. The default behaviour is to return all the
    instances that meet the given condition.


    * **streaming_mode** (`bool`) – If `True` return the values in streaming directly from the database (keep an open
    database connection), otherwise preloads the full set of values on memory and then retrieves them.


    * **transaction** (`typing.Optional`[[`minos.aggregate.transactions.entries.TransactionEntry`](minos.aggregate.transactions.entries.md#minos.aggregate.transactions.entries.TransactionEntry)]) – The transaction within the operation is performed. If not any value is provided, then the
    transaction is extracted from the context var. If not any transaction is being scoped then the query is
    performed to the global snapshot.


    * **exclude_deleted** (`bool`) – If `True`, deleted `RootEntity` entries are included, otherwise deleted


`RootEntity` entries are filtered.
:param kwargs: Additional named arguments.
:rtype: `typing.AsyncIterator`[[`minos.aggregate.snapshots.entries.SnapshotEntry`](minos.aggregate.snapshots.entries.md#minos.aggregate.snapshots.entries.SnapshotEntry)]
:return: An asynchronous iterator that containing the `RootEntity` instances.


#### _classmethod_ from_config(config=None, \*\*kwargs)
Build a new instance from config.


* **Parameters**

    
    * **config** (`typing.Union`[`minos.common.configuration.config.MinosConfig`, `pathlib.Path`, `None`]) – Config instance. If None is provided, default config is chosen.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`S`, bound= `minos.common.setup.MinosSetup`)



* **Returns**

    A instance of the called class.



#### _async_ get(name, uuid, \*\*kwargs)
Get a `RootEntity` instance from its identifier.


* **Parameters**

    
    * **name** (`str`) – Class name of the `RootEntity`.


    * **uuid** (`uuid.UUID`) – Identifier of the `RootEntity`.


    * **kwargs** – Additional named arguments.



* **Return type**

    [`minos.aggregate.entities.models.RootEntity`](minos.aggregate.entities.models.md#minos.aggregate.entities.models.RootEntity)



* **Returns**

    The `RootEntity` instance.



#### _async_ get_entry(name, uuid, \*\*kwargs)
Get a `SnapshotEntry` from its identifier.


* **Parameters**

    
    * **name** (`str`) – Class name of the `RootEntity`.


    * **uuid** (`uuid.UUID`) – Identifier of the `RootEntity`.


    * **kwargs** – Additional named arguments.



* **Return type**

    [`minos.aggregate.snapshots.entries.SnapshotEntry`](minos.aggregate.snapshots.entries.md#minos.aggregate.snapshots.entries.SnapshotEntry)



* **Returns**

    The `SnapshotEntry` instance.



#### locked_cursor(key, \*args, \*\*kwargs)
Get a new locked cursor.


* **Parameters**

    
    * **key** (`collections.abc.Hashable`) – The key to be used for locking.


    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.AsyncContextManager`[`aiopg.connection.Cursor`]



* **Returns**

    A Cursor wrapped into an asynchronous context manager.



#### _property_ pool(_: minos.common.database.pools.PostgreSqlPoo_ )
Get the connections pool.


* **Return type**

    `minos.common.database.pools.PostgreSqlPool`



* **Returns**

    A `Pool` object.



#### _async_ setup()
Setup miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ submit_query(operation, parameters=None, \*, timeout=None, lock=None, \*\*kwargs)
Submit a SQL query.


* **Parameters**

    
    * **operation** (`typing.Any`) – Query to be executed.


    * **parameters** (`typing.Optional`[`typing.Any`]) – Parameters to be projected into the query.


    * **timeout** (`typing.Optional`[`float`]) – An optional timeout.


    * **lock** (`typing.Optional`[`typing.Any`]) – Optional key to perform the query with locking. If not set, the query is performed without any
    lock.


    * **kwargs** – Additional named arguments.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ submit_query_and_fetchone(\*args, \*\*kwargs)
Submit a SQL query and gets the first response.


* **Parameters**

    
    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `tuple`



* **Returns**

    This method does not return anything.



#### _async_ submit_query_and_iter(operation, parameters=None, \*, timeout=None, lock=None, streaming_mode=False, \*\*kwargs)
Submit a SQL query and return an asynchronous iterator.


* **Parameters**

    
    * **operation** (`typing.Any`) – Query to be executed.


    * **parameters** (`typing.Optional`[`typing.Any`]) – Parameters to be projected into the query.


    * **timeout** (`typing.Optional`[`float`]) – An optional timeout.


    * **lock** (`typing.Optional`[`int`]) – Optional key to perform the query with locking. If not set, the query is performed without any
    lock.


    * **streaming_mode** (`bool`) – If `True` the data fetching is performed in streaming mode, that is iterating over the
    cursor and yielding once a time (requires an opening connection to do that). Otherwise, all the data is
    fetched and keep in memory before yielding it.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.AsyncIterator`[`tuple`]



* **Returns**

    This method does not return anything.
