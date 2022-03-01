# minos.networks.brokers.dispatchers.impl module


### _class_ minos.networks.brokers.dispatchers.impl.BrokerDispatcher(actions, publisher, \*\*kwargs)
Bases: `minos.common.setup.MinosSetup`

Broker Dispatcher class.


#### \__init__(actions, publisher, \*\*kwargs)

#### _property_ actions(_: dict[str, Optional[collections.abc.Callable]_ )
Actions getter.


* **Return type**

    `dict`[`str`, `typing.Optional`[`collections.abc.Callable`]]



* **Returns**

    A dictionary in which the keys are topics and the values are the handler.



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



#### _async_ dispatch(message)
Dispatch an entry.


* **Parameters**

    **message** ([`minos.networks.brokers.messages.models.abc.BrokerMessage`](minos.networks.brokers.messages.models.abc.md#minos.networks.brokers.messages.models.abc.BrokerMessage)) – The entry to be dispatched.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _classmethod_ from_config(config=None, \*\*kwargs)
Build a new instance from config.


* **Parameters**

    
    * **config** (`typing.Union`[`minos.common.configuration.config.MinosConfig`, `pathlib.Path`, `None`]) – Config instance. If None is provided, default config is chosen.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`S`, bound= `minos.common.setup.MinosSetup`)



* **Returns**

    A instance of the called class.



#### get_action(topic)
Get the handling function to be called.


* **Parameters**

    **topic** (`str`) – The name of the topic that matches the action.



* **Return type**

    `collections.abc.Callable`[[`minos.networks.requests.abc.Request`](minos.networks.requests.abc.md#minos.networks.requests.abc.Request), `typing.Union`[[`minos.networks.requests.abc.Response`](minos.networks.requests.abc.md#minos.networks.requests.abc.Response), `None`, `collections.abc.Awaitable`[`typing.Optional`[[`minos.networks.requests.abc.Response`](minos.networks.requests.abc.md#minos.networks.requests.abc.Response)]]]]



* **Returns**

    A `Callable` instance.



#### _static_ get_callback(fn)
Get the handler function to be used by the Broker Handler.


* **Parameters**

    **fn** (`collections.abc.Callable`[[`minos.networks.brokers.dispatchers.requests.BrokerRequest`](minos.networks.brokers.dispatchers.requests.md#minos.networks.brokers.dispatchers.requests.BrokerRequest), `typing.Union`[[`minos.networks.brokers.dispatchers.requests.BrokerResponse`](minos.networks.brokers.dispatchers.requests.md#minos.networks.brokers.dispatchers.requests.BrokerResponse), `None`, `collections.abc.Awaitable`[`typing.Optional`[[`minos.networks.brokers.dispatchers.requests.BrokerResponse`](minos.networks.brokers.dispatchers.requests.md#minos.networks.brokers.dispatchers.requests.BrokerResponse)]]]]) – The action function.



* **Return type**

    `collections.abc.Callable`[[`minos.networks.brokers.messages.models.abc.BrokerMessage`](minos.networks.brokers.messages.models.abc.md#minos.networks.brokers.messages.models.abc.BrokerMessage), `collections.abc.Awaitable`[[`minos.networks.brokers.messages.models.v1.BrokerMessageV1Payload`](minos.networks.brokers.messages.models.v1.md#minos.networks.brokers.messages.models.v1.BrokerMessageV1Payload)]]



* **Returns**

    A wrapper function around the given one that is compatible with the Broker Handler API.



#### _property_ publisher(_: [minos.networks.brokers.publishers.abc.BrokerPublisher](minos.networks.brokers.publishers.abc.md#minos.networks.brokers.publishers.abc.BrokerPublisher_ )
Get the publisher instance.


* **Return type**

    [`minos.networks.brokers.publishers.abc.BrokerPublisher`](minos.networks.brokers.publishers.abc.md#minos.networks.brokers.publishers.abc.BrokerPublisher)



* **Returns**

    A `BrokerPublisher` instance.



#### _async_ setup()
Setup miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.
