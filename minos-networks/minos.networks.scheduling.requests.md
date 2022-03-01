# minos.networks.scheduling.requests module


### _class_ minos.networks.scheduling.requests.ScheduledRequest(scheduled_at, \*args, \*\*kwargs)
Bases: [`minos.networks.requests.abc.Request`](minos.networks.requests.abc.md#minos.networks.requests.abc.Request)

Scheduling Request class.


#### \__init__(scheduled_at, \*args, \*\*kwargs)

#### _async_ content(\*\*kwargs)
Get the request content.


* **Parameters**

    **kwargs** – Additional named arguments.



* **Return type**

    `typing.Any`



* **Returns**

    The request content.



#### _property_ has_content(_: boo_ )
Check if the request has content.


* **Return type**

    `bool`



* **Returns**

    `True` if it has content or `False` otherwise.



#### _property_ has_params(_: boo_ )
Check if the request has params.


* **Return type**

    `bool`



* **Returns**

    `True` if it has params or `False` otherwise.



#### _async_ params(\*\*kwargs)
Get the request params.


* **Parameters**

    **kwargs** – Additional named arguments.



* **Return type**

    `dict`[`str`, `typing.Any`]



* **Returns**

    The request params.



#### _property_ user(_: Optional[uuid.UUID_ )
The user of the request.


* **Return type**

    `typing.Optional`[`uuid.UUID`]



* **Returns**

    Always return `None` as scheduled request are launched by the system.



### _class_ minos.networks.scheduling.requests.ScheduledRequestContent(\*args, \*\*kwargs)
Bases: `minos.common.model.declarative.DeclarativeModel`

Scheduling Request Content class.


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



#### avro_schema(_ = [{'name': 'ScheduledRequestContent', 'namespace': 'minos.networks.scheduling.requests.42bc4f64-d7b7-41d7-b80d-3e6a1a92712f', 'type': 'record', 'fields': [{'name': 'scheduled_at', 'type': {'type': 'long', 'logicalType': 'timestamp-micros'}}]}_ )

#### _property_ avro_str(_: st_ )
Generate bytes representation of the current instance.


* **Return type**

    `str`



* **Returns**

    A bytes object.



#### classname(_ = 'minos.networks.scheduling.requests.ScheduledRequestContent_ )

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

#### scheduled_at(_: datetim_ )

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

### _exception_ minos.networks.scheduling.requests.ScheduledResponseException(\*args, status=400)
Bases: [`minos.networks.requests.abc.ResponseException`](minos.networks.requests.abc.md#minos.networks.requests.abc.ResponseException)

Scheduled Response Exception class.


#### \__init__(\*args, status=400)

#### args()

#### _property_ status(_: in_ )
The status code of the response.


* **Return type**

    `int`



* **Returns**

    An `int` value.



#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.
