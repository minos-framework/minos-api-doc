# minos.common.model.serializers.avro.data.encoder module


### _class_ minos.common.model.serializers.avro.data.encoder.AvroDataEncoder(value=None)
Bases: [`minos.common.model.serializers.abc.DataEncoder`](minos.common.model.serializers.abc.md#minos.common.model.serializers.abc.DataEncoder)

Avro Data Encoder class.


#### \__init__(value=None)

#### build(value=<class 'minos.common.model.types.constants.MissingSentinel'>, \*\*kwargs)
Build an avro data representation based on the content of the given field.


* **Parameters**

    **value** – The value to be encoded.



* **Return type**

    `typing.Any`



* **Returns**

    A avro-compatible data.
