# minos.networks.brokers.dispatchers.requests module


### _class_ minos.networks.brokers.dispatchers.requests.BrokerRequest(raw, \*args, \*\*kwargs)
Bases: [`minos.networks.requests.abc.Request`](minos.networks.requests.abc.md#minos.networks.requests.abc.Request)

Handler Request class.


#### \__init__(raw, \*args, \*\*kwargs)

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



#### _property_ headers(_: dict[str, str_ )
Get the headers of the request.


* **Return type**

    `dict`[`str`, `str`]



* **Returns**

    A dictionary in which keys are `str` instances and values are `str` instances.



#### _async_ params(\*\*kwargs)
Get the request params.


* **Parameters**

    **kwargs** – Additional named arguments.



* **Return type**

    `dict`[`str`, `typing.Any`]



* **Returns**

    The request params.



#### raw()

#### user()
Returns the UUID of the user making the Request.


### _class_ minos.networks.brokers.dispatchers.requests.BrokerResponse(data=<object object>, \*, status=200)
Bases: [`minos.networks.requests.abc.Response`](minos.networks.requests.abc.md#minos.networks.requests.abc.Response)

Handler Response class.


#### \__init__(data=<object object>, \*, status=200)

#### _async_ content(\*\*kwargs)
Response content.


* **Parameters**

    **kwargs** – Additional named arguments.



* **Return type**

    `typing.Any`



* **Returns**

    A list of items.



#### _property_ has_content(_: boo_ )
Check if the request has content.


* **Return type**

    `bool`



* **Returns**

    `True` if it has content or `False` otherwise.



#### _property_ status(_: in_ )
The status code of the response.


* **Return type**

    `int`



* **Returns**

    An `int` value.



### _exception_ minos.networks.brokers.dispatchers.requests.BrokerResponseException(\*args, status=400)
Bases: [`minos.networks.requests.abc.ResponseException`](minos.networks.requests.abc.md#minos.networks.requests.abc.ResponseException)

Handler Response Exception class.


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
