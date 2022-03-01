# minos.networks.decorators.callables.checkers module


### _class_ minos.networks.decorators.callables.checkers.CheckerMeta(func, max_attempts, delay)
Bases: `object`

Checker Meta class.


#### \__init__(func, max_attempts, delay)

#### async_wrapper()
Get the async `HandlerWrapper` instance.


* **Returns**

    A `HandlerWrapper` instance.



#### delay(_: floa_ )

#### func(_: collections.abc.Callable[[[minos.networks.requests.abc.Request](minos.networks.requests.abc.md#minos.networks.requests.abc.Request)], Union[bool, None, collections.abc.Awaitable[Optional[bool]]]_ )

#### max_attempts(_: in_ )

#### _async static_ run_async(metas, \*args, \*\*kwargs)
Run a set of checkers asynchronously.


* **Parameters**

    
    * **metas** (`set`[`minos.networks.decorators.callables.checkers.CheckerMeta`]) – The set of checkers.


    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _static_ run_sync(metas, \*args, \*\*kwargs)
Run a set of checkers synchronously.


* **Parameters**

    
    * **metas** (`set`[`minos.networks.decorators.callables.checkers.CheckerMeta`]) – The set of checkers.


    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `bool`



* **Returns**

    This method does not return anything.



#### sync_wrapper()
Get the sync `HandlerWrapper` instance.


* **Returns**

    A `HandlerWrapper` instance.



#### _property_ wrapper(_: minos.networks.decorators.callables.checkers.CheckerWrappe_ )
Get the `HandlerWrapper` instance.


* **Return type**

    `minos.networks.decorators.callables.checkers.CheckerWrapper`



* **Returns**

    A `HandlerWrapper` instance.



### _class_ minos.networks.decorators.callables.checkers.CheckerWrapper(\*args, \*\*kwargs)
Bases: `Protocol`

Checker Wrapper class.


#### \__init__(\*args, \*\*kwargs)

#### meta(_: minos.networks.decorators.callables.checkers.CheckerMet_ )
