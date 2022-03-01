# minos.networks.brokers.clients module


### _class_ minos.networks.brokers.clients.BrokerClient(topic, publisher, subscriber, \*\*kwargs)
Bases: `minos.common.setup.MinosSetup`

Broker Client class.


#### \__init__(topic, publisher, subscriber, \*\*kwargs)

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



#### _classmethod_ from_config(config=None, \*\*kwargs)
Build a new instance from config.


* **Parameters**

    
    * **config** (`typing.Union`[`minos.common.configuration.config.MinosConfig`, `pathlib.Path`, `None`]) – Config instance. If None is provided, default config is chosen.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`S`, bound= `minos.common.setup.MinosSetup`)



* **Returns**

    A instance of the called class.



#### _async_ receive(\*args, \*\*kwargs)
Get one handler entry from the given topics.


* **Parameters**

    
    * **args** – Additional positional parameters to be passed to receive_many.


    * **kwargs** – Additional named parameters to be passed to receive_many.



* **Return type**

    [`minos.networks.brokers.messages.models.abc.BrokerMessage`](minos.networks.brokers.messages.models.abc.md#minos.networks.brokers.messages.models.abc.BrokerMessage)



* **Returns**

    A `HandlerEntry` instance.



#### _async_ receive_many(count, timeout=60, \*\*kwargs)
Get multiple handler entries from the given topics.


* **Parameters**

    
    * **timeout** (`float`) – Maximum time in seconds to wait for messages.


    * **count** (`int`) – Number of entries to be collected.



* **Return type**

    `collections.abc.AsyncIterator`[[`minos.networks.brokers.messages.models.abc.BrokerMessage`](minos.networks.brokers.messages.models.abc.md#minos.networks.brokers.messages.models.abc.BrokerMessage)]



* **Returns**

    A list of `HandlerEntry` instances.



#### _async_ send(message)
Send a `BrokerMessage`.


* **Parameters**

    **message** ([`minos.networks.brokers.messages.models.abc.BrokerMessage`](minos.networks.brokers.messages.models.abc.md#minos.networks.brokers.messages.models.abc.BrokerMessage)) – The message to be sent.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ setup()
Setup miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.
