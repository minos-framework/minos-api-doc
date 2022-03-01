# minos.common.database.pools module


### _class_ minos.common.database.pools.PostgreSqlLockPool(host, port, database, user, password, \*args, \*\*kwargs)
Bases: `minos.common.database.pools.PostgreSqlPool`

Postgres Locking Pool class.


#### \__init__(host, port, database, user, password, \*args, \*\*kwargs)

#### acquire(key, \*args, \*\*kwargs)
Acquire a new lock.


* **Parameters**

    **key** (`collections.abc.Hashable`) – The key to be used for locking.



* **Return type**

    [`minos.common.database.locks.PostgreSqlLock`](minos.common.database.locks.md#minos.common.database.locks.PostgreSqlLock)



* **Returns**

    A `PostgreSqlLock` instance.



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



#### _async_ close(timeout=None)

* **Return type**

    `None`



#### _async_ destroy()
Destroy miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _classmethod_ from_config(config=None, \*\*kwargs)
Build a new instance from config.


* **Parameters**

    
    * **config** (`typing.Union`[[`minos.common.configuration.config.MinosConfig`](minos.common.configuration.config.md#minos.common.configuration.config.MinosConfig), `pathlib.Path`, `None`]) – Config instance. If None is provided, default config is chosen.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`S`, bound= [`minos.common.setup.MinosSetup`](minos.common.setup.md#minos.common.setup.MinosSetup))



* **Returns**

    A instance of the called class.



#### _async_ setup()
Setup miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



### _class_ minos.common.database.pools.PostgreSqlPool(host, port, database, user, password, \*args, \*\*kwargs)
Bases: [`minos.common.pools.MinosPool`](minos.common.pools.md#minos.common.pools.MinosPool)[`aiomisc.pool.ContextManager`]

Postgres Pool class.


#### \__init__(host, port, database, user, password, \*args, \*\*kwargs)

#### acquire(\*args, \*\*kwargs)
Acquire a new instance wrapped on an asynchronous context manager.


* **Parameters**

    
    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`P`)



* **Returns**

    An asynchronous context manager.



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



#### _async_ close(timeout=None)

* **Return type**

    `None`



#### _async_ destroy()
Destroy miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _classmethod_ from_config(config=None, \*\*kwargs)
Build a new instance from config.


* **Parameters**

    
    * **config** (`typing.Union`[[`minos.common.configuration.config.MinosConfig`](minos.common.configuration.config.md#minos.common.configuration.config.MinosConfig), `pathlib.Path`, `None`]) – Config instance. If None is provided, default config is chosen.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`S`, bound= [`minos.common.setup.MinosSetup`](minos.common.setup.md#minos.common.setup.MinosSetup))



* **Returns**

    A instance of the called class.



#### _async_ setup()
Setup miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.
