# minos.networks.decorators.callables.handlers module


### _class_ minos.networks.decorators.callables.handlers.HandlerMeta(func, decorators=None, checkers=None)
Bases: `object`

Handler Meta class.


#### \__init__(func, decorators=None, checkers=None)

#### add_decorator(decorator)
Add a new decorator to the `decorators` set.


* **Parameters**

    **decorator** ([`minos.networks.decorators.definitions.abc.EnrouteDecorator`](minos.networks.decorators.definitions.abc.md#minos.networks.decorators.definitions.abc.EnrouteDecorator)) – The decorator to be added.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### async_wrapper()
Get the async `HandlerWrapper` instance.


* **Returns**

    A `HandlerWrapper` instance.



#### check()
Get the check decorator.


* **Returns**

    A `CheckDecorator` type.



#### checkers(_: set[[minos.networks.decorators.callables.checkers.CheckerMeta](minos.networks.decorators.callables.checkers.md#minos.networks.decorators.callables.checkers.CheckerMeta)_ )

#### decorators(_: set[[minos.networks.decorators.definitions.abc.EnrouteDecorator](minos.networks.decorators.definitions.abc.md#minos.networks.decorators.definitions.abc.EnrouteDecorator)_ )

#### func(_: collections.abc.Callable[[[minos.networks.requests.abc.Request](minos.networks.requests.abc.md#minos.networks.requests.abc.Request)], Union[[minos.networks.requests.abc.Response](minos.networks.requests.abc.md#minos.networks.requests.abc.Response), None, collections.abc.Awaitable[Optional[[minos.networks.requests.abc.Response](minos.networks.requests.abc.md#minos.networks.requests.abc.Response)]]]_ )

#### sync_wrapper()
Get the sync `HandlerWrapper` instance.


* **Returns**

    A `HandlerWrapper` instance.



#### _property_ wrapper(_: minos.networks.decorators.callables.handlers.HandlerWrappe_ )
Get the `HandlerWrapper` instance.


* **Return type**

    `minos.networks.decorators.callables.handlers.HandlerWrapper`



* **Returns**

    A `HandlerWrapper` instance.



### _class_ minos.networks.decorators.callables.handlers.HandlerWrapper(\*args, \*\*kwargs)
Bases: `Protocol`

Handler Wrapper class.


#### \__init__(\*args, \*\*kwargs)

#### check(_: Type[[minos.networks.decorators.definitions.checkers.CheckDecorator](minos.networks.decorators.definitions.checkers.md#minos.networks.decorators.definitions.checkers.CheckDecorator)_ )

#### meta(_: minos.networks.decorators.callables.handlers.HandlerMet_ )
