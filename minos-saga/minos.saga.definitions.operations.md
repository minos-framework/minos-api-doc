# minos.saga.definitions.operations module


### _class_ minos.saga.definitions.operations.SagaOperation(callback, parameters=None, \*\*kwargs)
Bases: `Generic`[`minos.saga.definitions.operations.T`]

Saga Step Operation class.


#### \__init__(callback, parameters=None, \*\*kwargs)

#### _classmethod_ from_raw(raw, \*\*kwargs)
Build a new instance from a raw representation.


* **Parameters**

    
    * **raw** (`typing.Union`[`dict`[`str`, `typing.Any`], `minos.saga.definitions.operations.SagaOperation`[`typing.TypeVar`(`T`, bound= `typing.Callable`)], `None`]) – A raw representation.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.Optional`[`minos.saga.definitions.operations.SagaOperation`[`typing.TypeVar`(`T`, bound= `typing.Callable`)]]



* **Returns**

    A `SagaStepOperation` instance if the `raw` argument is not `None`, `None` otherwise.



#### _property_ parameterized(_: boo_ )
parameterized getter.


* **Return type**

    `bool`



* **Returns**

    `True` if parameters are provided or `False` otherwise.



#### _property_ raw(_: dict[str, Any_ )
Generate a rew representation of the instance.


* **Return type**

    `dict`[`str`, `typing.Any`]



* **Returns**

    A `dict` instance.
