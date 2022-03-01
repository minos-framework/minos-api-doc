# minos.common.model.serializers.abc module


### _class_ minos.common.model.serializers.abc.DataDecoder()
Bases: `abc.ABC`

Data Decoder base class.


#### _abstract_ build(data, type_, \*\*kwargs)
Cast data type according to the field definition.


* **Parameters**

    
    * **data** (`typing.Any`) – Data to be casted.


    * **type** – The type of the decoded data.



* **Return type**

    `typing.Any`



* **Returns**

    The casted object.



### _class_ minos.common.model.serializers.abc.DataEncoder()
Bases: `abc.ABC`

Data Encoder base class.


#### _abstract_ build(value, \*\*kwargs)
Build an avro data representation based on the content of the given field.


* **Parameters**

    **value** (`typing.Any`) – The value to be encoded.



* **Return type**

    `typing.Any`



* **Returns**

    A avro-compatible data.



### _class_ minos.common.model.serializers.abc.SchemaDecoder()
Bases: `abc.ABC`

Schema Decoder base class.


#### _abstract_ build(schema, \*\*kwargs)
Build type from given avro schema item.


* **Parameters**

    **schema** (`typing.Any`) – The schema to be decoded as a type.



* **Return type**

    `type`



* **Returns**

    A type object.



### _class_ minos.common.model.serializers.abc.SchemaEncoder()
Bases: `abc.ABC`

Schema Encoder base class.


#### _abstract_ build(type_, \*\*kwargs)
Build the avro schema for the given field.


* **Parameters**

    **type** – The type to be encoded as a schema.



* **Return type**

    `typing.Any`



* **Returns**

    A dictionary object.
