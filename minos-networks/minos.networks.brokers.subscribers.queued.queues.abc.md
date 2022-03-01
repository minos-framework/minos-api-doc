# minos.networks.brokers.subscribers.queued.queues.abc module


### _class_ minos.networks.brokers.subscribers.queued.queues.abc.BrokerSubscriberQueue(topics, \*\*kwargs)
Bases: [`minos.networks.brokers.collections.queues.abc.BrokerQueue`](minos.networks.brokers.collections.queues.abc.md#minos.networks.brokers.collections.queues.abc.BrokerQueue), `abc.ABC`

Broker Subscriber Queue class.


#### \__init__(topics, \*\*kwargs)

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



#### _async_ dequeue()
Dequeue method.


* **Return type**

    [`minos.networks.brokers.messages.models.abc.BrokerMessage`](minos.networks.brokers.messages.models.abc.md#minos.networks.brokers.messages.models.abc.BrokerMessage)



#### _async_ destroy()
Destroy miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ enqueue(message)
Enqueue method.


* **Return type**

    `None`



#### _classmethod_ from_config(config=None, \*\*kwargs)
Build a new instance from config.


* **Parameters**

    
    * **config** (`typing.Union`[`minos.common.configuration.config.MinosConfig`, `pathlib.Path`, `None`]) – Config instance. If None is provided, default config is chosen.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`S`, bound= `minos.common.setup.MinosSetup`)



* **Returns**

    A instance of the called class.



#### _async_ setup()
Setup miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _property_ topics(_: set[str_ )
Topics getter.


* **Return type**

    `set`[`str`]



* **Returns**

    A list of string values.



### _class_ minos.networks.brokers.subscribers.queued.queues.abc.BrokerSubscriberQueueBuilder(\*args, \*\*kwargs)
Bases: [`minos.networks.utils.Builder`](minos.networks.utils.md#minos.networks.utils.Builder)[`minos.networks.brokers.subscribers.queued.queues.abc.BrokerSubscriberQueue`], `abc.ABC`

Broker Subscriber Queue Builder class.


#### \__init__(\*args, \*\*kwargs)

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



#### _abstract_ build()
Build the instance.


* **Return type**

    `typing.TypeVar`(`Instance`)



* **Returns**

    A `BrokerSubscriber` instance.



#### copy()
Get a copy of the instance.


* **Return type**

    `typing.TypeVar`(`B`, bound= [`minos.networks.utils.Builder`](minos.networks.utils.md#minos.networks.utils.Builder))



* **Returns**

    A `BrokerSubscriberBuilder` instance.



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



#### _classmethod_ new()
Get a new instance.


* **Return type**

    `typing.TypeVar`(`B`, bound= [`minos.networks.utils.Builder`](minos.networks.utils.md#minos.networks.utils.Builder))



* **Returns**

    A `BrokerSubscriberBuilder` instance.



#### _async_ setup()
Setup miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### with_config(config)
Set config.


* **Parameters**

    **config** (`minos.common.configuration.config.MinosConfig`) – The config to be set.



* **Return type**

    `typing.TypeVar`(`B`, bound= [`minos.networks.utils.Builder`](minos.networks.utils.md#minos.networks.utils.Builder))



* **Returns**

    This method return the builder instance.



#### with_kwargs(kwargs)
Set kwargs.


* **Parameters**

    **kwargs** (`dict`[`str`, `typing.Any`]) – The kwargs to be set.



* **Return type**

    `typing.TypeVar`(`B`, bound= [`minos.networks.utils.Builder`](minos.networks.utils.md#minos.networks.utils.Builder))



* **Returns**

    This method return the builder instance.



#### with_topics(topics)
Set topics.


* **Parameters**

    **topics** (`collections.abc.Iterable`[`str`]) – The topics to be set.



* **Return type**

    `typing.TypeVar`(`B`, bound= `minos.networks.brokers.subscribers.queued.queues.abc.BrokerSubscriberQueueBuilder`)



* **Returns**

    This method return the builder instance.
