# minos.networks.brokers.collections.queues.abc module


### _class_ minos.networks.brokers.collections.queues.abc.BrokerQueue(\*args, already_setup=False, \*\*kwargs)
Bases: `abc.ABC`, `minos.common.setup.MinosSetup`

Broker Queue class.


#### \__init__(\*args, already_setup=False, \*\*kwargs)

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
