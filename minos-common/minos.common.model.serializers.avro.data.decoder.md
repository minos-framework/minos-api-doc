# minos.common.model.serializers.avro.data.decoder module


### _class_ minos.common.model.serializers.avro.data.decoder.AvroDataDecoder(type_=None)
Bases: [`minos.common.model.serializers.abc.DataDecoder`](minos.common.model.serializers.abc.md#minos.common.model.serializers.abc.DataDecoder)

Avro Data Decoder class.


#### \__init__(type_=None)

#### build(data, type_=<class 'minos.common.model.types.constants.MissingSentinel'>, \*\*kwargs)
Cast data type according to the field definition.


* **Parameters**

    
    * **data** (`typing.Any`) – Data to be casted.


    * **type** – The type of the decoded data.



* **Return type**

    `typing.Any`



* **Returns**

    The casted object.
