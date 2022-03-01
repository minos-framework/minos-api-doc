# minos.common.model.serializers.avro.schema.encoder module


### _class_ minos.common.model.serializers.avro.schema.encoder.AvroSchemaEncoder(type_=None)
Bases: [`minos.common.model.serializers.abc.SchemaEncoder`](minos.common.model.serializers.abc.md#minos.common.model.serializers.abc.SchemaEncoder)

Avro Schema Encoder class.


#### \__init__(type_=None)

#### build(type_=<class 'minos.common.model.types.constants.MissingSentinel'>, \*\*kwargs)
Build the avro schema for the given field.


* **Parameters**

    **type** – The type to be encoded as a schema.



* **Return type**

    `typing.Union`[`dict`, `list`, `str`]



* **Returns**

    A dictionary object.



#### _static_ generate_random_str()
Generate a random string


* **Return type**

    `str`



* **Returns**

    A random string value.
