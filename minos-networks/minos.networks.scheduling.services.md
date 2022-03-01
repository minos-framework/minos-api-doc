# minos.networks.scheduling.services module


### _class_ minos.networks.scheduling.services.PeriodicTaskSchedulerService(\*\*kwargs)
Bases: `aiomisc.service.base.Service`

Task Scheduler Service class.


#### \__init__(\*\*kwargs)

#### _property_ context(_: aiomisc.context.Contex_ )

* **Return type**

    `aiomisc.context.Context`



#### scheduler()
Get the service scheduler.


* **Returns**

    A `PeriodicTaskScheduler` instance.



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



#### _async_ stop(exception=None)
Stop the service execution.


* **Parameters**

    **exception** (`typing.Optional`[`Exception`]) – Optional exception that stopped the execution.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.
