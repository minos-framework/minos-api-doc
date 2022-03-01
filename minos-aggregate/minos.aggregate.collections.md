# minos.aggregate.collections module


### _class_ minos.aggregate.collections.IncrementalSet(data=None, \*args, \*\*kwargs)
Bases: `minos.common.model.declarative.DeclarativeModel`, `collections.abc.MutableSet`, `Generic`[`minos.aggregate.collections.T`]

Incremental Set class.


#### \__init__(data=None, \*args, \*\*kwargs)
Class constructor.


* **Parameters**

    **kwargs** – Named arguments to be set as model attributes.



#### add(value_object)
Add a value object.
:type value_object: `typing.TypeVar`(`T`)
:param value_object: The value object to be added.
:rtype: `None`
:return: This method does not return anything.


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



#### avro_schema(_ = [{'type': 'array', 'items': 'null', 'logicalType': 'minos.aggregate.collections.IncrementalSet'}_ )

#### _property_ avro_str(_: st_ )
Generate bytes representation of the current instance.


* **Return type**

    `str`



* **Returns**

    A bytes object.



#### classname(_ = 'minos.aggregate.collections.IncrementalSet_ )

#### clear()
This is slow (creates N new iterators!) but effective.


#### data(_: set[T_ )

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

    `minos.aggregate.collections.IncrementalSet`



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



#### diff(another)
Compute the difference between self and another entity set.
:type another: `minos.aggregate.collections.IncrementalSet`[`typing.TypeVar`(`T`)]
:param another: Another entity set instance.
:rtype: `minos.aggregate.collections.IncrementalSetDiff`
:return: The difference between both entity sets.


#### discard(value_object)
Remove a value object.
:type value_object: `typing.TypeVar`(`T`)
:param value_object: The value object to be added.
:rtype: `None`
:return: This method does not return anything.


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

#### isdisjoint(other)
Return True if two sets have a null intersection.


#### items()

#### keys()

#### pop()
Return the popped value.  Raise KeyError if empty.


#### remove(value)
Remove an element. If not a member, raise a KeyError.


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

#### type_hints_parameters(_ = (~T,_ )

#### values()

### _class_ minos.aggregate.collections.IncrementalSetDiff(\*args, \*\*kwargs)
Bases: `minos.common.model.declarative.DeclarativeModel`

Incremental Set Diff class.


#### \__init__(\*args, \*\*kwargs)
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



#### avro_schema(_ = [{'name': 'IncrementalSetDiff', 'namespace': 'minos.aggregate.collections.e3eb8f89-8e31-43ec-b524-78067d2cf7b5', 'type': 'record', 'fields': [{'name': 'diffs', 'type': {'type': 'array', 'items': {'name': 'SetDiffEntry', 'namespace': '', 'type': 'record', 'fields': [{'name': 'action', 'type': {'type': 'string', 'logicalType': 'minos.aggregate.actions.Action'}}, {'name': 'entity', 'type': 'null'}]}}}]}_ )

#### _property_ avro_str(_: st_ )
Generate bytes representation of the current instance.


* **Return type**

    `str`



* **Returns**

    A bytes object.



#### classname(_ = 'minos.aggregate.collections.IncrementalSetDiff_ )

#### _static_ decode_data(decoder, target, type_, \*\*kwargs)
Decode data with the given decoder.


* **Parameters**

    
    * **decoder** (`minos.common.model.serializers.abc.DataDecoder`) – The decoder instance.


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

    
    * **decoder** (`minos.common.model.serializers.abc.SchemaDecoder`) – The decoder instance.


    * **target** (`typing.Any`) – The schema to be decoded.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.Any`



* **Returns**

    The decoded schema as a type.



#### diffs(_: list[IncrementalSetDiffEntry_ )

#### _static_ encode_data(encoder, target, \*\*kwargs)
Encode data with the given encoder.


* **Parameters**

    
    * **encoder** (`minos.common.model.serializers.abc.DataEncoder`) – The encoder instance.


    * **target** (`typing.Any`) – An optional pre-encoded data.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.Any`



* **Returns**

    The encoded data of the instance.



#### _static_ encode_schema(encoder, target, \*\*kwargs)
Encode schema with the given encoder.


* **Parameters**

    
    * **encoder** (`minos.common.model.serializers.abc.SchemaEncoder`) – The encoder instance.


    * **target** (`typing.Any`) – An optional pre-encoded schema.


    * **kwargs** – Additional named arguments.



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



#### _classmethod_ from_difference(new, old, get_fn=None)
Build a new instance from two entity sets.
:type new: `minos.aggregate.collections.IncrementalSet`[`typing.TypeVar`(`T`)]
:param new: The new entity set.
:type old: `minos.aggregate.collections.IncrementalSet`[`typing.TypeVar`(`T`)]
:param old: The old entity set.
:type get_fn: `typing.Optional`[`typing.Callable`[[`typing.TypeVar`(`T`)], `typing.Any`]]
:param get_fn: Optional function to get entries from the set by identifier.
:rtype: `minos.aggregate.collections.IncrementalSetDiff`
:return: The difference between new and old.


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

#### items()

#### keys()

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

#### type_hints_parameters(_ = (_ )

#### values()
