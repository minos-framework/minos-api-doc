# minos.common.storage.lmdb module


### _class_ minos.common.storage.lmdb.MinosStorageLmdb(env, protocol=<class 'minos.common.protocol.avro.databases.MinosAvroDatabaseProtocol'>, \*\*kwargs)
Bases: [`minos.common.storage.abc.MinosStorage`](minos.common.storage.abc.md#minos.common.storage.abc.MinosStorage)

Minos Storage LMDB class


#### \__init__(env, protocol=<class 'minos.common.protocol.avro.databases.MinosAvroDatabaseProtocol'>, \*\*kwargs)

#### add(table, key, value)
Store a value.


* **Parameters**

    
    * **table** (`str`) – Table in which the data is stored.


    * **key** (`str`) – Key that identifies the data.


    * **value** (`typing.Any`) – Data to be stored.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _classmethod_ build(path, max_db=10, map_size=1000000000, \*\*kwargs)
Build a new instance.


* **Parameters**

    
    * **path** (`typing.Union`[`str`, `pathlib.Path`]) – Path in which the database is stored.


    * **max_db** (`int`) – Maximum number of available databases.


    * **map_size** (`int`) – Maximum number of entries to be stored on the database. Default set to 1GB


    * **kwargs** – Additional named arguments.



* **Return type**

    `minos.common.storage.lmdb.MinosStorageLmdb`



* **Returns**

    A `MinosStorageLmdb` instance.



#### delete(table, key)
Delete the stored value.


* **Parameters**

    
    * **table** (`str`) – Table in which the data is stored.


    * **key** (`str`) – Key that identifies the data.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### get(table, key)
Get the stored value..


* **Parameters**

    
    * **table** (`str`) – Table in which the data is stored.


    * **key** (`str`) – Key that identifies the data.



* **Return type**

    `typing.Optional`[`typing.Any`]



* **Returns**

    The stored value or `None` if it’s empty.



#### update(table, key, value)
Update the stored value.


* **Parameters**

    
    * **table** (`str`) – Table in which the data is stored.


    * **key** (`str`) – Key that identifies the data.


    * **value** (`typing.Any`) – Data to be stored.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.
