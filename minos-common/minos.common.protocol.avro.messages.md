# minos.common.protocol.avro.messages module


### _class_ minos.common.protocol.avro.messages.MinosAvroMessageProtocol()
Bases: [`minos.common.protocol.avro.base.MinosAvroProtocol`](minos.common.protocol.avro.base.md#minos.common.protocol.avro.base.MinosAvroProtocol)

Minos Avro Messages Protocol class.


#### _classmethod_ decode(data, \*args, \*\*kwargs)
Decode the given bytes of data into a single dictionary or a sequence of dictionaries.


* **Parameters**

    
    * **data** (`bytes`) – A bytes object.


    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `dict`



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



#### _classmethod_ encode(headers, body=None, \*args, \*\*kwargs)
encoder in avro
all the headers are converted in fields with double underscore name
the body is a set fields coming from the data type.


* **Return type**

    `bytes`
