# minos.common.model.serializers.avro.schema.decoder module


### _class_ minos.common.model.serializers.avro.schema.decoder.AvroSchemaDecoder(schema=None)
Bases: [`minos.common.model.serializers.abc.SchemaDecoder`](minos.common.model.serializers.abc.md#minos.common.model.serializers.abc.SchemaDecoder)

Avro Schema Decoder class.


#### \__init__(schema=None)

#### build(schema=<class 'minos.common.model.types.constants.MissingSentinel'>, \*\*kwargs)
Build type from given avro schema item.


* **Parameters**

    **schema** (`typing.Any`) – The schema to be decoded as a type.



* **Return type**

    `type`



* **Returns**

    A type object.
