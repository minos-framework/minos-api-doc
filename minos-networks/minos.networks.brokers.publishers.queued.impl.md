# minos.networks.brokers.publishers.queued.impl module


### _class_ minos.networks.brokers.publishers.queued.impl.QueuedBrokerPublisher(impl, queue, \*args, \*\*kwargs)
Bases: [`minos.networks.brokers.publishers.abc.BrokerPublisher`](minos.networks.brokers.publishers.abc.md#minos.networks.brokers.publishers.abc.BrokerPublisher)

Queued Broker Publisher class.


#### \__init__(impl, queue, \*args, \*\*kwargs)

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



#### impl(_: [minos.networks.brokers.publishers.abc.BrokerPublisher](minos.networks.brokers.publishers.abc.md#minos.networks.brokers.publishers.abc.BrokerPublisher_ )

#### queue(_: [minos.networks.brokers.publishers.queued.queues.abc.BrokerPublisherQueue](minos.networks.brokers.publishers.queued.queues.abc.md#minos.networks.brokers.publishers.queued.queues.abc.BrokerPublisherQueue_ )

#### _async_ send(message)
Send a message.


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
