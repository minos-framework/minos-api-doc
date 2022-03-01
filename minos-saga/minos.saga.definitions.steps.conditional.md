# minos.saga.definitions.steps.conditional module


### _class_ minos.saga.definitions.steps.conditional.ConditionalSagaStep(if_then=None, else_then=None, \*\*kwargs)
Bases: [`minos.saga.definitions.steps.abc.SagaStep`](minos.saga.definitions.steps.abc.md#minos.saga.definitions.steps.abc.SagaStep)

Conditional Saga Step class.


#### \__init__(if_then=None, else_then=None, \*\*kwargs)

#### commit(\*args, \*\*kwargs)
Commit the current `SagaStep` on the `Saga`.


* **Parameters**

    
    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    [`minos.saga.definitions.saga.Saga`](minos.saga.definitions.saga.md#minos.saga.definitions.saga.Saga)



* **Returns**

    A `Saga` instance.



#### conditional_step(\*args, \*\*kwargs)
Create a new conditional step in the `Saga`.


* **Parameters**

    
    * **args** – Additional positional parameters.


    * **kwargs** – Additional named parameters.



* **Return type**

    `minos.saga.definitions.steps.conditional.ConditionalSagaStep`



* **Returns**

    A new `SagaStep` instance.



#### else_then(saga)
Set the `ElseThenAlternative` with the given saga.


* **Parameters**

    **saga** ([`minos.saga.definitions.saga.Saga`](minos.saga.definitions.saga.md#minos.saga.definitions.saga.Saga)) – The saga to be executed if not any condition is met.



* **Return type**

    `minos.saga.definitions.steps.conditional.ConditionalSagaStep`



* **Returns**

    This method returns the same instance that is called.



#### _classmethod_ from_raw(raw, \*\*kwargs)
Build a new instance from raw.


* **Parameters**

    
    * **raw** (`typing.Union`[`dict`[`str`, `typing.Any`], [`minos.saga.definitions.steps.abc.SagaStep`](minos.saga.definitions.steps.abc.md#minos.saga.definitions.steps.abc.SagaStep)]) – A raw representation.


    * **kwargs** – Additional named arguments.



* **Return type**

    [`minos.saga.definitions.steps.abc.SagaStep`](minos.saga.definitions.steps.abc.md#minos.saga.definitions.steps.abc.SagaStep)



* **Returns**

    A `SagaStep` instance.



#### if_then(condition, saga)
Add a new `IfThenAlternative` based on a condition and a saga.


* **Parameters**

    
    * **condition** (`typing.Callable`[[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)], `typing.Union`[`bool`, `typing.Awaitable`[`bool`]]]) – The condition that must be satisfied to execute the alternative.


    * **saga** ([`minos.saga.definitions.saga.Saga`](minos.saga.definitions.saga.md#minos.saga.definitions.saga.Saga)) – The saga to be executed if the condition is satisfied.



* **Return type**

    `minos.saga.definitions.steps.conditional.ConditionalSagaStep`



* **Returns**

    This method returns the same instance that is called.



#### local_step(\*args, \*\*kwargs)
Create a new local step in the `Saga`.


* **Parameters**

    
    * **args** – Additional positional parameters.


    * **kwargs** – Additional named parameters.



* **Return type**

    [`minos.saga.definitions.steps.local.LocalSagaStep`](minos.saga.definitions.steps.local.md#minos.saga.definitions.steps.local.LocalSagaStep)



* **Returns**

    A new `SagaStep` instance.



#### _property_ raw(_: dict[str, Any_ )
Get the raw representation of the step.


* **Return type**

    `dict`[`str`, `typing.Any`]



* **Returns**

    A `dict` instance.



#### remote_step(\*args, \*\*kwargs)
Create a new remote step in the `Saga`.


* **Parameters**

    
    * **args** – Additional positional parameters.


    * **kwargs** – Additional named parameters.



* **Return type**

    [`minos.saga.definitions.steps.remote.RemoteSagaStep`](minos.saga.definitions.steps.remote.md#minos.saga.definitions.steps.remote.RemoteSagaStep)



* **Returns**

    A new `SagaStep` instance.



#### step(\*args, \*\*kwargs)
Create a new step in the `Saga`.


* **Parameters**

    
    * **args** – Additional positional parameters.


    * **kwargs** – Additional named parameters.



* **Return type**

    [`minos.saga.definitions.steps.abc.SagaStep`](minos.saga.definitions.steps.abc.md#minos.saga.definitions.steps.abc.SagaStep)



* **Returns**

    A new `SagaStep` instance.



#### validate()
Check if the step is valid.


* **Return type**

    `None`



* **Returns**

    This method does not return anything, but raises an exception if the step is not valid.



### _class_ minos.saga.definitions.steps.conditional.ElseThenAlternative(saga)
Bases: `object`

Else Then Alternative class.


#### \__init__(saga)

#### _classmethod_ from_raw(raw, \*\*kwargs)
Build a new instance from a raw representation.


* **Parameters**

    
    * **raw** (`typing.Union`[`dict`[`str`, `typing.Any`], `minos.saga.definitions.steps.conditional.ElseThenAlternative`]) – The raw representation.


    * **kwargs** – Additional named arguments.



* **Return type**

    `minos.saga.definitions.steps.conditional.ElseThenAlternative`



* **Returns**

    A new `ElseThenAlternative` instance.



#### _property_ raw(_: dict[str, Any_ )
Get the raw representation of the alternative.


* **Return type**

    `dict`[`str`, `typing.Any`]



* **Returns**

    A `dict` value.



#### validate()
Check if the alternative is valid.


* **Return type**

    `None`



* **Returns**

    This method does not return anything, but raises an exception if the alternative is not valid.



### _class_ minos.saga.definitions.steps.conditional.IfThenAlternative(condition, saga)
Bases: `object`

If Then Alternative class.


#### \__init__(condition, saga)

#### _classmethod_ from_raw(raw, \*\*kwargs)
Build a new instance from a raw representation.


* **Parameters**

    
    * **raw** (`typing.Union`[`dict`[`str`, `typing.Any`], `minos.saga.definitions.steps.conditional.IfThenAlternative`]) – The raw representation.


    * **kwargs** – Additional named arguments.



* **Return type**

    `minos.saga.definitions.steps.conditional.IfThenAlternative`



* **Returns**

    A new `IfThenAlternative` instance.



#### _property_ raw(_: dict[str, Any_ )
Get the raw representation of the alternative.


* **Return type**

    `dict`[`str`, `typing.Any`]



* **Returns**

    A `dict` value.



#### validate()
Check if the alternative is valid.


* **Return type**

    `None`



* **Returns**

    This method does not return anything, but raises an exception if the alternative is not valid.
