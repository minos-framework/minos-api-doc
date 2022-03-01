# minos.common.model.dynamic.dto module


### _class_ minos.common.model.dynamic.dto.DataTransferObject(name, \*args, namespace='', \*\*kwargs)
Bases: [`minos.common.model.dynamic.abc.DynamicModel`](minos.common.model.dynamic.abc.md#minos.common.model.dynamic.abc.DynamicModel)

Data Transfer Object to build the objects dynamically from bytes


#### \__init__(name, \*args, namespace='', \*\*kwargs)
Class constructor.


* **Parameters**

    **fields** – Dictionary that contains the `Field` instances of the model indexed by name.



#### _property_ avro_bytes(_: byte_ )
Generate bytes representation of the current instance.


* **Return type**

    `bytes`



* **Returns**

    A bytes object.



#### _property_ avro_data(_: dict[str, Any_ )
Compute the avro data of the model.


* **Return type**

    `dict`[`str`, `typing.Any`]



* **Returns**

    A dictionary object.



#### _property_ avro_str(_: st_ )
Generate bytes representation of the current instance.


* **Return type**

    `str`



* **Returns**

    A bytes object.



#### _property_ classname(_: st_ )
Compute the current class name.


* **Return type**

    `str`



* **Returns**

    An string object.



#### _static_ decode_data(decoder, target, type_, \*\*kwargs)
Decode data with the given decoder.


* **Parameters**

    
    * **decoder** ([`minos.common.model.serializers.abc.DataDecoder`](minos.common.model.serializers.abc.md#minos.common.model.serializers.abc.DataDecoder)) – The decoder instance.


    * **target** (`typing.Any`) – The data to be decoded.


    * **type** – The data type.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.Any`



* **Returns**

    A decoded instance.



#### _static_ decode_schema(decoder, target, \*\*kwargs)
Decode schema with the given encoder.


* **Parameters**

    
    * **decoder** ([`minos.common.model.serializers.abc.SchemaDecoder`](minos.common.model.serializers.abc.md#minos.common.model.serializers.abc.SchemaDecoder)) – The decoder instance.


    * **target** (`typing.Any`) – The schema to be decoded.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.Any`



* **Returns**

    The decoded schema as a type.



#### _static_ encode_data(encoder, target, \*\*kwargs)
Encode data with the given encoder.


* **Parameters**

    
    * **encoder** ([`minos.common.model.serializers.abc.DataEncoder`](minos.common.model.serializers.abc.md#minos.common.model.serializers.abc.DataEncoder)) – The encoder instance.


    * **target** (`typing.Any`) – An optional pre-encoded data.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.Any`



* **Returns**

    The encoded data of the instance.



#### _static_ encode_schema(encoder, target, \*\*kwargs)
Encode schema with the given encoder.


* **Parameters**

    
    * **encoder** ([`minos.common.model.serializers.abc.SchemaEncoder`](minos.common.model.serializers.abc.md#minos.common.model.serializers.abc.SchemaEncoder)) – The encoder instance.


    * **target** (`typing.Any`) – An optional pre-encoded schema.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.Any`



* **Returns**

    The encoded schema of the instance.



#### _property_ fields(_: dict[str, [minos.common.model.fields.Field](minos.common.model.fields.md#minos.common.model.fields.Field)_ )
Fields getter


* **Return type**

    `dict`[`str`, [`minos.common.model.fields.Field`](minos.common.model.fields.md#minos.common.model.fields.Field)]



#### _classmethod_ from_avro(schema, data)
Build a new instance from the `avro` schema and data.


* **Parameters**

    
    * **schema** (`typing.Any`) – The avro schema of the model.


    * **data** (`typing.Any`) – The avro data of the model.



* **Return type**

    `typing.TypeVar`(`T`, bound= [`minos.common.model.abc.Model`](minos.common.model.abc.md#minos.common.model.abc.Model))



* **Returns**

    A new `DynamicModel` instance.



#### _classmethod_ from_avro_bytes(raw, batch_mode=False, \*\*kwargs)
Build a single instance or a sequence of instances from bytes


* **Parameters**

    
    * **raw** (`bytes`) – A `bytes` representation of the model.


    * **batch_mode** (`bool`) – If `True` the data is processed as a list of models, otherwise the data is processed as a


single model.
:param kwargs: Additional named arguments.
:rtype: `typing.Union`[`typing.TypeVar`(`T`, bound= [`minos.common.model.abc.Model`](minos.common.model.abc.md#minos.common.model.abc.Model)), `list`[`typing.TypeVar`(`T`, bound= [`minos.common.model.abc.Model`](minos.common.model.abc.md#minos.common.model.abc.Model))]]
:return: A single instance or a sequence of instances.


#### _classmethod_ from_avro_str(raw, \*\*kwargs)
Build a single instance or a sequence of instances from bytes


* **Parameters**

    **raw** (`str`) – A `str` representation of the model.



* **Return type**

    `typing.Union`[`typing.TypeVar`(`T`, bound= [`minos.common.model.abc.Model`](minos.common.model.abc.md#minos.common.model.abc.Model)), `list`[`typing.TypeVar`(`T`, bound= [`minos.common.model.abc.Model`](minos.common.model.abc.md#minos.common.model.abc.Model))]]



* **Returns**

    A single instance or a sequence of instances.



#### _classmethod_ from_model_type(model_type, \*args, \*\*kwargs)
Build a `DataTransferObject` from a `ModelType`.


* **Parameters**

    
    * **model_type** ([`minos.common.model.types.model_types.ModelType`](minos.common.model.types.model_types.md#minos.common.model.types.model_types.ModelType)) – `ModelType` object containing the model structure


    * **args** – Positional arguments to be passed to the model constructor.


    * **kwargs** – Named arguments to be passed to the model constructor.



* **Return type**

    `minos.common.model.dynamic.dto.DataTransferObject`



* **Returns**

    A new `DataTransferObject` instance.



#### _classmethod_ from_typed_dict(typed_dict, \*args, \*\*kwargs)
Build a `Model` from a `TypeDict` and `data`.


* **Parameters**

    
    * **typed_dict** (`typing.TypedDict`) – `TypeDict` object containing the DTO’s structure


    * **args** – Positional arguments to be passed to the model constructor.


    * **kwargs** – Named arguments to be passed to the model constructor.



* **Return type**

    `typing.TypeVar`(`T`, bound= [`minos.common.model.abc.Model`](minos.common.model.abc.md#minos.common.model.abc.Model))



* **Returns**

    A new `DataTransferObject` instance.



#### get(k, )

#### items()

#### keys()

#### _classmethod_ to_avro_bytes(models)
Create a `bytes` representation of the given object instances.


* **Parameters**

    **models** (`list`[`typing.TypeVar`(`T`, bound= [`minos.common.model.abc.Model`](minos.common.model.abc.md#minos.common.model.abc.Model))]) – A sequence of minos models.



* **Return type**

    `bytes`



* **Returns**

    A bytes object.



#### _classmethod_ to_avro_str(models)
Build the avro string representation of the given object instances.


* **Parameters**

    **models** (`list`[`typing.TypeVar`(`T`, bound= [`minos.common.model.abc.Model`](minos.common.model.abc.md#minos.common.model.abc.Model))]) – A sequence of minos models.



* **Return type**

    `str`



* **Returns**

    A bytes object.



#### type_hints(_ = {_ )

#### type_hints_parameters(_ = (_ )

#### values()
