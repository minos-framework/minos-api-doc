# minos.networks.requests.memory module


### _class_ minos.networks.requests.memory.InMemoryRequest(content=<object object>, params=<object object>, user=None, \*args, \*\*kwargs)
Bases: [`minos.networks.requests.abc.Request`](minos.networks.requests.abc.md#minos.networks.requests.abc.Request)

In Memory Request class.


#### \__init__(content=<object object>, params=<object object>, user=None, \*args, \*\*kwargs)

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
For testing purposes


* **Return type**

    `typing.Optional`[`uuid.UUID`]
