# minos.networks.brokers.handlers.services module


### _class_ minos.networks.brokers.handlers.services.BrokerHandlerService(\*\*kwargs)
Bases: `aiomisc.service.base.Service`

Broker Handler Service class.


#### \__init__(\*\*kwargs)

#### _property_ context(_: aiomisc.context.Contex_ )

* **Return type**

    `aiomisc.context.Context`



#### handler()
Get the service handler.


* **Returns**

    A `Handler` instance.



#### set_loop(loop)

* **Return type**

    `None`



#### _async_ start()
Start the service execution.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _property_ start_event(_: asyncio.locks.Even_ )

* **Return type**

    `asyncio.locks.Event`



#### _async_ stop(err=None)
Stop the service execution.


* **Parameters**

    **err** (`typing.Optional`[`Exception`]) – Optional exception that stopped the execution.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.
