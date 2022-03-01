# minos.networks.scheduling.schedulers module


### _class_ minos.networks.scheduling.schedulers.PeriodicTask(crontab, fn)
Bases: `object`

Periodic Task class.


#### \__init__(crontab, fn)

#### _property_ crontab(_: crontab._crontab.CronTa_ )
Get the crontab of the periodic task.


* **Return type**

    `crontab._crontab.CronTab`



* **Returns**

    A `CronTab` instance.



#### _property_ fn(_: Callable[[[minos.networks.scheduling.requests.ScheduledRequest](minos.networks.scheduling.requests.md#minos.networks.scheduling.requests.ScheduledRequest)], Awaitable[None]_ )
Get the function to be called periodically.


* **Return type**

    `typing.Callable`[[[`minos.networks.scheduling.requests.ScheduledRequest`](minos.networks.scheduling.requests.md#minos.networks.scheduling.requests.ScheduledRequest)], `typing.Awaitable`[`None`]]



* **Returns**

    A function returning an awaitable.



#### _async_ run_forever()
Run the periodic function forever. This method is equivalent to start, but it keeps waiting until infinite.


* **Return type**

    `typing.NoReturn`



* **Returns**

    This method never returns.



#### _async_ run_once(now=None)
Run the periodic function one time.


* **Parameters**

    **now** (`typing.Optional`[`datetime.datetime`]) – An optional datetime expressing the current datetime.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _property_ running(_: boo_ )
Check if the periodic function is running.


* **Return type**

    `bool`



* **Returns**

    `True` if it’s running or `False` otherwise.



#### _async_ start()
Start the periodic task.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _property_ started(_: boo_ )
Check if the periodic task has been started.


* **Return type**

    `bool`



* **Returns**

    `True` if started or `False` otherwise.



#### _async_ stop(timeout=None)
Stop the periodic task.


* **Parameters**

    **timeout** (`typing.Optional`[`float`]) – An optional timeout expressed in seconds.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _property_ task(_: _asyncio.Tas_ )
Get the asyncio task.


* **Return type**

    `_asyncio.Task`



* **Returns**

    An `asyncio.Task` instance.



### _class_ minos.networks.scheduling.schedulers.PeriodicTaskScheduler(tasks, \*args, \*\*kwargs)
Bases: `minos.common.setup.MinosSetup`

Periodic Task Scheduler class.


#### \__init__(tasks, \*args, \*\*kwargs)

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



#### _async_ setup()
Setup miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ start()
Start the execution of periodic tasks.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ stop(timeout=None)
Stop the execution of periodic tasks.


* **Parameters**

    **timeout** (`typing.Optional`[`float`]) – An optional timeout expressed in seconds.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _property_ tasks(_: set[minos.networks.scheduling.schedulers.PeriodicTask_ )
Get the set of periodic tasks.


* **Return type**

    `set`[`minos.networks.scheduling.schedulers.PeriodicTask`]



* **Returns**

    A `set` of `PeriodicTask` instances.
