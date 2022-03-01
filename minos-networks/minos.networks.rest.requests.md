# minos.networks.rest.requests module


### _class_ minos.networks.rest.requests.RestRequest(raw, \*args, \*\*kwargs)
Bases: [`minos.networks.requests.abc.Request`](minos.networks.requests.abc.md#minos.networks.requests.abc.Request)

Rest Request class.


#### \__init__(raw, \*args, \*\*kwargs)

#### _async_ content(\*\*kwargs)
Get the request content.


* **Parameters**

    **kwargs** – Additional named arguments.



* **Return type**

    `typing.Any`



* **Returns**

    The request content.



#### _property_ content_type(_: st_ )
Get the content type.


* **Return type**

    `str`



* **Returns**

    A `str` value.



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



#### _property_ has_query_params(_: boo_ )
Check if the request has query params.


* **Return type**

    `bool`



* **Returns**

    `True` if it has query params or `False` otherwise.



#### _property_ has_url_params(_: boo_ )
Check if the request has url params.


* **Return type**

    `bool`



* **Returns**

    `True` if it has url params or `False` otherwise.



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



#### _async_ query_params(type_=None, \*\*kwargs)
Get the query params.


* **Parameters**

    
    * **type** – Optional `type` or `str` (classname) that defines the request content type.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.Any`



* **Returns**

    A dictionary instance.



#### raw()

#### _property_ raw_request(_: aiohttp.web_request.Reques_ )
Get the raw request within the instance.


* **Return type**

    `aiohttp.web_request.Request`



* **Returns**

    An `aiohttp.web.Request` instance.



#### _async_ url_params(type_=None, \*\*kwargs)
Get the url params.


* **Parameters**

    
    * **type** – Optional `type` or `str` (classname) that defines the request content type.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.Any`



* **Returns**

    A dictionary instance.



#### user()
Returns the UUID of the user making the Request.


### _class_ minos.networks.rest.requests.RestResponse(\*args, content_type='application/json', \*\*kwargs)
Bases: [`minos.networks.requests.abc.Response`](minos.networks.requests.abc.md#minos.networks.requests.abc.Response)

Rest Response class.


#### \__init__(\*args, content_type='application/json', \*\*kwargs)

#### _async_ content(\*\*kwargs)
Raw response content.


* **Parameters**

    **kwargs** – Additional named arguments.



* **Return type**

    `typing.Optional`[`bytes`]



* **Returns**

    The raw content as a `bytes` instance.



#### _classmethod_ from_response(response)
Build a new `RestRequest` from another response.


* **Parameters**

    **response** (`typing.Optional`[[`minos.networks.requests.abc.Response`](minos.networks.requests.abc.md#minos.networks.requests.abc.Response)]) – The base response.



* **Return type**

    `minos.networks.rest.requests.RestResponse`



* **Returns**

    A `RestResponse` instance.



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



### _exception_ minos.networks.rest.requests.RestResponseException(\*args, status=400)
Bases: [`minos.networks.requests.abc.ResponseException`](minos.networks.requests.abc.md#minos.networks.requests.abc.ResponseException)

Rest Response Exception class.


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
