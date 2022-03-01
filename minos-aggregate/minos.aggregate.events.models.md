# minos.aggregate.events.models module


### _class_ minos.aggregate.events.models.Event(\*args, \*\*kwargs)
Bases: `minos.common.model.declarative.DeclarativeModel`

Event class.


#### \__init__(\*args, \*\*kwargs)
Class constructor.


* **Parameters**

    **kwargs** – Named arguments to be set as model attributes.



#### action(_: [Action](minos.aggregate.actions.md#minos.aggregate.actions.Action_ )

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



#### avro_schema()

#### _property_ avro_str(_: st_ )
Generate bytes representation of the current instance.


* **Return type**

    `str`



* **Returns**

    A bytes object.



#### classname(_ = 'minos.aggregate.events.models.Event_ )

#### created_at(_: datetim_ )

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



#### decompose()
Decompose the `Event` fields into multiple `Event` instances with once Field.


* **Return type**

    `list`[`minos.aggregate.events.models.Event`]



* **Returns**

    An list of\`\`Event\`\` instances.



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



#### fields_diff(_: [FieldDiffContainer](minos.aggregate.events.fields.md#minos.aggregate.events.fields.FieldDiffContainer_ )

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



#### _classmethod_ from_deleted_root_entity(instance, action=Action.DELETE)
Build an `Event` from a `RootEntity` (considering all fields as differences).


* **Parameters**

    
    * **instance** ([`minos.aggregate.entities.models.RootEntity`](minos.aggregate.entities.models.md#minos.aggregate.entities.models.RootEntity)) – A `RootEntity` instance.


    * **action** ([`minos.aggregate.actions.Action`](minos.aggregate.actions.md#minos.aggregate.actions.Action)) – The action that generates the event.



* **Return type**

    `minos.aggregate.events.models.Event`



* **Returns**

    An `Event` instance.



#### _classmethod_ from_difference(a, b, action=Action.UPDATE)
Build an `Event` instance from the difference of two instances.


* **Parameters**

    
    * **a** ([`minos.aggregate.entities.models.RootEntity`](minos.aggregate.entities.models.md#minos.aggregate.entities.models.RootEntity)) – One `RootEntity` instance.


    * **b** ([`minos.aggregate.entities.models.RootEntity`](minos.aggregate.entities.models.md#minos.aggregate.entities.models.RootEntity)) – Another `RootEntity` instance.


    * **action** ([`minos.aggregate.actions.Action`](minos.aggregate.actions.md#minos.aggregate.actions.Action)) – The action that generates the `RootEntity` difference.



* **Return type**

    `minos.aggregate.events.models.Event`



* **Returns**

    An `Event` instance.



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



#### _classmethod_ from_root_entity(instance, action=Action.CREATE)
Build an `Event` from a `RootEntity` (considering all fields as differences).


* **Parameters**

    
    * **instance** ([`minos.aggregate.entities.models.RootEntity`](minos.aggregate.entities.models.md#minos.aggregate.entities.models.RootEntity)) – A `RootEntity` instance.


    * **action** ([`minos.aggregate.actions.Action`](minos.aggregate.actions.md#minos.aggregate.actions.Action)) – The action that generates the event.



* **Return type**

    `minos.aggregate.events.models.Event`



* **Returns**

    An `Event` instance.



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

#### get_all(return_diff=False)
Get all field diffs with given name.


* **Parameters**

    **return_diff** (`bool`) – If `True` the result is returned as field diff instances, otherwise the result is
    returned as value instances.



* **Return type**

    `dict`[`str`, `typing.Union`[[`minos.aggregate.events.fields.FieldDiff`](minos.aggregate.events.fields.md#minos.aggregate.events.fields.FieldDiff), `typing.Any`, `list`[[`minos.aggregate.events.fields.FieldDiff`](minos.aggregate.events.fields.md#minos.aggregate.events.fields.FieldDiff)], `list`[`typing.Any`]]]



* **Returns**

    A list of `FieldDiff` instances.



#### get_one(name, return_diff=False)
Get first field diff with given name.


* **Parameters**

    
    * **name** (`str`) – The name of the field diff.


    * **return_diff** (`bool`) – If `True` the result is returned as field diff instances, otherwise the result is
    returned as value instances.



* **Return type**

    `typing.Union`[[`minos.aggregate.events.fields.FieldDiff`](minos.aggregate.events.fields.md#minos.aggregate.events.fields.FieldDiff), `typing.Any`, `list`[[`minos.aggregate.events.fields.FieldDiff`](minos.aggregate.events.fields.md#minos.aggregate.events.fields.FieldDiff)], `list`[`typing.Any`]]



* **Returns**

    A `FieldDiff` instance.



#### items()

#### keys()

#### name(_: st_ )

#### _property_ simplified_name(_: st_ )
Get the RootEntity’s simplified name.


* **Return type**

    `str`



* **Returns**

    An string value.



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

#### uuid(_: UUI_ )

#### values()

#### version(_: in_ )
