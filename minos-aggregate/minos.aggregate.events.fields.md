# minos.aggregate.events.fields module


### _class_ minos.aggregate.events.fields.FieldDiff(name, type_, value, \*\*kwargs)
Bases: `minos.common.model.abc.Model`, `Generic`[`minos.aggregate.events.fields.T`]

Field Diff class.


#### \__init__(name, type_, value, \*\*kwargs)
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



#### avro_schema(_ = [{'name': 'FieldDiff', 'namespace': 'minos.aggregate.events.fields.60b785c5-7d78-49fa-bb86-288b34246dc4', 'type': 'record', 'fields': []}_ )

#### _property_ avro_str(_: st_ )
Generate bytes representation of the current instance.


* **Return type**

    `str`



* **Returns**

    A bytes object.



#### classname(_ = 'minos.aggregate.events.fields.FieldDiff_ )

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



#### _classmethod_ from_model_type(model_type, \*args, \*\*kwargs)
Build a new instance from model type.


* **Parameters**

    
    * **model_type** (`minos.common.model.types.model_types.ModelType`) – The model type.


    * **args** – Additional positional. arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `minos.aggregate.events.fields.FieldDiff`



* **Returns**

    A new `FieldDiff` instance.



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

#### model_type()
alias of `minos.common.model.types.model_types.FieldDiff`


#### name(_: st_ )

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



#### type_hints(_ = {_ )

#### type_hints_parameters(_ = (~T,_ )

#### value(_: minos.aggregate.events.fields._ )

#### values()

### _class_ minos.aggregate.events.fields.FieldDiffContainer(diffs=None, fields=None, \*\*kwargs)
Bases: `minos.common.model.dynamic.bucket.BucketModel`

Field Diff Container class.


#### \__init__(diffs=None, fields=None, \*\*kwargs)
Class constructor.


* **Parameters**

    **fields** (`typing.Union`[`typing.Iterable`[`minos.common.model.fields.Field`], `dict`[`str`, `minos.common.model.fields.Field`], `None`]) – Dictionary that contains the `Field` instances of the model indexed by name.



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



#### avro_schema(_ = [{'name': 'FieldDiffContainer', 'namespace': 'minos.aggregate.events.fields.afc07cad-3fca-4860-8d37-ff405b3c721b', 'type': 'record', 'fields': []}_ )

#### _property_ avro_str(_: st_ )
Generate bytes representation of the current instance.


* **Return type**

    `str`



* **Returns**

    A bytes object.



#### classname(_ = 'minos.aggregate.events.fields.FieldDiffContainer_ )

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



#### _classmethod_ empty()
Build an empty `BucketModel` instance.


* **Return type**

    `typing.TypeVar`(`T`, bound= `minos.common.model.dynamic.bucket.BucketModel`)



* **Returns**

    A `BucketModel` instance.



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



#### flatten_items()
Get the field differences in a flatten way.


* **Return type**

    `typing.Iterator`[`tuple`[`str`, `minos.aggregate.events.fields.FieldDiff`]]



* **Returns**

    An `Iterator` of `tuple[str, FieldDiff]` instances.



#### flatten_values()
Get the field differences in a flatten way.


* **Return type**

    `typing.Iterator`[`minos.aggregate.events.fields.FieldDiff`]



* **Returns**

    An `Iterator` of `FieldDiff` instances.



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



#### _classmethod_ from_difference(a, b, ignore=frozenset({}))
Build a new instance from the difference between two models.


* **Parameters**

    
    * **a** (`minos.common.model.abc.Model`) – Latest model instance.


    * **b** (`minos.common.model.abc.Model`) – Oldest model instance.


    * **ignore** (`set`[`str`]) – Set of fields to be ignored.



* **Return type**

    `minos.aggregate.events.fields.FieldDiffContainer`



* **Returns**

    A new `FieldDiffContainer` instance.



#### _classmethod_ from_model(model, ignore=frozenset({}))
Build a new difference from a single model.


* **Parameters**

    
    * **model** (`minos.common.model.abc.Model`) – The model instance.


    * **ignore** (`set`[`str`]) – Set of fields to be ignored.



* **Return type**

    `minos.aggregate.events.fields.FieldDiffContainer`



* **Returns**

    A new `FieldDiffContainer` instance.



#### _classmethod_ from_model_type(model_type, \*args, \*\*kwargs)
Build a `DynamicModel` from a `ModelType`.


* **Parameters**

    
    * **model_type** (`minos.common.model.types.model_types.ModelType`) – `ModelType` object containing the model structure


    * **args** – Positional arguments to be passed to the model constructor.


    * **kwargs** – Named arguments to be passed to the model constructor.



* **Return type**

    `typing.TypeVar`(`T`, bound= `minos.common.model.dynamic.abc.DynamicModel`)



* **Returns**

    A new `DynamicModel` instance.



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



#### _static_ generate_random_str()
Generate a random string


* **Return type**

    `str`



* **Returns**

    A random string value.



#### get(k, )

#### get_all(return_diff=True)
Get a dictionary containing all names as keys and all the values of each one as values.


* **Parameters**

    **return_diff** (`bool`) – If `True` the result is returned as field diff instances, otherwise the result is
    returned as value instances.



* **Return type**

    `dict`[`str`, `typing.Union`[`minos.aggregate.events.fields.FieldDiff`, `typing.Any`, `list`[`minos.aggregate.events.fields.FieldDiff`], `list`[`typing.Any`]]]



* **Returns**

    A `dict` with `str` keys and `list[Any]` values.



#### get_one(name, return_diff=True)
Get first field diff with given name.


* **Parameters**

    
    * **name** (`str`) – The name of the field diff.


    * **return_diff** (`bool`) – If `True` the result is returned as field diff instances, otherwise the result is
    returned as value instances.



* **Return type**

    `typing.Union`[`minos.aggregate.events.fields.FieldDiff`, `typing.Any`, `list`[`minos.aggregate.events.fields.FieldDiff`], `list`[`typing.Any`]]



* **Returns**

    A `FieldDiff` instance.



#### items()

#### keys()

#### model_type()
alias of `minos.common.model.types.model_types.FieldDiffContainer`


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



#### type_hints(_ = {_ )

#### type_hints_parameters(_ = (_ )

#### values()

### _class_ minos.aggregate.events.fields.IncrementalFieldDiff(name, type_, value, action, \*\*kwargs)
Bases: `minos.aggregate.events.fields.FieldDiff`, `Generic`[`minos.aggregate.events.fields.T`]

Incremental Field Diff class.


#### \__init__(name, type_, value, action, \*\*kwargs)
Class constructor.


* **Parameters**

    **fields** – Dictionary that contains the `Field` instances of the model indexed by name.



#### action(_: [minos.aggregate.actions.Action](minos.aggregate.actions.md#minos.aggregate.actions.Action_ )

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



#### avro_schema(_ = [{'name': 'IncrementalFieldDiff', 'namespace': 'minos.aggregate.events.fields.0e185514-2212-4e22-9daf-c330920aca90', 'type': 'record', 'fields': []}_ )

#### _property_ avro_str(_: st_ )
Generate bytes representation of the current instance.


* **Return type**

    `str`



* **Returns**

    A bytes object.



#### classname(_ = 'minos.aggregate.events.fields.IncrementalFieldDiff_ )

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



#### _classmethod_ from_model_type(model_type, \*args, \*\*kwargs)
Build a new instance from model type.


* **Parameters**

    
    * **model_type** (`minos.common.model.types.model_types.ModelType`) – The model type.


    * **args** – Additional positional. arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `minos.aggregate.events.fields.FieldDiff`



* **Returns**

    A new `FieldDiff` instance.



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

#### model_type()
alias of `minos.common.model.types.model_types.IncrementalFieldDiff`


#### name(_: st_ )

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



#### type_hints(_ = {_ )

#### type_hints_parameters(_ = (~T,_ )

#### value(_: minos.aggregate.events.fields._ )

#### values()
