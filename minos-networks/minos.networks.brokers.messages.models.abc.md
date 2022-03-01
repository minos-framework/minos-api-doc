# minos.networks.brokers.messages.models.abc module


### _class_ minos.networks.brokers.messages.models.abc.BrokerMessage(fields=None, \*\*kwargs)
Bases: `abc.ABC`, `minos.common.model.abc.Model`

Broker Message base class.


#### \__init__(fields=None, \*\*kwargs)
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



#### avro_schema(_ = [{'name': 'BrokerMessage', 'namespace': 'minos.networks.brokers.messages.models.abc.5dc75ebf-1c18-450a-9049-3060251436ee', 'type': 'record', 'fields': []}_ )

#### _property_ avro_str(_: st_ )
Generate bytes representation of the current instance.


* **Return type**

    `str`



* **Returns**

    A bytes object.



#### classname(_ = 'minos.networks.brokers.messages.models.abc.BrokerMessage_ )

#### _abstract property_ content(_: An_ )
Get the content of the message.


* **Return type**

    `typing.Any`



* **Returns**

    Any value.



#### _classmethod_ decode_data(decoder, target, type_, \*\*kwargs)
Decode data with the given decoder.


* **Parameters**

    
    * **decoder** (`minos.common.model.serializers.abc.DataDecoder`) – The decoder instance.


    * **target** (`typing.Any`) – The data to be decoded.


    * **type** – The data type.



* **Return type**

    `minos.networks.brokers.messages.models.abc.BrokerMessage`



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



#### _classmethod_ encode_data(encoder, target, \*\*kwargs)
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


    * **target** (`minos.common.model.types.model_types.ModelType`) – An optional pre-encoded schema.



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



#### _abstract classmethod_ from_model_type(model_type, \*args, \*\*kwargs)
Build a `Model` from a `ModelType`.


* **Parameters**

    
    * **model_type** (`minos.common.model.types.model_types.ModelType`) – `ModelType` object containing the DTO’s structure


    * **args** – Positional arguments to be passed to the model constructor.


    * **kwargs** – Named arguments to be passed to the model constructor.



* **Return type**

    `typing.TypeVar`(`T`, bound= `minos.common.model.abc.Model`)



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

#### _abstract property_ headers(_: dict[str, str_ )
Get the headers of the message.


* **Return type**

    `dict`[`str`, `str`]



* **Returns**

    A `dict` instance with `str` keys and `str` values.



#### _abstract property_ identifier(_: uuid.UUI_ )
Get the identifier of the message.


* **Return type**

    `uuid.UUID`



* **Returns**

    An `UUID` instance.



#### items()

#### keys()

#### model_type()
alias of `minos.common.model.types.model_types.BrokerMessage`


#### _abstract property_ ok(_: boo_ )
Check if the message is okay or not.


* **Return type**

    `bool`



* **Returns**

    `True` if the message is okay or `False` otherwise.



#### _abstract property_ reply_topic(_: Optional[str_ )
Get the reply topic of the message if there is someone.


* **Return type**

    `typing.Optional`[`str`]



* **Returns**

    A `str` value or `None`.



#### _abstract_ set_reply_topic(value)
Set the message’s reply topic.


* **Parameters**

    **value** (`typing.Optional`[`str`]) – A `str` value or `None`.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _property_ should_reply(_: boo_ )

* **Return type**

    `bool`



* **Returns**

    


#### _abstract property_ status(_: in_ )
Get the status of the message.


* **Return type**

    `int`



* **Returns**

    An `int` instance.



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



#### _abstract property_ topic(_: st_ )
Get the topic of the message.


* **Return type**

    `str`



* **Returns**

    A `str` value.



#### type_hints(_ = {_ )

#### type_hints_parameters(_ = (_ )

#### values()

#### _abstract class property_ version(_: in_ )
Get the version of the message.


* **Return type**

    `int`



* **Returns**

    A strictly positive `int` value.
