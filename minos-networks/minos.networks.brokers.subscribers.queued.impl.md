# minos.networks.brokers.subscribers.queued.impl module


### _class_ minos.networks.brokers.subscribers.queued.impl.QueuedBrokerSubscriber(impl, queue, \*\*kwargs)
Bases: [`minos.networks.brokers.subscribers.abc.BrokerSubscriber`](minos.networks.brokers.subscribers.abc.md#minos.networks.brokers.subscribers.abc.BrokerSubscriber)

Queued Broker Subscriber class.


#### \__init__(impl, queue, \*\*kwargs)

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



#### impl(_: [minos.networks.brokers.subscribers.abc.BrokerSubscriber](minos.networks.brokers.subscribers.abc.md#minos.networks.brokers.subscribers.abc.BrokerSubscriber_ )

#### queue(_: [minos.networks.brokers.subscribers.queued.queues.abc.BrokerSubscriberQueue](minos.networks.brokers.subscribers.queued.queues.abc.md#minos.networks.brokers.subscribers.queued.queues.abc.BrokerSubscriberQueue_ )

#### _async_ receive()
Receive a new message.


* **Return type**

    [`minos.networks.brokers.messages.models.abc.BrokerMessage`](minos.networks.brokers.messages.models.abc.md#minos.networks.brokers.messages.models.abc.BrokerMessage)



* **Returns**

    A `BrokerMessage` instance.



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



### _class_ minos.networks.brokers.subscribers.queued.impl.QueuedBrokerSubscriberBuilder(\*args, impl_builder, queue_builder, \*\*kwargs)
Bases: [`minos.networks.brokers.subscribers.abc.BrokerSubscriberBuilder`](minos.networks.brokers.subscribers.abc.md#minos.networks.brokers.subscribers.abc.BrokerSubscriberBuilder)

Queued Broker Subscriber Publisher class.


#### \__init__(\*args, impl_builder, queue_builder, \*\*kwargs)

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



#### build()
Build the instance.


* **Return type**

    [`minos.networks.brokers.subscribers.abc.BrokerSubscriber`](minos.networks.brokers.subscribers.abc.md#minos.networks.brokers.subscribers.abc.BrokerSubscriber)



* **Returns**

    A `QueuedBrokerSubscriber` instance.



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

    [`minos.networks.brokers.subscribers.abc.BrokerSubscriberBuilder`](minos.networks.brokers.subscribers.abc.md#minos.networks.brokers.subscribers.abc.BrokerSubscriberBuilder)



* **Returns**

    This method return the builder instance.



#### with_group_id(group_id)
Set group_id.


* **Parameters**

    **group_id** (`typing.Optional`[`str`]) – The group_id to be set.



* **Return type**

    [`minos.networks.brokers.subscribers.abc.BrokerSubscriberBuilder`](minos.networks.brokers.subscribers.abc.md#minos.networks.brokers.subscribers.abc.BrokerSubscriberBuilder)



* **Returns**

    This method return the builder instance.



#### with_kwargs(kwargs)
Set kwargs.


* **Parameters**

    **kwargs** (`dict`[`str`, `typing.Any`]) – The kwargs to be set.



* **Return type**

    [`minos.networks.brokers.subscribers.abc.BrokerSubscriberBuilder`](minos.networks.brokers.subscribers.abc.md#minos.networks.brokers.subscribers.abc.BrokerSubscriberBuilder)



* **Returns**

    This method return the builder instance.



#### with_remove_topics_on_destroy(remove_topics_on_destroy)
Set remove_topics_on_destroy.


* **Parameters**

    **remove_topics_on_destroy** (`bool`) – The remove_topics_on_destroy flag to be set.



* **Return type**

    [`minos.networks.brokers.subscribers.abc.BrokerSubscriberBuilder`](minos.networks.brokers.subscribers.abc.md#minos.networks.brokers.subscribers.abc.BrokerSubscriberBuilder)



* **Returns**

    This method return the builder instance.



#### with_topics(topics)
Set topics.


* **Parameters**

    **topics** (`collections.abc.Iterable`[`str`]) – The topics to be set.



* **Return type**

    [`minos.networks.brokers.subscribers.abc.BrokerSubscriberBuilder`](minos.networks.brokers.subscribers.abc.md#minos.networks.brokers.subscribers.abc.BrokerSubscriberBuilder)



* **Returns**

    This method return the builder instance.
