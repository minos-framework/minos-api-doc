# minos.saga.messages module


### _class_ minos.saga.messages.SagaRequest(target, content=None)
Bases: `object`

Saga Request class.


#### \__init__(target, content=None)

#### _async_ content(\*\*kwargs)
Get the content of the request.


* **Parameters**

    **kwargs** – Additional named parameters.



* **Return type**

    `typing.Any`



* **Returns**

    The content of the request.



#### _property_ target(_: st_ )
Get the target of the request.


* **Return type**

    `str`



* **Returns**

    A `str` instance.



### _class_ minos.saga.messages.SagaResponse(content=None, related_services=None, status=None, uuid=None, \*args, \*\*kwargs)
Bases: `object`

Saga Response class.


#### \__init__(content=None, related_services=None, status=None, uuid=None, \*args, \*\*kwargs)

#### _async_ content(\*\*kwargs)
Get the response content.


* **Parameters**

    **kwargs** – Additional named parameters.



* **Return type**

    `typing.Any`



* **Returns**

    The content of the response.



#### _classmethod_ from_message(message)
Build a new `SagaResponse` from a `BrokerMessage`.


* **Parameters**

    **message** (`minos.networks.brokers.messages.models.abc.BrokerMessage`) – The `BrokerMessage` instance.



* **Return type**

    `minos.saga.messages.SagaResponse`



* **Returns**

    A `SagaResponse`.



#### _property_ ok(_: boo_ )
Check if the response is okay.


* **Return type**

    `bool`



* **Returns**

    `True` if the response is okay



#### _property_ related_services(_: set[str_ )
Get the microservice name that generated the response.


* **Return type**

    `set`[`str`]



* **Returns**

    An string value containing the microservice name.



#### _property_ status(_: minos.saga.messages.SagaResponseStatu_ )
Get the status code of the response.


* **Return type**

    `minos.saga.messages.SagaResponseStatus`



* **Returns**

    A `ResponseStatus` instance.



#### _property_ uuid(_: uuid.UUI_ )
Get the identifier of the saga execution that must receive the response.


* **Return type**

    `uuid.UUID`



* **Returns**

    An `UUID` value.



### _class_ minos.saga.messages.SagaResponseStatus(value)
Bases: `enum.IntEnum`

Saga Response Status class.


#### ERROR(_ = 40_ )

#### SUCCESS(_ = 20_ )

#### SYSTEM_ERROR(_ = 50_ )

#### _classmethod_ from_raw(raw)
Build a new instance from raw.


* **Parameters**

    **raw** (`int`) – The raw representation of the instance.



* **Return type**

    `minos.saga.messages.SagaResponseStatus`



* **Returns**

    A `SagaResponseStatus` instance.
