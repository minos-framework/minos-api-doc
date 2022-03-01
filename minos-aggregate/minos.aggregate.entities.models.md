# minos.aggregate.entities.models module


### _class_ minos.aggregate.entities.models.Entity(\*args, uuid=None, \*\*kwargs)
Bases: `minos.common.model.declarative.DeclarativeModel`

Entity class.


#### \__init__(\*args, uuid=None, \*\*kwargs)
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



#### avro_schema(_ = [{'name': 'Entity', 'namespace': 'minos.aggregate.entities.models.ae52f22a-5558-4763-a510-1ce164f20ffe', 'type': 'record', 'fields': [{'name': 'uuid', 'type': {'type': 'string', 'logicalType': 'uuid'}}]}_ )

#### _property_ avro_str(_: st_ )
Generate bytes representation of the current instance.


* **Return type**

    `str`



* **Returns**

    A bytes object.



#### classname(_ = 'minos.aggregate.entities.models.Entity_ )

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

#### uuid(_: UUI_ )

#### values()

### _class_ minos.aggregate.entities.models.ExternalEntity(uuid, \*args, \*\*kwargs)
Bases: `minos.aggregate.entities.models.Entity`

External Entity class.


#### \__init__(uuid, \*args, \*\*kwargs)
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



#### _property_ avro_str(_: st_ )
Generate bytes representation of the current instance.


* **Return type**

    `str`



* **Returns**

    A bytes object.



#### classname(_ = 'minos.aggregate.entities.models.ExternalEntity_ )

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



#### type_hints_parameters(_ = (_ )

#### uuid(_: UUI_ )

#### values()

#### version(_: in_ )

### _class_ minos.aggregate.entities.models.RootEntity(\*args, uuid=UUID('00000000-0000-0000-0000-000000000000'), version=0, created_at=datetime.datetime(9999, 12, 31, 23, 59, 59, 999999, tzinfo=datetime.timezone.utc), updated_at=datetime.datetime(9999, 12, 31, 23, 59, 59, 999999, tzinfo=datetime.timezone.utc), _event_repository=<dependency_injector.wiring.Provide object>, _snapshot_repository=<dependency_injector.wiring.Provide object>, \*\*kwargs)
Bases: `minos.aggregate.entities.models.Entity`

Base Root Entity class.


#### \__init__(\*args, uuid=UUID('00000000-0000-0000-0000-000000000000'), version=0, created_at=datetime.datetime(9999, 12, 31, 23, 59, 59, 999999, tzinfo=datetime.timezone.utc), updated_at=datetime.datetime(9999, 12, 31, 23, 59, 59, 999999, tzinfo=datetime.timezone.utc), _event_repository=<dependency_injector.wiring.Provide object>, _snapshot_repository=<dependency_injector.wiring.Provide object>, \*\*kwargs)
Class constructor.


* **Parameters**

    **kwargs** – Named arguments to be set as model attributes.



#### apply_diff(event)
Apply the differences over the instance.


* **Parameters**

    **event** ([`minos.aggregate.events.models.Event`](minos.aggregate.events.models.md#minos.aggregate.events.models.Event)) – The `FieldDiffContainer` containing the values to be set.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



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



#### classname(_ = 'minos.aggregate.entities.models.RootEntity_ )

#### _async classmethod_ create(\*args, \*\*kwargs)
Create a new `RootEntity` instance.


* **Parameters**

    
    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`T`, bound= `minos.aggregate.entities.models.RootEntity`)



* **Returns**

    A new `RootEntity` instance.



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



#### _async_ delete()
Delete the given root entity instance.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### diff(another)
Compute the difference with another instance.

Both `RootEntity` instances (`self` and `another`) must share the same `uuid` value.


* **Parameters**

    **another** (`minos.aggregate.entities.models.RootEntity`) – Another `RootEntity` instance.



* **Return type**

    [`minos.aggregate.events.models.Event`](minos.aggregate.events.models.md#minos.aggregate.events.models.Event)



* **Returns**

    An `FieldDiffContainer` instance.



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



#### _classmethod_ find(cls, condition, ordering=None, limit=None, \*, _snapshot_repository=<dependency_injector.wiring.Provide object>, \*\*kwargs)
Find a collection of instances based on a given `Condition`.


* **Parameters**

    
    * **condition** (`minos.aggregate.queries._Condition`) – The `Condition` that must be satisfied by all the instances.


    * **ordering** (`typing.Optional`[`minos.aggregate.queries._Ordering`]) – Optional argument to return the instance with specific ordering strategy. The default behaviour
    is to retrieve them without any order pattern.


    * **limit** (`typing.Optional`[`int`]) – Optional argument to return only a subset of instances. The default behaviour is to return all the
    instances that meet the given condition.


    * **_snapshot_repository** ([`minos.aggregate.snapshots.abc.SnapshotRepository`](minos.aggregate.snapshots.abc.md#minos.aggregate.snapshots.abc.SnapshotRepository)) – Snapshot to be set to the instances.



* **Return type**

    `typing.AsyncIterator`[`typing.TypeVar`(`T`, bound= `minos.aggregate.entities.models.RootEntity`)]



* **Returns**

    An asynchronous iterator of `RootEntity` instances.



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



#### _classmethod_ from_diff(event, \*args, \*\*kwargs)
Build a new instance from an `Event`.


* **Parameters**

    
    * **event** ([`minos.aggregate.events.models.Event`](minos.aggregate.events.models.md#minos.aggregate.events.models.Event)) – The difference that contains the data.


    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`T`, bound= `minos.aggregate.entities.models.RootEntity`)



* **Returns**

    A new `RootEntity` instance.



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



#### _async classmethod_ get(cls, uuid, \*, _snapshot_repository=<dependency_injector.wiring.Provide object>, \*\*kwargs)
Get one instance from the database based on its identifier.


* **Parameters**

    
    * **uuid** (`uuid.UUID`) – The identifier of the instance.


    * **_snapshot_repository** ([`minos.aggregate.snapshots.abc.SnapshotRepository`](minos.aggregate.snapshots.abc.md#minos.aggregate.snapshots.abc.SnapshotRepository)) – Snapshot to be set to the root entity.



* **Return type**

    `typing.TypeVar`(`T`, bound= `minos.aggregate.entities.models.RootEntity`)



* **Returns**

    A `RootEntity` instance.



#### _classmethod_ get_all(cls, ordering=None, limit=None, \*, _snapshot_repository=<dependency_injector.wiring.Provide object>, \*\*kwargs)
Get all instance from the database.


* **Parameters**

    
    * **ordering** (`typing.Optional`[`minos.aggregate.queries._Ordering`]) – Optional argument to return the instance with specific ordering strategy. The default behaviour
    is to retrieve them without any order pattern.


    * **limit** (`typing.Optional`[`int`]) – Optional argument to return only a subset of instances. The default behaviour is to return all the
    instances that meet the given condition.


    * **_snapshot_repository** ([`minos.aggregate.snapshots.abc.SnapshotRepository`](minos.aggregate.snapshots.abc.md#minos.aggregate.snapshots.abc.SnapshotRepository)) – Snapshot to be set to the root entity.



* **Return type**

    `typing.AsyncIterator`[`typing.TypeVar`(`T`, bound= `minos.aggregate.entities.models.RootEntity`)]



* **Returns**

    A `RootEntity` instance.



#### items()

#### keys()

#### _async_ refresh()
Refresh the state of the given instance.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ save()
Store the current instance on the repository.

If didn’t exist previously creates a new one, otherwise updates the existing one.


* **Return type**

    `None`



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



#### type_hints_parameters(_ = (_ )

#### _async_ update(\*\*kwargs)
Update an existing `RootEntity` instance.


* **Parameters**

    **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`T`, bound= `minos.aggregate.entities.models.RootEntity`)



* **Returns**

    An updated `RootEntity`  instance.



#### updated_at(_: datetim_ )

#### uuid(_: UUI_ )

#### values()

#### version(_: in_ )
