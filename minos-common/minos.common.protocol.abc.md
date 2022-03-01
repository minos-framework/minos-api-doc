# minos.common.protocol.abc module


### _class_ minos.common.protocol.abc.MinosBinaryProtocol()
Bases: `abc.ABC`

Minos binary encoder / decoder interface.


#### _abstract classmethod_ decode(data, \*args, \*\*kwargs)
Decodes the given bytes data.


* **Parameters**

    **data** (`bytes`) – bytes data to be decoded.



* **Return type**

    `typing.Any`



* **Returns**

    De decoded data.



#### _abstract classmethod_ encode(\*args, \*\*kwargs)
Encodes the given value into bytes.


* **Parameters**

    
    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `bytes`



* **Returns**

    A bytes instance.
