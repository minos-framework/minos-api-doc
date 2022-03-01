# minos.networks.rest.handlers module


### _class_ minos.networks.rest.handlers.RestHandler(host, port, endpoints, \*\*kwargs)
Bases: `minos.common.setup.MinosSetup`

Rest Handler class.


#### \__init__(host, port, endpoints, \*\*kwargs)

#### _property_ already_destroyed(_: boo_ )
Already Destroy getter.


* **Return type**

    `bool`



* **Returns**

    A boolean value.



#### _property_ already_setup(_: boo_ )
Already Setup getter.


* **Return type**

    `bool`



* **Returns**

    A boolean value.



#### _async_ destroy()
Destroy miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _property_ endpoints(_: dict[(<class 'str'>, <class 'str'>), typing.Callable_ )
Endpoints getter.


* **Return type**

    `dict`[(`str`, `str`), `typing.Callable`]



* **Returns**

    A dictionary value.



#### _classmethod_ from_config(config=None, \*\*kwargs)
Build a new instance from config.


* **Parameters**

    
    * **config** (`typing.Union`[`minos.common.configuration.config.MinosConfig`, `pathlib.Path`, `None`]) – Config instance. If None is provided, default config is chosen.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`S`, bound= `minos.common.setup.MinosSetup`)



* **Returns**

    A instance of the called class.



#### get_app()
Return rest application instance.


* **Return type**

    `aiohttp.web_app.Application`



* **Returns**

    A web.Application instance.



#### _static_ get_callback(fn)
Get the handler function to be used by the `aiohttp` Controller.


* **Parameters**

    **fn** (`typing.Callable`[[[`minos.networks.rest.requests.RestRequest`](minos.networks.rest.requests.md#minos.networks.rest.requests.RestRequest)], `typing.Union`[[`minos.networks.rest.requests.RestResponse`](minos.networks.rest.requests.md#minos.networks.rest.requests.RestResponse), `None`, `typing.Awaitable`[`typing.Optional`[[`minos.networks.rest.requests.RestResponse`](minos.networks.rest.requests.md#minos.networks.rest.requests.RestResponse)]]]]) – The action function.



* **Return type**

    `typing.Callable`[[`aiohttp.web_request.Request`], `typing.Awaitable`[`aiohttp.web_response.Response`]]



* **Returns**

    A wrapper function around the given one that is compatible with the `aiohttp` Controller.



#### _property_ host(_: st_ )
Get the rest host.


* **Return type**

    `str`



* **Returns**

    A `str` object.



#### _property_ port(_: in_ )
Get the rest port.


* **Return type**

    `int`



* **Returns**

    An integer value.



#### _async_ setup()
Setup miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.
