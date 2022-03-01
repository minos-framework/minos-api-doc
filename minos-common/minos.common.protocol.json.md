# minos.common.protocol.json module


### _class_ minos.common.protocol.json.MinosJsonBinaryProtocol()
Bases: [`minos.common.protocol.abc.MinosBinaryProtocol`](minos.common.protocol.abc.md#minos.common.protocol.abc.MinosBinaryProtocol)

JSON based binary encoder / decoder implementation.


#### _classmethod_ decode(data, \*args, \*\*kwargs)
Decodes the given bytes data.


* **Parameters**

    **data** (`bytes`) – bytes data to be decoded.



* **Return type**

    `typing.Any`



* **Returns**

    De decoded data.



#### _classmethod_ encode(data, \*args, \*\*kwargs)
Encodes the given value into bytes.


* **Parameters**

    
    * **data** (`typing.Any`) – Data to be encoded.


    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `bytes`



* **Returns**

    A bytes instance.
