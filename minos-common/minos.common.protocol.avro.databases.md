# minos.common.protocol.avro.databases module


### _class_ minos.common.protocol.avro.databases.MinosAvroDatabaseProtocol()
Bases: [`minos.common.protocol.avro.base.MinosAvroProtocol`](minos.common.protocol.avro.base.md#minos.common.protocol.avro.base.MinosAvroProtocol)

Encoder/Decoder class for values to be stored on the database with avro format.


#### _classmethod_ decode(data, \*args, \*\*kwargs)
Decode the given bytes of data into a single dictionary or a sequence of dictionaries.


* **Parameters**

    
    * **data** (`bytes`) – A bytes object.


    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.Union`[`dict`[`str`, `typing.Any`], `list`[`dict`[`str`, `typing.Any`]]]



* **Returns**

    A dictionary or a list of dictionaries.



#### _classmethod_ decode_schema(data, \*args, \*\*kwargs)
Decode the given bytes of data into a single dictionary or a sequence of dictionaries.


* **Parameters**

    
    * **data** (`bytes`) – A bytes object.


    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.Union`[`dict`[`str`, `typing.Any`], `list`[`dict`[`str`, `typing.Any`]]]



* **Returns**

    A tuple or a list of tuples.



#### _classmethod_ encode(value, \*args, \*\*kwargs)
Encoder in avro for database Values
all the headers are converted in fields with double underscore name
the body is a set fields coming from the data type.


* **Parameters**

    
    * **value** (`typing.Any`) – The data to be stored.


    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `bytes`



* **Returns**

    A bytes object.
