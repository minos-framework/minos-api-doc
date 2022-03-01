# minos.common.protocol.avro.base module


### _class_ minos.common.protocol.avro.base.MinosAvroProtocol()
Bases: [`minos.common.protocol.abc.MinosBinaryProtocol`](minos.common.protocol.abc.md#minos.common.protocol.abc.MinosBinaryProtocol)

Minos Avro Protocol class.


#### _classmethod_ decode(data, \*args, batch_mode=False, \*\*kwargs)
Decode the given bytes of data into a single dictionary or a sequence of dictionaries.


* **Parameters**

    
    * **data** (`bytes`) – A bytes object.


    * **args** – Additional positional arguments.


    * **batch_mode** (`bool`) – If `True` the data is processed as a list of models, otherwise the data is processed as a


single model.
:param kwargs: Additional named arguments.
:rtype: `typing.Any`
:return: A dictionary or a list of dictionaries.


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



#### _classmethod_ encode(value, schema, \*args, batch_mode=False, \*\*kwargs)
Encoder in avro for database Values
all the headers are converted in fields with double underscore name
the body is a set fields coming from the data type.


* **Parameters**

    
    * **value** (`typing.Any`) – The data to be stored.


    * **schema** (`typing.Any`) – The schema relative to the data.


    * **args** – Additional positional arguments.


    * **batch_mode** (`bool`) – If `True` the data is processed as a list of models, otherwise the data is processed as a


single model.
:param kwargs: Additional named arguments.
:rtype: `bytes`
:return: A bytes object.
