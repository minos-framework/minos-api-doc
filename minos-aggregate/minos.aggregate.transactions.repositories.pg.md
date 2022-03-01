# minos.aggregate.transactions.repositories.pg module


### _class_ minos.aggregate.transactions.repositories.pg.PostgreSqlTransactionRepository(host, port, database, user, password, \*args, \*\*kwargs)
Bases: `minos.common.database.abc.PostgreSqlMinosDatabase`, [`minos.aggregate.transactions.repositories.abc.TransactionRepository`](minos.aggregate.transactions.repositories.abc.md#minos.aggregate.transactions.repositories.abc.TransactionRepository)

PostgreSql Transaction Repository class.


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



#### _classmethod_ from_config(config=None, \*\*kwargs)
Build a new instance from config.


* **Parameters**

    
    * **config** (`typing.Union`[`minos.common.configuration.config.MinosConfig`, `pathlib.Path`, `None`]) – Config instance. If None is provided, default config is chosen.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`S`, bound= `minos.common.setup.MinosSetup`)



* **Returns**

    A instance of the called class.



#### _async_ get(uuid, \*\*kwargs)
Get a `TransactionEntry` from its identifier.


* **Parameters**

    
    * **uuid** (`uuid.UUID`) – Identifier of the `RootEntity`.


    * **kwargs** – Additional named arguments.



* **Return type**

    [`minos.aggregate.transactions.entries.TransactionEntry`](minos.aggregate.transactions.entries.md#minos.aggregate.transactions.entries.TransactionEntry)



* **Returns**

    The `TransactionEntry` instance.



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



#### _async_ select(uuid=None, uuid_ne=None, uuid_in=None, destination_uuid=None, status=None, status_in=None, event_offset=None, event_offset_lt=None, event_offset_gt=None, event_offset_le=None, event_offset_ge=None, updated_at=None, updated_at_lt=None, updated_at_gt=None, updated_at_le=None, updated_at_ge=None, \*\*kwargs)
Get a transaction from the repository.


* **Parameters**

    
    * **uuid** (`typing.Optional`[`uuid.UUID`]) – Transaction identifier equal to the given value.


    * **uuid_ne** (`typing.Optional`[`uuid.UUID`]) – Transaction identifier not equal to the given value


    * **uuid_in** (`typing.Optional`[`tuple`[`uuid.UUID`, `...`]]) – Transaction identifier within the given values.


    * **destination_uuid** (`typing.Optional`[`uuid.UUID`]) – Destination Transaction identifier equal to the given value.


    * **status** (`typing.Optional`[[`minos.aggregate.transactions.entries.TransactionStatus`](minos.aggregate.transactions.entries.md#minos.aggregate.transactions.entries.TransactionStatus)]) – Transaction status equal to the given value.


    * **status_in** (`typing.Optional`[`tuple`[`str`, `...`]]) – Transaction status within the given values


    * **event_offset** (`typing.Optional`[`int`]) – Event offset equal to the given value.


    * **event_offset_lt** (`typing.Optional`[`int`]) – Event Offset lower than the given value


    * **event_offset_gt** (`typing.Optional`[`int`]) – Event Offset greater than the given value


    * **event_offset_le** (`typing.Optional`[`int`]) – Event Offset lower or equal to the given value


    * **event_offset_ge** (`typing.Optional`[`int`]) – Event Offset greater or equal to the given value


    * **updated_at** (`typing.Optional`[`datetime.datetime`]) – Updated at equal to the given value.


    * **updated_at_lt** (`typing.Optional`[`datetime.datetime`]) – Updated at lower than the given value.


    * **updated_at_gt** (`typing.Optional`[`datetime.datetime`]) – Updated at greater than the given value.


    * **updated_at_le** (`typing.Optional`[`datetime.datetime`]) – Updated at lower or equal to the given value.


    * **updated_at_ge** (`typing.Optional`[`datetime.datetime`]) – Updated at greater or equal to the given value.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.AsyncIterator`[[`minos.aggregate.transactions.entries.TransactionEntry`](minos.aggregate.transactions.entries.md#minos.aggregate.transactions.entries.TransactionEntry)]



* **Returns**

    An asynchronous iterator.



#### _async_ setup()
Setup miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ submit(transaction)
Submit a new or updated transaction to store it on the repository.


* **Parameters**

    **transaction** ([`minos.aggregate.transactions.entries.TransactionEntry`](minos.aggregate.transactions.entries.md#minos.aggregate.transactions.entries.TransactionEntry)) – The transaction to be stored.



* **Return type**

    [`minos.aggregate.transactions.entries.TransactionEntry`](minos.aggregate.transactions.entries.md#minos.aggregate.transactions.entries.TransactionEntry)



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



#### write_lock()
Get write lock.


* **Return type**

    `minos.common.locks.Lock`



* **Returns**

    An asynchronous context manager.
