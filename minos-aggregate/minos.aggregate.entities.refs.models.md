# minos.aggregate.entities.refs.models module


### _class_ minos.aggregate.entities.refs.models.Ref(data, \*args, broker_pool=<dependency_injector.wiring.Provide object>, \*\*kwargs)
Bases: `minos.common.model.declarative.DeclarativeModel`, `uuid.UUID`, `Generic`[`minos.aggregate.entities.refs.models.MT`]

Model Reference.


#### \__init__(data, \*args, broker_pool=<dependency_injector.wiring.Provide object>, \*\*kwargs)
Class constructor.


* **Parameters**

    **kwargs** – Named arguments to be set as model attributes.



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



#### avro_schema(_ = {'logicalType': 'uuid', 'type': 'string'_ )

#### _property_ avro_str(_: st_ )
Generate bytes representation of the current instance.


* **Return type**

    `str`



* **Returns**

    A bytes object.



#### _property_ bytes()

#### _property_ bytes_le()

#### classname(_ = 'minos.aggregate.entities.refs.models.Ref_ )

#### _property_ clock_seq()

#### _property_ clock_seq_hi_variant()

#### _property_ clock_seq_low()

#### data(_: Union[MT, UUID_ )

#### _property_ data_cls(_: Optional[type_ )
Get data class if available.


* **Return type**

    `typing.Optional`[`type`]



* **Returns**

    A model type.



#### _classmethod_ decode_data(decoder, target, type_, \*\*kwargs)
Decode data with the given decoder.


* **Parameters**

    
    * **decoder** (`minos.common.model.serializers.abc.DataDecoder`) – The decoder instance.


    * **target** (`typing.Any`) – The data to be decoded.


    * **type** – The data type.



* **Return type**

    `minos.aggregate.entities.refs.models.Ref`



* **Returns**

    A decoded instance.



#### _classmethod_ decode_schema(decoder, target, \*\*kwargs)
Decode schema with the given encoder.


* **Parameters**

    
    * **decoder** (`minos.common.model.serializers.abc.SchemaDecoder`) – The decoder instance.


    * **target** (`typing.Any`) – The schema to be decoded.



* **Return type**

    `minos.common.model.types.model_types.ModelType`



* **Returns**

    The decoded schema as a type.



#### _static_ encode_data(encoder, target, \*\*kwargs)
Encode data with the given encoder.


* **Parameters**

    
    * **encoder** (`minos.common.model.serializers.abc.DataEncoder`) – The encoder instance.


    * **target** (`typing.Any`) – An optional pre-encoded data.



* **Return type**

    `typing.Any`



* **Returns**

    The encoded data of the instance.



#### _classmethod_ encode_schema(encoder, target, \*\*kwargs)
Encode schema with the given encoder.


* **Parameters**

    
    * **encoder** (`minos.common.model.serializers.abc.SchemaEncoder`) – The encoder instance.


    * **target** (`typing.Any`) – An optional pre-encoded schema.



* **Return type**

    `typing.Any`



* **Returns**

    The encoded schema of the instance.



#### _property_ fields(_: dict[str, minos.common.model.fields.Field_ )
Fields getter


* **Return type**

    `dict`[`str`, `minos.common.model.fields.Field`]



#### _classmethod_ from_avro(schema, data)
Build a new instance from the `avro` schema and data.


* **Parameters**

    
    * **schema** (`typing.Any`) – The avro schema of the model.


    * **data** (`typing.Any`) – The avro data of the model.



* **Return type**

    `typing.TypeVar`(`T`, bound= `minos.common.model.abc.Model`)



* **Returns**

    A new `DynamicModel` instance.



#### _classmethod_ from_avro_bytes(raw, batch_mode=False, \*\*kwargs)
Build a single instance or a sequence of instances from bytes


* **Parameters**

    
    * **raw** (`bytes`) – A `bytes` representation of the model.


    * **batch_mode** (`bool`) – If `True` the data is processed as a list of models, otherwise the data is processed as a


single model.
:param kwargs: Additional named arguments.
:rtype: `typing.Union`[`typing.TypeVar`(`T`, bound= `minos.common.model.abc.Model`), `list`[`typing.TypeVar`(`T`, bound= `minos.common.model.abc.Model`)]]
:return: A single instance or a sequence of instances.


#### _classmethod_ from_avro_str(raw, \*\*kwargs)
Build a single instance or a sequence of instances from bytes


* **Parameters**

    **raw** (`str`) – A `str` representation of the model.



* **Return type**

    `typing.Union`[`typing.TypeVar`(`T`, bound= `minos.common.model.abc.Model`), `list`[`typing.TypeVar`(`T`, bound= `minos.common.model.abc.Model`)]]



* **Returns**

    A single instance or a sequence of instances.



#### _classmethod_ from_model_type(model_type, \*args, \*\*kwargs)
Build a `DeclarativeModel` from a `ModelType`.


* **Parameters**

    
    * **model_type** (`minos.common.model.types.model_types.ModelType`) – `ModelType` object containing the model structure.


    * **args** – Positional arguments to be passed to the model constructor.


    * **kwargs** – Named arguments to be passed to the model constructor.



* **Return type**

    `typing.TypeVar`(`T`, bound= `minos.common.model.declarative.DeclarativeModel`)



* **Returns**

    A new `DeclarativeModel` instance.



#### _classmethod_ from_typed_dict(typed_dict, \*args, \*\*kwargs)
Build a `Model` from a `TypeDict` and `data`.


* **Parameters**

    
    * **typed_dict** (`typing.TypedDict`) – `TypeDict` object containing the DTO’s structure


    * **args** – Positional arguments to be passed to the model constructor.


    * **kwargs** – Named arguments to be passed to the model constructor.



* **Return type**

    `typing.TypeVar`(`T`, bound= `minos.common.model.abc.Model`)



* **Returns**

    A new `DataTransferObject` instance.



#### get(k, )

#### _property_ hex()

#### _property_ int(_: in_ )
Get the UUID as a 128-bit integer.


* **Return type**

    `int`



* **Returns**

    An integer value.



#### _property_ is_safe(_: uuid.SafeUUI_ )
Get an enum indicating whether the UUID has been generated in a way that is safe.


* **Return type**

    `uuid.SafeUUID`



* **Returns**

    A `SafeUUID` value.



#### items()

#### keys()

#### _property_ node()

#### _async_ resolve(force=False, \*\*kwargs)
Resolve the instance.


* **Parameters**

    
    * **force** (`bool`) – If `True`, the resolution will be performed also if it is not necessary.


    * **kwargs** – Additional named arguments.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _property_ resolved(_: boo_ )
Check if the instance is already resolved.


* **Return type**

    `bool`



* **Returns**

    `True` if resolved or `False` otherwise.



#### _property_ time()

#### _property_ time_hi_version()

#### _property_ time_low()

#### _property_ time_mid()

#### _classmethod_ to_avro_bytes(models)
Create a `bytes` representation of the given object instances.


* **Parameters**

    **models** (`list`[`typing.TypeVar`(`T`, bound= `minos.common.model.abc.Model`)]) – A sequence of minos models.



* **Return type**

    `bytes`



* **Returns**

    A bytes object.



#### _classmethod_ to_avro_str(models)
Build the avro string representation of the given object instances.


* **Parameters**

    **models** (`list`[`typing.TypeVar`(`T`, bound= `minos.common.model.abc.Model`)]) – A sequence of minos models.



* **Return type**

    `str`



* **Returns**

    A bytes object.



#### type_hints()

#### type_hints_parameters(_ = (~MT,_ )

#### _property_ urn()

#### _property_ uuid(_: uuid.UUI_ )
Get the UUID that identifies the `Model`.


* **Return type**

    `uuid.UUID`



* **Returns**

    


#### values()

#### _property_ variant()

#### _property_ version()
