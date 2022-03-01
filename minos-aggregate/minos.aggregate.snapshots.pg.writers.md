# minos.aggregate.snapshots.pg.writers module


### _class_ minos.aggregate.snapshots.pg.writers.PostgreSqlSnapshotWriter(\*args, reader, event_repository=<dependency_injector.wiring.Provide object>, transaction_repository=<dependency_injector.wiring.Provide object>, \*\*kwargs)
Bases: [`minos.aggregate.snapshots.pg.abc.PostgreSqlSnapshotSetup`](minos.aggregate.snapshots.pg.abc.md#minos.aggregate.snapshots.pg.abc.PostgreSqlSnapshotSetup)

Minos Snapshot Dispatcher class.


#### \__init__(\*args, reader, event_repository=<dependency_injector.wiring.Provide object>, transaction_repository=<dependency_injector.wiring.Provide object>, \*\*kwargs)

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



#### _async_ dispatch(\*\*kwargs)
Perform a dispatching step, based on the sequence of non already processed `EventEntry` objects.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _classmethod_ from_config(config=None, \*\*kwargs)
Build a new instance from config.


* **Parameters**

    
    * **config** (`typing.Union`[`minos.common.configuration.config.MinosConfig`, `pathlib.Path`, `None`]) – Config instance. If None is provided, default config is chosen.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`S`, bound= `minos.common.setup.MinosSetup`)



* **Returns**

    A instance of the called class.



#### _async_ is_synced(name, \*\*kwargs)
Check if the snapshot has the latest version of a `RootEntity` instance.


* **Parameters**

    **name** (`str`) – Class name of the `RootEntity` to be checked.



* **Return type**

    `bool`



* **Returns**

    `True` if it has the latest version for the identifier or `False` otherwise.



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
