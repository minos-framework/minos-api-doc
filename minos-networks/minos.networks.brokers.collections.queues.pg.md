# minos.networks.brokers.collections.queues.pg module


### _class_ minos.networks.brokers.collections.queues.pg.PostgreSqlBrokerQueue(\*args, query_factory, retry, records, \*\*kwargs)
Bases: [`minos.networks.brokers.collections.queues.abc.BrokerQueue`](minos.networks.brokers.collections.queues.abc.md#minos.networks.brokers.collections.queues.abc.BrokerQueue), `minos.common.database.abc.PostgreSqlMinosDatabase`

PostgreSql Broker Queue class.


#### \__init__(\*args, query_factory, retry, records, \*\*kwargs)

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



#### _async_ dequeue()
Dequeue method.


* **Return type**

    [`minos.networks.brokers.messages.models.abc.BrokerMessage`](minos.networks.brokers.messages.models.abc.md#minos.networks.brokers.messages.models.abc.BrokerMessage)



#### _async_ destroy()
Destroy miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ enqueue(message)
Enqueue method.


* **Return type**

    `None`



#### _classmethod_ from_config(config=None, \*\*kwargs)
Build a new instance from config.


* **Parameters**

    
    * **config** (`typing.Union`[`minos.common.configuration.config.MinosConfig`, `pathlib.Path`, `None`]) – Config instance. If None is provided, default config is chosen.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`S`, bound= `minos.common.setup.MinosSetup`)



* **Returns**

    A instance of the called class.



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



#### _property_ query_factory(_: minos.networks.brokers.collections.queues.pg.PostgreSqlBrokerQueueQueryFactor_ )
Get the query factory.


* **Return type**

    `minos.networks.brokers.collections.queues.pg.PostgreSqlBrokerQueueQueryFactory`



* **Returns**

    A `PostgreSqlBrokerQueueQueryFactory` instance.



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



### _class_ minos.networks.brokers.collections.queues.pg.PostgreSqlBrokerQueueQueryFactory()
Bases: `abc.ABC`

PostgreSql Broker Queue Query Factory class.


#### build_count_not_processed()
Build the “count not processed” query.


* **Return type**

    `psycopg2.sql.SQL`



* **Returns**

    


#### build_create_table()
Build the “create table” query.


* **Return type**

    `psycopg2.sql.SQL`



* **Returns**

    A `SQL` instance.



#### build_delete_processed()
Build the “delete processed” query.


* **Return type**

    `psycopg2.sql.SQL`



* **Returns**

    A `SQL` instance.



#### build_insert()
Build the “insert” query.


* **Return type**

    `psycopg2.sql.SQL`



* **Returns**

    A `SQL` instance.



#### build_listen()
Build the “listen” query.


* **Return type**

    `psycopg2.sql.SQL`



* **Returns**

    A `SQL` instance.



#### build_mark_processing()

* **Return type**

    `psycopg2.sql.SQL`



* **Returns**

    A `SQL` instance.



#### build_notify()
Build the “notify” query.


* **Return type**

    `psycopg2.sql.SQL`



* **Returns**

    A `SQL` instance.



#### build_select_not_processed()
Build the “select not processed” query.


* **Return type**

    `psycopg2.sql.SQL`



* **Returns**

    A `SQL` instance.



#### _abstract_ build_table_name()
Get the table name.


* **Return type**

    `str`



* **Returns**

    A `str` value.



#### build_unlisten()
Build the “unlisten” query.


* **Return type**

    `psycopg2.sql.SQL`



* **Returns**

    A `SQL` instance.



#### build_update_not_processed()
Build the “update not processed” query.


* **Return type**

    `psycopg2.sql.SQL`



* **Returns**

    A `SQL` instance.
