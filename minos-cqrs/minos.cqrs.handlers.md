# minos.cqrs.handlers module


### _class_ minos.cqrs.handlers.PreEventHandler()
Bases: `object`

Pre Event Handler class.


#### _async classmethod_ handle(diff, resolve_references=True, \*\*kwargs)
Handle Ref resolution for Events.


* **Parameters**

    
    * **diff** (`typing.TypeVar`(`T`)) – The instance containing `Ref` instances.


    * **resolve_references** (`bool`) – If `True` the resolution is performed, otherwise it is skipped.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`T`)



* **Returns**

    The original instance with the `Ref` references already resolved.
